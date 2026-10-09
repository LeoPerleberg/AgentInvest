# ETFs

Nota sobre faixas de referência: os valores numéricos deste documento (taxas, tracking error, liquidez, patrimônio, alocações) são referências para triagem, não regras absolutas. Devem ser interpretados conforme o tipo de ETF, o mercado e o momento. Itens marcados com "(verificar regra vigente)" dependem de legislação ou regulamentação que muda com frequência. Tickers citados servem apenas como ilustração, sem recomendação.

## O que é um ETF e por que usar

ETF (Exchange Traded Fund) é um fundo de índice negociado em bolsa como se fosse uma ação. Ele busca replicar a carteira de um índice de referência (ações, renda fixa, ouro, imóveis etc.). Ao comprar uma cota, o investidor passa a ter exposição proporcional a todos os ativos do índice.

Principais motivos para usar:

- **Diversificação imediata:** uma única cota dá acesso a dezenas, centenas ou milhares de ativos.
- **Custo baixo:** gestão passiva dispensa análise de ativos individuais e costuma ter taxas muito menores que fundos de gestão ativa.
- **Transparência:** a composição da carteira e a metodologia do índice são públicas.
- **Liquidez:** negociação em bolsa durante o pregão, com compra e venda a preço de mercado.
- **Simplicidade:** reduz a necessidade de selecionar ações e de decidir o momento de operar.
- **Disciplina:** o próprio índice faz o rebalanceamento e substitui ativos conforme suas regras.

Limitações: o ETF acompanha o índice, para o bem e para o mal. Não protege contra quedas do mercado que ele replica, e a qualidade do resultado depende da metodologia do índice e da eficiência da gestão.

## Gestão passiva e o efeito dos custos

Fundos de gestão ativa tentam superar o mercado e cobram taxas maiores (administração e, em alguns casos, performance). Estudos de longo prazo indicam que a maioria dos gestores ativos não supera consistentemente o índice depois dos custos. O ETF passivo, por ter custo baixo, parte com vantagem estrutural.

O custo corrói o resultado de forma composta. Uma taxa de 2% ao ano, quando comparada a uma taxa próxima de zero, retira uma fração crescente do ganho acumulado:

| Horizonte | Redução aproximada do retorno acumulado com taxa de 2% ao ano |
|---|---|
| 10 anos | cerca de 17% |
| 30 anos | cerca de 43% |
| 50 anos | cerca de 61% |

Os percentuais são ilustrativos e variam conforme a rentabilidade bruta assumida; a lição é que diferenças aparentemente pequenas de taxa pesam muito no longo prazo.

## ETFs na B3 versus ETFs no exterior

| Aspecto | ETFs na B3 | ETFs listados no exterior (ex.: EUA) |
|---|---|---|
| Moeda | Reais | Dólar (ou outra moeda do ativo) |
| Acesso | Conta em corretora brasileira | Conta internacional ou corretora com acesso a bolsas estrangeiras |
| Taxa de administração | Geralmente mais alta, por menor escala | Geralmente muito baixa nos maiores fundos, por escala |
| Variedade | Menor, mas crescente | Milhares de opções (ações, renda fixa, setores, commodities, moedas) |
| Câmbio | Em ETFs de ativos locais, não há; em ETFs de índices estrangeiros, a exposição cambial vem embutida | Conversão de moeda feita pelo investidor; incide IOF na remessa (verificar regra vigente) |
| Proventos | Regra do fundo; muitos ETFs brasileiros de ações reinvestem os proventos na cota | Muitos ETFs distribuem dividendos em caixa |
| Burocracia fiscal | Mais simples (IR sobre ganho de capital, apuração mensal) | Declaração anual e apuração em reais (verificar regra vigente) |
| Risco sucessório | Inventário no Brasil | Possível imposto de herança sobre ativos domiciliados nos EUA acima de um limite para não residentes (verificar regra vigente) |

### ETFs na B3 que replicam índices estrangeiros

Existem ETFs negociados na B3 que investem em ETFs ou índices estrangeiros (por exemplo, os que acompanham o S&P 500). Funcionam como um intermediário: o fundo local capta recursos em reais e compra o ETF original no exterior.

- **Vantagens:** não exige conta internacional, opera em reais, permite compra pelos canais habituais, simplifica a tributação e evita o imposto de herança americano sobre o patrimônio mantido no Brasil.
- **Desvantagens:** camada adicional de custo (taxa do fundo local somada à do ETF subjacente), liquidez e spread que podem ser piores que os do original, variedade limitada de estratégias e tracking difference potencialmente maior.
- **Conclusão prática:** vale comparar o custo total e a conveniência. Para valores menores ou quem quer evitar burocracia, a opção local pode ser razoável; para patrimônios maiores e foco em custo, o ETF original costuma ser mais eficiente.

BDRs de ETFs também existem, mas costumam ter menor liquidez e custos embutidos.

## Como o índice é construído

O ETF é tão bom quanto o índice que replica. Os pontos principais:

### Critérios de seleção

Cada índice define quais ativos entram e saem. O Ibovespa, por exemplo, é uma carteira teórica reavaliada periodicamente, com critérios baseados em liquidez: índice de negociabilidade (volume financeiro), presença em pregão (percentual mínimo de dias negociados) e exclusão de ações de preço muito baixo (penny stocks). Não há filtro de qualidade, lucratividade ou endividamento. Isso significa que o índice reflete o que é mais negociado, não necessariamente as empresas mais sólidas.

Já índices fatoriais ou de qualidade aplicam filtros adicionais, como retorno sobre capital, endividamento e consistência de lucros.

### Ponderação

| Método | Como funciona | Pontos de atenção |
|---|---|---|
| Valor de mercado (market cap weighted) | Peso proporcional ao tamanho da empresa | Padrão da maioria dos grandes índices; reduz risco de pequenas empresas, mas concentra nas maiores |
| Pesos iguais (equal weighted) | Todas as empresas têm o mesmo peso | Dá peso relevante a empresas pequenas e exige rebalanceamentos frequentes, o que aumenta custos e volatilidade |
| Fatorial ou por critério | Peso conforme qualidade, dividendos, baixa volatilidade etc. | Depende da robustez e da transparência da metodologia |

A ponderação por valor de mercado é a mais comum em ETFs amplos porque reflete o mercado de forma natural, tem baixo giro e custo menor.

### Rebalanceamento

Verifique a periodicidade da reavaliação da carteira (trimestral, semestral, anual). Rebalanceamentos mais frequentes aumentam giro e custos; menos frequentes podem deixar a carteira desatualizada.

## Tipos de ETFs

| Tipo | Descrição | Exemplos ilustrativos |
|---|---|---|
| Índice amplo | Replica um mercado inteiro ou grandes empresas de uma região | BOVA11 (Ibovespa), S&P 500 (VOO, IVV, SPY), Nasdaq 100 (QQQ) |
| Mercados desenvolvidos fora dos EUA | Ações de Europa, Japão, Canadá e Pacífico | VEA |
| Mercados emergentes | China, Índia, Taiwan, Brasil e outros | VWO, INDA |
| Small caps | Empresas de menor capitalização; maior volatilidade | SMAL11 |
| Setoriais | Um setor específico (consumo básico, energia, tecnologia, saúde) | XLP, IXC |
| Fatoriais e de qualidade | Filtram por qualidade, valor, baixa volatilidade, momentum | SPHQ |
| Dividendos | Empresas com histórico de pagamento de proventos | IDIV, DIVO11 |
| Imobiliário (REITs) | Fundos imobiliários internacionais; sensíveis a juros | VNQ |
| Renda fixa | Títulos públicos ou crédito corporativo, de diferentes prazos e riscos | IEF, TLT (Treasuries), LQD (grau de investimento), HYG (alto retorno) |
| Ouro e metais | Reserva de valor; não gera fluxo de caixa | IAU, SLV |
| Criptoativos | Exposição a criptomoedas; alta volatilidade | ETFs de bitcoin e outros |
| Temáticos | Teses específicas (inteligência artificial, games, ESG, nichos) | Diversos, geralmente de menor escala |

Características a observar em cada tipo:

- **Índice amplo:** base natural da carteira; baixo custo e grande diversificação, mas pode concentrar em poucas empresas grandes (em índices americanos, as maiores empresas de tecnologia chegam a ter peso relevante).
- **Setoriais:** concentram risco no ciclo do setor; úteis como complemento tático ou defensivo.
- **Qualidade e fatoriais:** costumam ter perfil mais defensivo, podendo ficar atrás do índice amplo em fases de forte alta de tecnologia.
- **Renda fixa:** avalie duration (sensibilidade a juros), risco de crédito e moeda. Treasuries curtos têm menor oscilação que os longos; high yield aproxima-se mais de ações em crises.
- **Ouro:** protege contra perda de poder de compra e instabilidade, mas não paga proventos; o peso deve ser pequeno e coerente com o patrimônio.
- **Temáticos:** a tese pode ser válida, mas tende a ter menos ativos, custo maior e maior risco de modismo. Devem ocupar fração pequena da carteira.

## Critérios de escolha

| Critério | O que olhar | Referência |
|---|---|---|
| Taxa de administração (expense ratio) | Custo anual total do fundo | ETFs amplos nos EUA: de 0,03% a 0,10%; setoriais e fatoriais: 0,10% a 0,40%; nichos: acima de 0,50% é caro. ETFs na B3: costumam ficar acima desses valores, avaliar caso a caso |
| Tracking difference | Diferença de retorno entre o ETF e o índice, normalmente próxima da taxa cobrada | Quanto menor e mais estável, melhor |
| Tracking error | Volatilidade da diferença de retorno em relação ao índice | Abaixo de 1% é desejável; valores próximos de 4% ou dados não divulgados indicam gestão ineficiente |
| Liquidez | Volume financeiro negociado por dia | Em ETFs internacionais, ao menos cerca de US$ 1 milhão por dia |
| Spread | Diferença entre preço de compra e de venda | Quanto menor, melhor; grandes ETFs têm spread mínimo |
| Patrimônio (AUM) | Tamanho do fundo | Em ETFs internacionais, evitar abaixo de cerca de US$ 100 milhões, pelo risco de baixa liquidez e de encerramento |
| Concentração | Número de ativos e peso das maiores posições | Fundos de nicho com 10 a 20 ativos oscilam muito mais; veja o peso das dez maiores posições |
| Composição real | Se a carteira corresponde à proposta | Desconfie de fundos com grande parte do patrimônio em caixa |
| Metodologia | Critérios do índice, ponderação, rebalanceamento | Prefira regras objetivas, transparentes e estáveis |
| Réplica | Física (compra os ativos) ou sintética (usa derivativos) | A física é mais simples de entender; a sintética tem risco de contraparte |
| Custos totais | Taxa, spread, corretagem, câmbio/IOF, impostos | Compare o custo completo, não só a taxa |
| Domicílio | País onde o fundo é constituído | Afeta tributação de proventos e risco sucessório (verificar regra vigente) |

Quando dois ETFs seguem exatamente o mesmo índice, a carteira é praticamente idêntica; o que os diferencia é a taxa. Por exemplo, entre fundos que replicam o S&P 500, a diferença de 0,03% para 0,09% ao ano decide a escolha em favor do mais barato, desde que liquidez e tamanho sejam adequados.

## Tributação

### ETFs nacionais (verificar regra vigente)

- **ETFs de renda variável:** imposto de 15% sobre o ganho de capital nas vendas; em operações day trade, 20%. Não há isenção para vendas até R$ 20 mil por mês, benefício que vale apenas para ações. O imposto é apurado pelo investidor e recolhido por guia (DARF) (verificar regra vigente).
- **ETFs de renda fixa:** tributação sobre o ganho conforme regra vigente para esses fundos, sem o mecanismo de come-cotas aplicável a alguns fundos tradicionais (verificar regra vigente).
- **Perdas:** podem ser compensadas com ganhos futuros na mesma categoria de ativos (verificar regra vigente).
- **ETFs de índices estrangeiros na B3:** seguem o regime dos ETFs nacionais, com apuração em reais e sem declaração de bens no exterior (verificar regra vigente).

### ETFs internacionais (verificar regra vigente)

- **Ganhos e proventos:** a legislação brasileira atual prevê tributação anual de aplicações financeiras no exterior, com apuração em reais e declaração obrigatória; há mecanismos para compensar o imposto pago no exterior (verificar regra vigente).
- **Declaração:** posições no exterior devem ser declaradas à Receita Federal e, acima de determinados valores, ao Banco Central (verificar regra vigente).
- **IOF:** incide na conversão de moeda; as alíquotas variam conforme a natureza da operação e podem mudar (verificar regra vigente).
- **Imposto de herança nos EUA:** para não residentes, ativos domiciliados nos EUA acima de um limite de isenção podem ser tributados em alíquotas progressivas que chegam a 40% (verificar regra vigente). Estratégias de mitigação incluem uso de ativos não domiciliados nos EUA, contas conjuntas ou estrutura patrimonial, com orientação profissional.

### Dividendos e domicílio do fundo

- **ETFs domiciliados nos EUA:** dividendos pagos a não residentes costumam sofrer retenção de 30% na fonte, por não haver tratado que reduza a alíquota para brasileiros (verificar regra vigente).
- **ETFs domiciliados na Irlanda ou em Luxemburgo (UCITS):** podem ter retenção menor sobre os dividendos recebidos das empresas americanas, graças a tratados tributários, e não estão sujeitos ao imposto de herança americano, por não serem ativos domiciliados nos EUA (verificar regra vigente). Muitos UCITS são de acumulação, isto é, reinvestem os proventos em vez de pagá-los, o que melhora a eficiência fiscal. O acesso a eles depende da corretora e das regras para investidores de varejo (verificar regra vigente).
- **ETFs de acumulação versus distribuição:** os de distribuição pagam dividendos em caixa; os de acumulação os reinvestem automaticamente na cota. Verifique qual modelo o fundo adota.

## Exemplos de uso em carteira por perfil

Referências genéricas, não recomendação. A proporção ideal depende de objetivos, prazo, patrimônio, tolerância a risco e do peso que a carteira internacional tem no total.

| Perfil | Papel dos ETFs | Composição ilustrativa da parcela em ETFs |
|---|---|---|
| Conservador | Núcleo da carteira, com ênfase em diversificação e defesa | Ampla parte em índice amplo ou qualidade, complementada por mercados desenvolvidos fora dos EUA, consumo básico e imobiliário; renda fixa de curto prazo em moeda forte; ouro em fração pequena apenas para patrimônios maiores |
| Moderado | Núcleo equilibrado, com espaço para escolhas individuais | Combinação de índice amplo ou qualidade com mercados desenvolvidos e alguns setores; renda fixa e imobiliário como estabilizadores |
| Arrojado | Núcleo menor, com maior peso em setores e regiões de maior volatilidade | Índice amplo como base, mais exposição a mercados emergentes, setores cíclicos ou tecnologia; renda fixa em menor proporção |

Princípios gerais:

- Use ETFs amplos e baratos como base e deixe temas, setores e nichos como complemento.
- Combine ETFs com baixa sobreposição para reduzir concentração (por exemplo, índice dos EUA, mercados desenvolvidos fora dos EUA e emergentes).
- Metais preciosos como proteção só costumam fazer sentido com patrimônio elevado; em fase inicial de acumulação, o custo de oportunidade tende a pesar mais.
- Revise periodicamente a alocação e rebalanceie quando uma classe se afastar muito do alvo.

## Passo a passo para comparar ETFs

1. **Defina o objetivo:** qual papel o ETF terá (núcleo, diversificação geográfica, defesa, renda, tese específica).
2. **Identifique o índice:** leia a metodologia, os critérios de seleção, a ponderação e a frequência de rebalanceamento.
3. **Liste candidatos que seguem o mesmo índice ou índices equivalentes.**
4. **Compare custos:** taxa de administração, spread, corretagem, câmbio e impostos.
5. **Avalie a qualidade da réplica:** tracking difference e tracking error em vários anos.
6. **Verifique tamanho e liquidez:** patrimônio, volume diário e spread médio.
7. **Analise a composição real:** número de ativos, peso das maiores posições, setores, países e parcela em caixa.
8. **Confira domicílio e tributação:** país de constituição, retenção sobre dividendos, risco sucessório e forma de tributar (verificar regra vigente).
9. **Verifique o modelo de proventos:** distribuição ou acumulação.
10. **Avalie sobreposição com o que você já possui** para não duplicar exposição.
11. **Decida pelo menor custo total entre alternativas equivalentes** e registre os critérios usados para revisar depois.

## Sinais de alerta

- Taxa de administração muito acima da média da categoria sem justificativa clara.
- Patrimônio pequeno, baixo volume e spreads largos.
- Tracking error elevado ou ausência de divulgação desses dados.
- Carteira com poucos ativos ou grande concentração em uma única posição.
- Grande parte do patrimônio em caixa, em desacordo com a proposta.
- Índice próprio, pouco transparente ou criado para vender uma tese da moda.
- Nome e marketing mais atraentes que a metodologia.
- Réplica sintética com contraparte pouco clara.
- Histórico recente de fechamento de ETFs similares ou liquidez dependente de poucos formadores de mercado.
- Promessas de retorno ou de proteção garantida.

## Erros comuns

- Escolher pelo desempenho passado recente em vez de pelo custo e pela metodologia.
- Concentrar o patrimônio em ETFs temáticos ou setoriais.
- Comprar vários ETFs com sobreposição alta e achar que está diversificado.
- Ignorar o custo total (spread, câmbio, IOF, impostos) e olhar apenas a taxa de administração.
- Confundir o nome do ETF com o conteúdo real da carteira.
- Desconsiderar o risco cambial em ETFs de índices estrangeiros.
- Ignorar domicílio do fundo, retenção de dividendos e risco sucessório.
- Operar em excesso, tratando o ETF como instrumento de curto prazo.
- Não rebalancear ou rebalancear sem critério.
- Assumir que o índice amplo local é de qualidade só por ser a referência do mercado.
- Esquecer de declarar posições e ganhos no exterior.
