---
name: busca-avancada-fiis-oceans14
description: "Busca avançada de FIIs usando o screener do site Oceans14 (oceans14.com.br) em fluxo assistido: gera a ficha de filtros baseada na base de conhecimento (P/VP, dividend yield contra FFO yield, vacância, número de imóveis, liquidez, tipo do fundo), o usuário aplica no Oceans14 e cola ou exporta o resultado, e o agente limpa, pontua, verifica os finalistas e devolve os candidatos em tabela. Use quando o usuário pedir busca, filtro, ranking ou triagem de fundos imobiliários no Oceans14."
argument-hint: "Perfil ou filtros (ex.: tijolo com P/VP até 1, vacância até 10%) e, se já tiver, o resultado do Oceans14"
---

# Busca Avançada de FIIs no Oceans14 (fluxo assistido)

Usa o screener do Oceans14 como fonte da triagem e a base de conhecimento como critério. O resultado é uma lista de candidatos, não uma recomendação; cada candidato ainda passa pela skill [analise-fiis-fiagros](../analise-fiis-fiagros/SKILL.md), sobretudo fundos de papel, Fiagro e FI-Infra.

## Limite de acesso (verificado em 09/10/2026)
O Oceans14 responde HTTP 403 a requisições automatizadas, tanto pela ferramenta de web quanto pelo terminal. Por isso o agente não consegue abrir o screener sozinho. Não tente contornar o bloqueio (outros cabeçalhos, proxies ou automação de navegador): o fluxo é assistido, com o usuário operando o site. Se em uma execução futura o site responder normalmente, o agente pode usá-lo diretamente, sem burlar proteções.

Se o usuário não puder operar o Oceans14, ofereça a alternativa de receber dele uma lista de fundos com os indicadores (de qualquer fonte) e seguir a partir da etapa de validação.

## Base de conhecimento
+ [fiis-fiagros.md](../../Docs/Base%20de%20conhecimento/fiis-fiagros.md): seção 2 (tipos), seção 3 (indicadores), seção 4 (juros e cotas), seção 5 (critérios e filtros de exclusão), seção 7 (sustentabilidade do rendimento), seção 9 (alocação), seção 12 (sinais de alerta), seção 13 (erros comuns).
+ [montagem-de-carteira.md](../../Docs/Base%20de%20conhecimento/montagem-de-carteira.md): seções 2 e 3 (peso de FIIs e diversificação).

## Procedimento
1. **Definir o perfil** (tijolo de qualidade, desconto com cautela ou renda). Sem instrução, use "Tijolo de qualidade" e declare. Valores do usuário prevalecem.
2. **Entregar a ficha de filtros** ao usuário (modelo abaixo), com valores, motivo na base e a observação de que os nomes dos indicadores devem ser casados com os do screener do Oceans14. Não invente nomes de campos nem de menus do site; se um indicador não existir lá, deixe-o para a verificação dos finalistas.
3. **Pedir o resultado**: o usuário aplica a ficha no Oceans14, ordena por P/VP ou por dividend yield e cola a tabela (ou anexa imagem ou exportação), informando a data da consulta e a ordenação. Peça pelo menos: ticker, segmento ou tipo, cotação, P/VP, dividend yield, vacância, número de imóveis, liquidez diária e valor de mercado; FFO yield, cap rate, taxa de administração e alavancagem, se o site mostrar.
4. **Validar o que veio**: conferir unidades (percentual em 0 a 100 ou decimal), data e colunas ausentes. Tratar vazio ou 0 como "sem dado" (comum em fundos de papel e de fundos). Descartar fundos sem negociação recente.
5. **Separar por tipo**: fundos de tijolo recebem a triagem completa; fundos de papel, fundos de fundos, Fiagro e FI-Infra recebem só preço e liquidez e vão para a verificação qualitativa. O tipo informado pelo site pode estar impreciso: reclassifique os finalistas pelo relatório gerencial.
6. **Aplicar os filtros que o screener não cobriu**, como DY menor ou igual ao FFO yield e liquidez mínima.
7. **Pontuar e ordenar** (ver "Pontuação").
8. **Verificar os finalistas** (top 10) no relatório gerencial mais recente (inquilinos e concentração, WALT, vencimentos, indexação, alavancagem, taxas, emissões recentes, composição do resultado) e, para papel, devedores, LTV, inadimplência e provisões. Para conferir os números, use `https://www.fundamentus.com.br/detalhes.php?papel=TICKER`. Se os dados do Oceans14 e da verificação divergirem, apresente os dois com a data.
9. **Entregar a tabela** no formato abaixo.

## Ficha de filtros para o Oceans14 (fiis-fiagros.md, seções 3 e 5)
Os marcados com (op.) são parâmetros operacionais de triagem que não constam na base.

| Indicador | Tijolo de qualidade (padrão) | Desconto com cautela | Renda |
|---|---|---|---|
| Tipo | Tijolo: logística, shoppings, lajes, varejo, hospital, hotel | Mesmos | Mesmos |
| P/VP | Entre 0,80 e 1,05 | Entre 0,60 e 0,90 (abaixo de 0,50 costuma indicar problema grave) | Até 1,05 |
| Dividend yield frente ao FFO yield | DY no máximo igual ao FFO yield | Idem | Idem |
| Dividend yield | (op.) comparar com a taxa livre de risco e a mediana do segmento; muito acima do segmento pede investigação | Idem | (op.) acima da mediana, abaixo do percentil 90 |
| Vacância | (op.) até 10% | (op.) até 20% | (op.) até 10% |
| Número de imóveis | Pelo menos 3 (evita monoativo) | Pelo menos 2 | Pelo menos 3 |
| Liquidez diária | (op.) a partir de R$1.000.000,00 | (op.) a partir de R$500.000,00 | (op.) a partir de R$1.000.000,00 |
| Valor de mercado | (op.) a partir de R$500.000.000,00 | (op.) a partir de R$200.000.000,00 | (op.) a partir de R$500.000.000,00 |
| Taxa de administração e gestão (se houver) | Até cerca de 1% a.a. no total | Idem | Idem |
| Alavancagem (se houver) | Baixa (referência abaixo de 50%) | Idem | Idem |

Fundos de papel (consulta separada): peça apenas P/VP, dividend yield, liquidez e valor de mercado, e deixe devedores, ratings, garantias, LTV, inadimplência e concentração para a verificação (seções 2.2 e 5.1).

## Pontuação (0 a 100)
Preço 30 (P/VP dentro da faixa, DY coberto pelo FFO yield), qualidade dos imóveis 40 (vacância, número de imóveis, cap rate frente aos pares), liquidez e porte 20, rendimento 10 (DY em relação ao segmento). Critério sem dado não pontua e vai para "Verificar".

## Regras e alertas
- DY acima do FFO yield de forma recorrente indica distribuir mais do que gera (seções 3.1 e 7).
- DY muito acima do segmento é prêmio de risco, não critério de compra (seções 3.1 e 13).
- P/VP abaixo de 0,50 vai para "armadilha provável" (seção 3.1).
- Vacância alta e persistente, monoativo, localização em decadência e gestão passiva em ativo com problemas são filtros de exclusão (seção 5.2).
- Selic alta pressiona as cotas; descontos em bons fundos podem ser oportunidade se a geração de caixa estiver preservada (seção 4).

## Formato de saída
1. **Filtros aplicados**: perfil, valores, quais são da base e quais operacionais; fonte (Oceans14), data informada pelo usuário e ordenação. Exiba valores monetários no formato R$9.999,99 (ponto nos milhares, vírgula nos centavos).
2. **Resumo do funil**: linhas recebidas, descartadas por critério, candidatos.
3. **Tabela de candidatos de tijolo** (até 10 linhas):

| # | Ticker | Tipo (reclassificado) | Cotação | P/VP | DY | FFO yield | DY menos FFO | Vacância | Imóveis | Liquidez diária | Pontos | Alertas |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

4. **Fundos de papel, FoF, Fiagro e FI-Infra** (tabela curta de P/VP, DY, liquidez), com o aviso de que dependem de análise de crédito.
5. **Verificar nos finalistas**: inquilinos, WALT, indexação, alavancagem, taxas, emissões, composição do resultado.
6. **Diversificação**: no máximo dois fundos por segmento na lista curta (fiis-fiagros.md, seção 9); a fatia total de FIIs segue o perfil do investidor (montagem-de-carteira.md, seção 2).
7. Aviso: triagem educacional, não é recomendação de investimento.

## Cuidados
- Não afirmar valores do Oceans14 que o usuário não forneceu.
- Não tratar rendimento alto como qualidade (seção 13).
- Informar quando poucos fundos passarem em vez de relaxar critérios sem avisar.
- A isenção de IR dos rendimentos e demais regras tributárias devem ser conferidas na regra vigente.
