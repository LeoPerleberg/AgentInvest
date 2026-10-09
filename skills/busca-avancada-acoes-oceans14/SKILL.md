---
name: busca-avancada-acoes-oceans14
description: "Busca avançada de ações brasileiras usando o screener do site Oceans14 (oceans14.com.br) em fluxo assistido: gera a ficha de filtros baseada na base de conhecimento (ROE, margem líquida, dívida, P/L, P/VP, dividend yield, liquidez, Graham e Bazin), o usuário aplica no Oceans14 e cola ou exporta o resultado, e o agente limpa, pontua, verifica as finalistas e devolve os candidatos em tabela. Use quando o usuário pedir busca, filtro, ranking ou triagem de ações no Oceans14."
argument-hint: "Perfil ou filtros (ex.: qualidade com DY acima de 6%, P/L até 12, ROE acima de 15%) e, se já tiver, o resultado do Oceans14"
---

# Busca Avançada de Ações no Oceans14 (fluxo assistido)

Usa o screener do Oceans14 como fonte da triagem e a base de conhecimento como critério. O resultado é uma lista de candidatas, não uma recomendação; cada candidata ainda passa pela skill [analise-acoes](../analise-acoes/SKILL.md).

## Limite de acesso (verificado em 09/10/2026)
O Oceans14 responde HTTP 403 a requisições automatizadas, tanto pela ferramenta de web quanto pelo terminal. Por isso o agente não consegue abrir o screener sozinho. Não tente contornar o bloqueio (outros cabeçalhos, proxies ou automação de navegador): o fluxo é assistido, com o usuário operando o site. Se em uma execução futura o site responder normalmente, o agente pode usá-lo diretamente, sem burlar proteções.

Se o usuário não puder operar o Oceans14, ofereça a alternativa de receber dele uma lista de tickers com os indicadores (de qualquer fonte) e seguir a partir da etapa de validação.

## Base de conhecimento
+ [acoes.md](../../Docs/Base%20de%20conhecimento/acoes.md): seção 3 (setores), seção 4 (indicadores), seção 5 (governança), seção 6 (preço justo), seção 7.2 (payout), seção 10 (sinais de alerta), seção 11 (erros comuns).
+ [montagem-de-carteira.md](../../Docs/Base%20de%20conhecimento/montagem-de-carteira.md): seção 3 (limite por ativo e por setor).

## Procedimento
1. **Definir o perfil** (qualidade, dividendos ou valor). Sem instrução, use "Qualidade" e declare. Valores do usuário prevalecem.
2. **Entregar a ficha de filtros** ao usuário (modelo abaixo), com valores, motivo na base e a observação de que os nomes dos indicadores devem ser casados com os do screener do Oceans14. Não invente nomes de campos nem de menus do site; se o usuário disser que um indicador não existe lá, deixe-o para a verificação das finalistas.
3. **Pedir o resultado**: o usuário aplica a ficha no Oceans14, ordena por ROE ou por dividend yield e cola a tabela (ou anexa imagem ou exportação), informando a data da consulta e o critério de ordenação. Peça pelo menos: ticker, setor, cotação, P/L, P/VP, dividend yield, ROE, margem líquida, dívida e liquidez; quanto mais colunas da ficha vierem, melhor.
4. **Validar o que veio**: conferir unidades (percentual em 0 a 100 ou decimal), data, colunas ausentes e linhas incompletas. Tratar vazio ou 0 como "sem dado". Deduplicar classes de ação da mesma empresa (manter a de maior liquidez). Separar bancos e seguradoras.
5. **Aplicar os filtros que o screener não cobriu** e calcular Graham e Bazin aproximados (abaixo).
6. **Pontuar e ordenar** (ver "Pontuação").
7. **Verificar as finalistas** (top 10 a 15) com fonte pública: `https://www.fundamentus.com.br/detalhes.php?papel=TICKER` (dívida líquida, EBIT, lucros, balanço), site de RI (payout, fatos relevantes) e segmento de listagem. Se os números do Oceans14 e da verificação divergirem, apresente os dois e a data de cada um.
8. **Entregar a tabela** no formato abaixo.

## Ficha de filtros para o Oceans14 (perfil Qualidade; ajuste conforme o perfil)
Os valores vêm de acoes.md, seção 4; os marcados com (op.) são parâmetros operacionais de triagem que não constam na base.

| Indicador | Condição | Motivo na base |
|---|---|---|
| Lucro líquido / P/L | Positivo; P/L até (op.) 25 | P/L inútil com prejuízo (seção 4.1) |
| ROE | Acima de 15% de forma consistente | seção 4.2 |
| ROIC | Acima de 10% e acima do custo de capital | seção 4.2 |
| Margem líquida | Acima de 10% | seção 4.2 |
| Dívida líquida/EBITDA | Até 2 (aceitável até 3 conforme o setor); se não houver, dívida líquida/patrimônio até (op.) 1 | seção 4.3 |
| Liquidez corrente | Acima de 1 | seção 4.3 |
| P/VP | Até (op.) 5; no perfil Valor, até 1,5 | seção 4.1 |
| Dividend yield | Positivo; no perfil Dividendos, acima de 6% (Bazin) | seções 4.1 e 6.2 |
| Payout | Abaixo de 100% | seção 4.4 |
| Crescimento da receita e do lucro | Positivo em 5 anos | seção 4.4 |
| Liquidez média diária | (op.) a partir de R$1.000.000,00 | seção 1.5 (impacto de baixa liquidez) |
| Setor | Excluir os que o usuário não quiser; compare pares do mesmo setor | seções 3 e 11 |

Perfil Dividendos: ROE acima de 10%, margem líquida acima de 8%, P/L até 15, P/VP até 2, dividend yield acima de 6%. Perfil Valor: ROE acima de 10%, P/L até 12, P/VP até 1,5 e margem de segurança de Graham positiva.

Bancos e seguradoras: peça uma consulta separada só com ROE, P/L, P/VP, dividend yield e liquidez, e sinalize "validar Basileia, inadimplência e eficiência" (seção 4.3).

## Cálculos a partir dos dados colados
- LPA = cotação / P/L; VPA = cotação / P/VP (só com P/L e P/VP positivos).
- **Graham** = raiz de (22,5 x LPA x VPA); margem de segurança = 1 - cotação / Graham (seção 6.1).
- **Teto de Bazin (aproximado)** = (dividend yield x cotação) / 0,06, com 12 meses de proventos; para decisão, use a média de vários anos (seção 6.2).

## Pontuação (0 a 100)
Qualidade 40 pontos (ROE, ROIC, margem líquida, crescimento), preço 30 (P/L, P/VP, margem de Graham), risco 20 (dívida, liquidez), proventos 10 (dividend yield, payout). Cada critério vale a sua fração do bloco quando atendido; critério sem dado não pontua e vai para "Verificar". No perfil Dividendos, proventos valem 30 e preço 10.

## Alertas
- Armadilha de valor: múltiplo baixo com ROE baixo, dívida alta ou lucro em queda (seção 4.5).
- Dividend yield muito acima do histórico ou payout acima de 100% (seções 7.2 e 10).
- Lucro atípico, grupamento recente, recuperação judicial, setor muito cíclico (seções 3.1 e 10).

## Formato de saída
1. **Filtros aplicados**: perfil, valores, quais são da base e quais operacionais; fonte (Oceans14), data informada pelo usuário e critério de ordenação. Exiba valores monetários no formato R$9.999,99 (ponto nos milhares, vírgula nos centavos).
2. **Resumo do funil**: linhas recebidas, descartadas por critério, candidatas.
3. **Tabela de candidatas** (até 10 ou 15 linhas):

| # | Ticker | Setor | Cotação | P/L | P/VP | DY | ROE | ROIC | Mrg. líq. | Dívida | Graham (margem) | Pontos | Alertas |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

4. **Verificar nas finalistas**: dívida líquida/EBITDA, histórico de lucros de 5 a 10 anos, segmento de listagem, payout, fatos relevantes.
5. **Concentração**: no máximo duas candidatas por setor (montagem-de-carteira.md, seção 3).
6. Aviso: triagem educacional, não é recomendação de investimento.

## Cuidados
- Não afirmar valores do Oceans14 que o usuário não forneceu.
- Indicar que a triagem não captura governança, qualidade do negócio nem eventos pontuais.
- Informar quando poucos papéis passarem em vez de relaxar critérios sem avisar.
