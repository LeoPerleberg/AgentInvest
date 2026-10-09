---
name: analise-etfs
description: "Analisar e comparar ETFs nacionais (B3: BOVA11, IVVB11, etc.) e internacionais (VOO, IVV, SPY, QQQ, VEA, VWO, VNQ, SPHQ, IEF, LQD, IAU): taxa de administração, tracking error, liquidez, spread, AUM, concentração, metodologia do índice, tributação e uso na carteira. Use quando o usuário pedir análise, comparação ou escolha de ETF, ou perguntar entre ETF e fundo ou ação."
argument-hint: "ETF(s) (ex.: VOO vs IVVB11) e objetivo (núcleo da carteira, setor, renda fixa, ouro)"
---

# Análise de ETFs

## Base de conhecimento
Consulte o arquivo antes de afirmar critérios, faixas ou regras:
- [etfs.md](<../../Docs/Base de conhecimento/etfs.md>): o que é e por que usar, gestão passiva e custos, ETFs na B3 versus exterior, construção do índice, tipos, critérios de escolha, tributação, uso por perfil, passo a passo, sinais de alerta e erros comuns.
- [montagem-de-carteira.md](<../../Docs/Base de conhecimento/montagem-de-carteira.md>): seções 2 e 3 (peso do exterior e diversificação).
- [acoes-exterior.md](<../../Docs/Base de conhecimento/acoes-exterior.md>): conta internacional, câmbio, W-8BEN, tributação e estate tax. [reserva-de-valor.md](<../../Docs/Base de conhecimento/reserva-de-valor.md>): ETFs de ouro e de criptoativos.

## Quando usar
- Escolher ou comparar ETFs de índice, setoriais, renda fixa, ouro ou temáticos.
- Decidir entre ETF no Brasil (B3) e ETF no exterior.
- Definir a parcela de ETFs na carteira.

## Conceitos-chave
- ETF é um fundo de índice negociado em bolsa: diversificação imediata, gestão passiva, custo baixo, transparência e liquidez. Acompanha o índice para o bem e para o mal e não protege contra quedas do mercado que replica.
- O custo corrói o resultado de forma composta: uma taxa de 2% ao ano reduz o retorno acumulado em cerca de 17% em 10 anos, 43% em 30 e 61% em 50 (valores ilustrativos).
- ETFs na B3 são simples de operar, mas os que replicam índices estrangeiros (ex.: IVVB11) somam a taxa do fundo local à do ETF subjacente. Para valores menores ou para evitar burocracia, a opção local pode ser razoável; para patrimônios maiores e foco em custo, o ETF original costuma ser mais eficiente (etfs.md, ETFs na B3 versus exterior).
- Índices nacionais selecionam ativos por critérios próprios: o Ibovespa é guiado por liquidez, sem filtro de qualidade, lucratividade ou endividamento. Verifique a metodologia antes de comprar.
- ETFs de acumulação reinvestem os proventos na cota; os de distribuição pagam em caixa. Verifique qual modelo o fundo adota.

## Critérios de escolha (etfs.md, Critérios de escolha)
Os valores são referências de triagem, não regras absolutas.

| Critério | O que olhar | Referência |
|---|---|---|
| Taxa de administração (expense ratio) | Custo anual total | ETFs amplos nos EUA: 0,03% a 0,10%; setoriais e fatoriais: 0,10% a 0,40%; nichos acima de 0,50% são caros. ETFs na B3 costumam ficar acima; avaliar caso a caso |
| Tracking difference e tracking error | Diferença de retorno e sua volatilidade em relação ao índice | Diferença próxima da taxa cobrada e estável; tracking error abaixo de 1% é desejável; valores próximos de 4% ou dados não divulgados indicam gestão ineficiente |
| Liquidez e spread | Volume diário e diferença entre compra e venda | Em ETFs internacionais, ao menos cerca de US$1.000.000,00 por dia; grandes ETFs têm spread mínimo |
| Patrimônio (AUM) | Tamanho do fundo | Em ETFs internacionais, evitar abaixo de cerca de US$100.000.000,00 (risco de baixa liquidez e encerramento) |
| Concentração | Número de ativos e peso das dez maiores posições | Nichos com 10 a 20 ativos oscilam muito mais |
| Metodologia | Critérios do índice, ponderação, rebalanceamento | Ponderação por valor de mercado é a mais comum em ETFs amplos; pesos iguais dão peso relevante a empresas pequenas e aumentam giro e custos |
| Réplica | Física ou sintética | A física é mais simples; a sintética tem risco de contraparte |
| Composição real | O que o fundo realmente carrega | Desconfiar de grande parte do patrimônio em caixa |
| Custos totais | Taxa, spread, corretagem, câmbio, IOF e impostos | Comparar o custo completo, não só a taxa |
| Domicílio e tributação | País do fundo, retenção sobre dividendos, risco sucessório | Ver seção de tributação abaixo |

Quando dois ETFs seguem exatamente o mesmo índice, a carteira é praticamente idêntica e a taxa decide, desde que liquidez e tamanho sejam adequados.

## Tipos (etfs.md, Tipos de ETFs)
- **Índice amplo**: S&P 500 (VOO, IVV, SPY), Nasdaq 100 (QQQ), Ibovespa (BOVA11). Base natural da carteira, mas pode concentrar em poucas empresas grandes.
- **Mercados desenvolvidos e emergentes**: VEA, VWO, INDA.
- **Small caps e dividendos**: SMAL11, IDIV, DIVO11.
- **Setoriais**: energia (IXC), consumo básico (XLP), imobiliário/REITs (VNQ). Concentram risco no ciclo do setor; servem de complemento.
- **Fatoriais e qualidade**: SPHQ. Perfil mais defensivo; podem ficar atrás em fases de forte alta de tecnologia.
- **Renda fixa**: Treasuries (IEF, TLT), crédito de qualidade (LQD), high yield (HYG). Avalie duration, risco de crédito e moeda.
- **Ouro e metais** (IAU, SLV) e **criptoativos**: ver reserva-de-valor.md; o peso deve ser pequeno e coerente com o patrimônio.
- **Temáticos e de nicho**: menos ativos, custo maior e risco de modismo; fração pequena da carteira.

## Tributação (etfs.md, Tributação; verificar regra vigente em todos os itens)
- **ETFs nacionais de renda variável**: imposto sobre ganho de capital (referência de 15%; 20% em day trade), sem a isenção mensal válida só para ações; apuração e recolhimento pelo investidor.
- **ETFs de índices estrangeiros na B3**: seguem o regime dos ETFs nacionais, em reais.
- **ETFs internacionais**: tributação anual de aplicações no exterior com apuração em reais, declaração à Receita (e ao Banco Central acima de certos valores) e IOF no câmbio.
- **Dividendos e domicílio**: ETFs domiciliados nos EUA sofrem retenção de 30% sobre dividendos para não residentes e podem gerar estate tax; ETFs irlandeses ou luxemburgueses (UCITS) podem ter retenção menor e não são ativos domiciliados nos EUA; muitos são de acumulação. O acesso depende da corretora.

## Procedimento (etfs.md, Passo a passo para comparar ETFs)
1. Definir o papel do ETF na carteira: núcleo, defesa, setor, renda fixa ou diversificador.
2. Identificar o índice: metodologia, critérios de seleção, ponderação e frequência de rebalanceamento.
3. Listar candidatos que seguem o mesmo índice ou equivalentes; coletar dados atuais (taxa, AUM, volume, composição, tracking) na página do emissor ou em fonte pública, com data.
4. Comparar custos totais e a qualidade da réplica (tracking em vários anos).
5. Verificar tamanho e liquidez, composição real (número de ativos, peso das maiores posições, setores, países, caixa).
6. Verificar a diferença entre a versão na B3 e a do exterior: custo total, câmbio, tributação e burocracia.
7. Conferir domicílio, tributação e modelo de proventos (acumulação ou distribuição).
8. Dimensionar o peso na carteira e a sobreposição com ações e fundos já existentes.
9. Decidir pelo menor custo total entre alternativas equivalentes e registrar os critérios.

## Uso na carteira (etfs.md, Exemplos de uso por perfil; referências, ajustar ao perfil)
- Conservador: ETFs como núcleo, com ênfase em diversificação e defesa (índice amplo ou qualidade, mercados desenvolvidos fora dos EUA, consumo básico, imobiliário, renda fixa de curto prazo); ouro em fração pequena só para patrimônios maiores.
- Moderado: núcleo equilibrado, com espaço para escolhas individuais; renda fixa e imobiliário como estabilizadores.
- Arrojado: núcleo menor, com mais exposição a emergentes, setores cíclicos ou tecnologia.
- Use ETFs amplos e baratos como base, deixe temas e nichos como complemento e combine ETFs com baixa sobreposição.

## Sinais de alerta (etfs.md, Sinais de alerta e Erros comuns)
- Taxa muito acima da média da categoria sem justificativa.
- Baixo volume, AUM pequeno ou spread alto; tracking error elevado ou não divulgado.
- ETF temático muito concentrado, índice próprio pouco transparente ou criado para vender tese da moda.
- Grande parte do patrimônio em caixa; réplica sintética com contraparte pouco clara.
- Escolher por desempenho passado recente; comprar vários ETFs com sobreposição alta e achar que está diversificado.
- Ignorar câmbio, IOF, domicílio, retenção de dividendos, risco sucessório e a declaração de posições no exterior.

## Formato de saída
1. Resumo e recomendação qualitativa (2 a 4 linhas).
2. Tabela comparativa: taxa, AUM, liquidez, tracking, número de ativos, domicílio.
3. Diferenças entre versão B3 e exterior, quando aplicável.
4. Papel na carteira e peso sugerido.
5. Riscos e pontos de atenção.
6. Fontes e data dos dados.
