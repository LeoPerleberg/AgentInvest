---
name: analise-acoes
description: "Analisar ações brasileiras (B3) de forma fundamentalista: setor, qualidade da empresa, indicadores (P/L, P/VP, ROE, margens, dívida líquida/EBITDA, payout, dividend yield), preço justo (Graham, Bazin), proventos (dividendos, JCP, desdobramento, grupamento, bonificação) e encaixe na carteira. Use quando o usuário pedir análise, comparação ou valuation de uma ação, ticker com final 3/4/11, ou dúvida sobre dividendos e data ex."
argument-hint: "Ticker ou empresa (ex.: WEGE3, BBAS3) e objetivo (renda, crescimento, comparação)"
---

# Análise de Ações (Brasil)

## Base de conhecimento
Consulte o arquivo antes de afirmar critérios, faixas ou fórmulas:
+ [acoes.md](../../Docs/Base%20de%20conhecimento/acoes.md): seção 1 (conceitos e termos), seção 2 (estratégias), seção 3 (setores), seção 4 (indicadores), seção 5 (qualidade e governança), seção 6 (preço justo), seção 7 (proventos e eventos corporativos, inclui preço médio), seção 8 (reinvestimento), seção 9 (passo a passo), seção 10 (sinais de alerta), seção 11 (erros comuns).
+ [montagem-de-carteira.md](../../Docs/Base%20de%20conhecimento/montagem-de-carteira.md): seções 2 a 4 (alocação por perfil, diversificação e rebalanceamento).
+ Para ETFs de índice nacional ou ativos fora do Brasil: [etfs.md](../../Docs/Base%20de%20conhecimento/etfs.md) e [acoes-exterior.md](../../Docs/Base%20de%20conhecimento/acoes-exterior.md).

## Quando usar
- Analisar ou comparar empresas listadas na B3.
- Estimar preço justo ou margem de segurança.
- Entender proventos e eventos corporativos.
- Decidir se uma ação cabe na carteira.

## Princípios do método
- Investimento de longo prazo (referência de 10 anos ou mais), com compra de boas empresas a preço razoável e margem de segurança. Day trade e swing trade são tratados como especulação (acoes.md, seções 1.5 e 2).
- Estratégias de valor, crescimento e comprar e manter não se excluem; escolha conforme o perfil do investidor (acoes.md, seção 2).
- O setor vem antes da empresa. Preferir setores perenes, pouco dependentes de regulação e previsíveis (ex.: financeiro, materiais básicos, saúde, utilidade pública, consumo não cíclico). Setores muito cíclicos exigem mais cautela (acoes.md, seção 3).
- Qualidade vale mais do que dividendo alto. Dividend yield elevado isolado não é critério de compra (acoes.md, seções 7.2 e 11).
- Diversificação mínima de cerca de 10 empresas com aportes equilibrados (acoes.md, seção 2; montagem-de-carteira.md, seção 3).

## Procedimento
1. **Objetivo e perfil**: renda, crescimento ou carteira equilibrada; horizonte.
2. **Setor** (acoes.md, seção 3.1): perenidade, regulação, ciclicidade, riscos externos, previsibilidade, intensidade de capital. Compare a empresa com pares do mesmo setor.
3. **Dados** (acoes.md, seção 4): obtenha os indicadores atuais e os dos últimos anos (idealmente 5 a 10) com fonte e data (ex.: site de RI da empresa, sites agregadores de dados). Leia resultados, notas explicativas e fatos relevantes (acoes.md, seção 9).
4. **Qualidade** (acoes.md, seções 3.2 e 5): aplique o checklist abaixo.
5. **Preço** (acoes.md, seção 6): calcule os preços justos e compare com a cotação.
6. **Proventos** (acoes.md, seção 7): verifique consistência e sustentabilidade.
7. **Governança e riscos** (acoes.md, seções 5 e 10): segmento de listagem, free float, tag along, controlador, diluição, integridade da gestão.
8. **Carteira** (montagem-de-carteira.md, seções 3 e 4): peso proposto, concentração por setor e correlação com o que já existe.
9. **Veredito**: faixa qualitativa (ex.: atrativa, neutra, cara/evitar) com justificativa e gatilhos de revisão. Venda por deterioração dos fundamentos, não por oscilação de preço.

## Indicadores e referências (acoes.md, seção 4)
As faixas são referências de triagem, não regras absolutas. Compare empresas do mesmo setor e olhe vários anos.

| Indicador | Fórmula | Leitura / referência |
|---|---|---|
| P/L | Preço / LPA | Anos de lucro pagos; comparar com o setor. Baixo pode ser barato ou empresa em dificuldade; não útil com prejuízo |
| P/VPA | Preço / VPA | Abaixo de 1: preço menor que o patrimônio; até cerca de 1,5 costuma ser tolerado em valor. Pode enganar em negócios leves em ativos (serviços, tecnologia) |
| EV/EBITDA | (Valor de mercado + dívida líquida) / EBITDA | Compara empresas com endividamentos distintos |
| Dividend Yield | Proventos 12m / preço | Bazin: mínimo de 6% a.a.; DY muito alto pode ser queda de preço ou provento não recorrente |
| Payout | Proventos / lucro líquido | Acima de 100% só é sustentável de forma pontual, com caixa excedente |
| ROE | Lucro líquido / patrimônio líquido | Referência: acima de 10% a 15% de forma consistente; ROE alto com muita dívida exige cautela |
| ROIC | Lucro operacional após impostos / capital investido | Mais abrangente que o ROE; deve superar o custo de capital |
| Margem líquida | Lucro líquido / receita líquida | Referência: cerca de 8% a 10% ou mais, variando por setor |
| Margem bruta e EBIT | Lucro bruto ou EBIT / receita líquida | Eficiência de produção e operação; avaliar a tendência |
| Dívida líquida / EBITDA | (Dívida bruta menos caixa) / EBITDA | Perfil conservador busca até cerca de 2; algumas triagens aceitam até 3, conforme o setor |
| Liquidez corrente e cobertura de juros | Ativo circulante / passivo circulante; EBIT / despesa financeira | Liquidez corrente acima de 1 é desejável; cobertura mostra a folga para pagar juros |
| CAGR de receita e lucro | (Valor final / valor inicial)^(1/anos) - 1 | Avaliar em 5 a 10 anos e comparar com o setor |
| Consistência de lucros | Lucro positivo ano a ano | Conservadores buscam pelo menos 5 a 10 anos |

Interpretação em conjunto (acoes.md, seção 4.5): múltiplo baixo com ROE baixo, dívida alta e lucro em queda é armadilha de valor, não oportunidade. Monte uma tabela de pares do mesmo setor.

Em bancos e seguradoras, não use dívida líquida/EBITDA da mesma forma; use ROE, Basileia, inadimplência e eficiência.

## Preço justo (acoes.md, seção 6)
- **Graham** (seção 6.1): preço justo = raiz quadrada de (22,5 x LPA x VPA); 22,5 vem de P/L máximo de 15 x P/VP máximo de 1,5. Só vale com LPA e VPA positivos; funciona melhor em empresas maduras e lucrativas e ignora crescimento e dívida. Margem de segurança = 1 menos (preço atual / preço justo).
- **Bazin** (seção 6.2): preço teto = dividendo médio anual por ação de vários anos / 0,06. Exige histórico consistente de pagamentos e baixo endividamento.
- **Múltiplos e fluxo de caixa descontado** (seção 6.3): compare P/L ou EV/EBITDA com a mediana do setor e o histórico da própria empresa; o fluxo de caixa descontado é muito sensível às premissas.
- Exija margem de segurança. Mostre sempre as premissas e a sensibilidade; se os métodos divergirem muito, explique por quê.

## Checklist de qualidade (acoes.md, seções 3.2 e 5)
Produto com potencial duradouro; vantagem competitiva; margens e controle de custos; gestão íntegra e estável; transparência em crises; baixa diluição acionária (follow-ons); estratégia de longo prazo; P&D e inovação quando aplicável.

Governança (seções 5.1 e 5.2): o Novo Mercado exige apenas ações ON, free float mínimo de 25% e tag along de 100%; os demais segmentos têm exigências menores (verificar regra vigente). Avalie o perfil do controlador (família, Estado, pulverizado); controle estatal tende a gerar desconto estrutural nos múltiplos.

## Proventos e eventos corporativos (acoes.md, seções 7 e 8)
- **Dividendos** (seções 7.2 e 7.3): dependem de lucro; o preço cai na data ex. Comprar na véspera não gera ganho real. Empresa que reinveste todo o lucro e não paga dividendos não é pior por isso.
- **JCP** (seção 7.4): dedutível para a empresa e com retenção na fonte (referência de 15%).
- **Data com / data ex**: quem compra a partir da data ex não recebe o provento.
- **Desdobramento e grupamento** (seção 7.5): o desdobramento aumenta a quantidade de ações sem alterar o valor total; o grupamento reduz a quantidade e costuma ocorrer quando a cotação fica abaixo de R$1,00 (sinal de alerta; gráficos ajustados escondem a perda histórica).
- **Bonificação, subscrição e diluição** (seção 7.6): quem não exerce nem vende o direito perde participação.
- **Preço médio** (seção 7.7): total investido com custos / quantidade; base do ganho de capital. Baixar o preço médio só faz sentido se os fundamentos continuam firmes.
- **Reinvestimento** (seção 8): na acumulação, reinvestir 100% dos proventos; use-os também para rebalancear.
- Confirme a tributação vigente de dividendos, JCP e da venda de ações (seção 7.8); as regras podem ter mudado.

## Sinais de alerta (acoes.md, seções 10 e 11)
- Dividend yield muito acima do histórico com lucro em queda ou payout acima de 100%.
- Endividamento crescente, margens em queda, fraude contábil ou governança fraca.
- Emissões de ações recorrentes, comunicação só de boas notícias em crises.
- Setor altamente cíclico ou regulado comprado no pico do ciclo.
- Confundir ação barata em reais com ação barata em fundamentos.
- Lucro atípico por evento não recorrente, grupamento de ações, recuperação judicial, auditoria com ressalvas.
- Comparar empresas de setores diferentes pelos mesmos múltiplos; tratar o Ibovespa como filtro de qualidade (seus critérios priorizam negociabilidade).

## Formato de saída
1. Resumo e veredito (2 a 4 linhas).
2. Tabela de indicadores: valor, referência, leitura.
3. Preço justo (Graham, Bazin, múltiplos) e margem de segurança.
4. Qualidade, governança e proventos.
5. Riscos e gatilhos de revisão.
6. Encaixe na carteira (peso sugerido e concentração).
7. Fontes e data dos dados.
