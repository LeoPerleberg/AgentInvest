---
name: analise-renda-fixa
description: "Analisar e comparar títulos de renda fixa: Tesouro Selic, Prefixado, IPCA+ (com ou sem juros semestrais), Renda+, Educa+, CDB, RDB, LC, LCI, LCA, CRI, CRA, debêntures, fundos de renda fixa e previdência. Cobre rentabilidade líquida após IR, indexadores (Selic, CDI, IPCA), marcação a mercado, FGC, risco de crédito, reserva de emergência e escolha de prazo. Use quando o usuário pedir para comparar taxas, decidir onde aplicar, calcular rentabilidade líquida ou dimensionar a parcela de renda fixa."
argument-hint: "Produtos ou taxas a comparar (ex.: CDB 110% CDI vs LCI 92% CDI) e prazo/objetivo"
---

# Análise de Renda Fixa

## Base de conhecimento
Consulte o arquivo antes de afirmar critérios, taxas ou regras:
+ [renda-fixa.md](../../Docs/Base%20de%20conhecimento/renda-fixa.md): seção 1 (conceitos), seção 2 (segurança, custódia e FGC), seção 3 (Tesouro Direto), seção 4 (títulos bancários), seção 5 (crédito privado), seção 6 (fundos), seção 7 (previdência), seção 8 (avaliação de risco de crédito), seção 9 (tributação e custos), seção 10 (marcação a mercado), seção 11 (fórmulas e comparações), seção 12 (reserva de emergência e vencimento), seção 13 (boas práticas de compra), seção 14 (passo a passo), seção 15 (sinais de alerta), seção 16 (erros comuns).
+ [montagem-de-carteira.md](../../Docs/Base%20de%20conhecimento/montagem-de-carteira.md): seção 2 (fatia de renda fixa por perfil) e seção 6 (reserva de emergência).
+ Para comparar com FIIs de papel, Fiagro e FI-Infra: [fiis-fiagros.md](../../Docs/Base%20de%20conhecimento/fiis-fiagros.md). Para renda fixa no exterior: [acoes-exterior.md](../../Docs/Base%20de%20conhecimento/acoes-exterior.md) seção 7.

## Quando usar
- Comparar produtos e taxas com IR e prazos diferentes.
- Escolher onde aplicar reserva de emergência, metas de curto prazo e longo prazo.
- Avaliar risco de crédito, liquidez e marcação a mercado.
- Definir a fatia de renda fixa na carteira.

## Conceitos-chave (renda-fixa.md, seções 1 e 2)
- Renda fixa é um empréstimo com regras de remuneração conhecidas na contratação; "fixa" refere-se à regra, não ao valor. Dá previsibilidade e estabilidade, mas não é isenta de risco.
- Indexadores: **Selic** (Tesouro Selic), **CDI** (cerca de 0,10 ponto abaixo da Selic; referência de CDB, LCI, LCA e debêntures pós-fixadas), **IPCA** (títulos IPCA+), **prefixado** (taxa conhecida na compra), **híbrido** (parte prefixada mais inflação).
- Rentabilidade deve ser avaliada em termos líquidos e reais: `real = (1 + nominal) / (1 + inflação) - 1`.
- Riscos: crédito, mercado (marcação a mercado), liquidez (carência) e reinvestimento.
- Os títulos ficam registrados em nome do investidor em câmaras de registro (B3 e outros), não no patrimônio da corretora; o saldo parado em conta, sem aplicação, pode ficar exposto.

## Produtos (renda-fixa.md, seções 3 a 7)
| Produto | Características | Para que serve |
|---|---|---|
| Tesouro Selic (seção 3.1) | Pós-fixado, oscilação mínima de preço, resgate em D+1 útil; IOF regressivo nos primeiros 30 dias (verificar regra vigente) | Reserva de emergência, caixa estratégico, curto prazo |
| Tesouro Prefixado (seção 3.2) | Taxa fixa, R$1.000,00 no vencimento; marcação a mercado | Travar taxa atrativa até objetivo com data; expectativa de queda de juros |
| Tesouro IPCA+ (seção 3.3) | Inflação mais taxa real; oscila bastante em prazos longos; IR sobre o ganho nominal | Preservar poder de compra em objetivos de longo prazo |
| Juros semestrais (seção 3.4) | Cupons a cada 6 meses, tributados pela tabela regressiva | Fase de renda; na acumulação reduz o efeito composto |
| Renda+ e Educa+ (seção 3.5) | Variantes do IPCA+ com pagamento em parcelas mensais no fim | Aposentadoria e educação |
| CDB, RDB e LC (seção 4.1) | Bancos e financeiras; prefixado, % do CDI ou IPCA + taxa; FGC dentro do limite | Reserva com liquidez diária em banco sólido; objetivos de 1 a 5 anos |
| LCI e LCA (seção 4.2) | Isentas de IR para pessoa física; prazo mínimo regulatório; FGC; risco do banco emissor | Curto e médio prazos; comparar com CDB pela taxa líquida |
| CRI e CRA (seção 5.1) | Isentos de IR; sem FGC; pagam mais pelo risco; liquidez menor | Risco de crédito privado com diversificação e análise de rating, lastro e garantias |
| Debêntures (seção 5.2) | Comuns tributadas pela tabela regressiva; incentivadas podem ser isentas; sem FGC; liquidez baixa | Parte moderada da carteira; taxa deve compensar o risco |
| Fundos de renda fixa (seção 6) | Taxa de administração e performance, come-cotas | Comprar títulos diretamente costuma ter custo menor; comparar retorno líquido com o CDI e o Tesouro Selic |
| Previdência PGBL e VGBL (seção 7) | Sem come-cotas; PGBL deduz até 12% da renda bruta (declaração completa); VGBL tributa só o rendimento; tabela regressiva ou progressiva | Aposentadoria e sucessão; cuidado com taxas de administração, carregamento e saída; portabilidade |

## Procedimento (renda-fixa.md, seções 8, 12, 13 e 14)
1. **Objetivo e prazo**: reserva de emergência, meta de curto, médio ou longo prazo, acumulação ou renda. Separe a reserva de emergência primeiro, com liquidez e baixo risco.
2. **Indexador conforme o objetivo**: Selic/CDI para liquidez e caixa, IPCA+ para preservar poder de compra, prefixado para travar taxa.
3. **Dados atuais**: coletar taxas e emissores (Tesouro Direto, corretora, Banco Central, ANBIMA) em mais de uma plataforma, com data; Selic, CDI e IPCA atuais precisam ser confirmados. O mercado secundário tende a ter ofertas melhores nas primeiras horas do pregão (por volta das 10h).
4. **Rentabilidade líquida**: converta tudo para o mesmo prazo e base, após IR (fórmulas abaixo).
5. **Risco de crédito** (seção 8): bancos pelo índice de Basileia (mínimo regulatório em torno de 10,5%; muitos analistas buscam folga acima de 12%, referência e não regra), liquidez, qualidade da carteira e histórico; empresas e crédito privado pelo rating (AAA a D), lastro, garantias, alavancagem e documentos da emissão. Taxa muito acima do mercado significa risco maior.
6. **FGC** (seção 2): referência de R$250.000,00 por CPF por instituição (conglomerado) e R$1.000.000,00 por CPF a cada 4 anos (verificar regra vigente); distribuir valores altos entre instituições diferentes. Tesouro, debêntures, CRI, CRA, fundos e previdência não têm cobertura do FGC.
7. **Liquidez e marcação a mercado**: alinhar o vencimento à data em que o dinheiro será necessário; avaliar o impacto de vender antes.
8. **Cenário**: prefixados com taxas altas após alta de juros e IPCA+ com taxas reais altas costumam ser oportunidades de longo prazo, mas não decida por medo ou euforia do momento; confirme com a análise.
9. **Diversificar** por emissor, indexador e vencimento; escalonar vencimentos reduz o risco de reinvestimento.
10. **Conclusão**: ranking dos produtos por rentabilidade líquida ajustada ao risco e à liquidez.

## Tributação (renda-fixa.md, seção 9; confirmar a regra vigente)
| Prazo da aplicação | IR regressivo |
|---|---|
| Até 180 dias | 22,5% |
| 181 a 360 dias | 20% |
| 361 a 720 dias | 17,5% |
| Acima de 720 dias | 15% |

- Aplica-se a Tesouro, CDB, RDB, LC, debêntures comuns e fundos de longo prazo (regras próprias); incide sobre o rendimento e é retido na fonte. LCI, LCA, CRI, CRA e debêntures incentivadas são isentos para pessoa física.
- IOF sobre o rendimento em resgates nos primeiros 30 dias, com alíquota decrescente.
- Fundos têm come-cotas semestral (maio e novembro): 15% em fundos de longo prazo ou 20% em curto prazo, com complemento no resgate. Previdência não tem come-cotas e tem tabela própria (regressiva de 35% a 10% ou progressiva).
- Em inflação alta, o IR sobre o ganho nominal reduz a rentabilidade real.
- Considere a taxa de custódia do Tesouro, taxas de fundos e previdência e a margem do distribuidor (o mesmo título pode ter taxas diferentes em plataformas diferentes).

## Cálculos úteis (renda-fixa.md, seção 11)
- **Rendimento líquido** = bruto x (1 menos alíquota de IR). Ex.: 12% ao ano bruto com IR de 20% rende 9,6% líquido.
- **Taxa bruta equivalente de um isento** = taxa do isento / (1 menos alíquota). Ex.: LCI de 90% do CDI equivale a CDB de cerca de 116% do CDI até 180 dias, 112,5% de 181 a 360 dias, 109% de 361 a 720 dias e 105,9% acima de 720 dias.
- **% do CDI**: retorno bruto aproximado = CDI x percentual. Compare sempre no mesmo prazo.
- **IPCA+**: `(1 + taxa real) x (1 + IPCA) - 1`; por exemplo, 5% mais 9% de inflação dá cerca de 14,45%. O IR incide sobre o ganho nominal.
- **Prefixado versus IPCA+**: compare a inflação implícita no prefixado com a que você espera; inflação esperada maior favorece o IPCA+, menor favorece o prefixado.
- Compare sempre valores líquidos, mesmo prazo e mesmo risco de crédito.

## Reserva de emergência e vencimento (renda-fixa.md, seção 12)
- Reserva: 6 a 12 meses de despesas essenciais (referência; depende da estabilidade da renda), em Tesouro Selic ou CDB de liquidez diária em banco sólido (dentro do limite do FGC); evite carência e marcação a mercado relevante.
- Horizonte: até 1 ano (Tesouro Selic, CDB de liquidez diária, LCI/LCA curtas); 1 a 5 anos (prefixados ou IPCA+ com vencimento próximo da data do objetivo, CDB, LCI/LCA); acima de 5 anos (IPCA+, Renda+, Educa+, debêntures incentivadas, previdência).

## Marcação a mercado (renda-fixa.md, seção 10)
- Preço de prefixados e IPCA+ varia diariamente com os juros: juros sobem, preço cai; juros caem, preço sobe; o efeito é maior em prazos longos. Todos convergem ao valor de resgate no vencimento.
- Manter até o vencimento garante a taxa contratada; vender antes pode gerar ganho ou perda.
- Regra prática: só antecipe a venda se a taxa líquida da nova aplicação, pelo prazo restante, superar o retorno líquido de manter o título (considere IR, IOF e custos).
- Debêntures e títulos bancários têm menor liquidez e preços menos transparentes no secundário.

## Sinais de alerta (renda-fixa.md, seções 15 e 16)
- Comparar taxa bruta com líquida, ou isento com tributado, ou indexadores e prazos diferentes sem converter.
- Emissor com baixa solidez ou sem informações públicas oferecendo taxa muito acima do mercado; promessa de retorno "garantido".
- Produto sem FGC vendido como "seguro"; exceder o limite do FGC em um único banco.
- Recomendação insistente de produto que gera comissão alta; pressão para aplicar rápido.
- Juros semestrais na fase de acumulação; reserva de emergência em títulos com carência ou volatilidade.
- Fundos e previdências com taxas altas (administração, carregamento, saída, performance).
- Investir em CRI, CRA e debêntures sem análise de crédito; títulos de capitalização apresentados como investimento.
- Esquecer que resgate antecipado pode gerar IR maior (faixa de prazo menor) e IOF.

## Formato de saída
1. Resumo e conclusão (2 a 4 linhas).
2. Tabela comparativa: produto, taxa, prazo, IR, rentabilidade líquida, liquidez, risco.
3. Premissas de Selic, CDI e IPCA com fonte e data.
4. Riscos e pontos de atenção (crédito, FGC, marcação a mercado).
5. Sugestão de uso por objetivo (reserva, meta, aposentadoria).
