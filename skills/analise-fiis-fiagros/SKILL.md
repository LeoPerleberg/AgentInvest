---
name: analise-fiis-fiagros
description: "Analisar fundos imobiliários (FIIs), Fiagros e FI-Infra: tipo (tijolo, papel high grade/high yield, fundo de fundos, desenvolvimento, híbrido), P/VP, dividend yield, vacância, WALT, inadimplência, LTV, FFO, liquidez, taxa de administração, concentração de inquilinos e alocação. Use quando o usuário pedir análise ou comparação de um fundo com ticker final 11 (ex.: HGLG11, KNRI11, MXRF11), renda mensal, ou carteira de fundos."
argument-hint: "Ticker do fundo (ex.: KNRI11) ou lista para comparar"
---

# Análise de FIIs e Fiagros

## Base de conhecimento
Consulte o arquivo antes de afirmar critérios, faixas ou regras:
+ [fiis-fiagros.md](../../Docs/Base%20de%20conhecimento/fiis-fiagros.md): seção 1 (funcionamento e tributação), seção 2 (tipos), seção 3 (indicadores), seção 4 (juros e cotas), seção 5 (seleção e filtros), seção 6 (qualidade), seção 7 (sustentabilidade do rendimento), seção 8 (riscos), seção 9 (alocação), seção 10 (reinvestimento), seção 11 (passo a passo), seção 12 (sinais de alerta), seção 13 (erros comuns).
+ [montagem-de-carteira.md](../../Docs/Base%20de%20conhecimento/montagem-de-carteira.md): seções 2 e 3 (peso de FIIs por perfil e diversificação).
+ Para REITs americanos: [acoes-exterior.md](../../Docs/Base%20de%20conhecimento/acoes-exterior.md) seção 6.5. Para renda fixa que serve de comparativo: [renda-fixa.md](../../Docs/Base%20de%20conhecimento/renda-fixa.md).

## Quando usar
- Analisar ou comparar FIIs, Fiagros e FI-Infra.
- Avaliar se o dividendo é sustentável.
- Definir a fatia de fundos na carteira e o equilíbrio entre tijolo e papel.

## Conceitos-chave (fiis-fiagros.md, seções 1 e 4)
- FII é renda variável: a cota oscila todos os dias, mesmo com renda estável. Aluguéis e juros de recebíveis viram rendimentos em geral mensais; a regra exige distribuir ao menos 95% do resultado de caixa a cada semestre (verificar regra vigente).
- Rendimentos são isentos de IR para pessoa física se o fundo e o investidor cumprirem as condições legais; o ganho de capital na venda da cota é tributado (verificar regra vigente).
- Função na carteira: renda e proteção contra inflação, com crescimento de capital limitado.
- Alto dividend yield é prêmio de risco, não oportunidade por si só.
- Selic em alta torna a renda fixa mais atrativa e tende a pressionar as cotas; quedas em bons fundos nesse ciclo podem ser oportunidade se vacância, inquilinos e geração de caixa estão intactos. Fundos de papel pós-fixados em CDI e de papel em IPCA reagem de forma diferente aos juros (seção 4).

## Tipos e riscos (fiis-fiagros.md, seção 2)
| Tipo | Como rende | Riscos principais |
|---|---|---|
| Tijolo: lajes e galpões logísticos | Aluguel | Qualidade e concentração de inquilinos, vacância, localização, oferta nova |
| Tijolo: shoppings | Aluguel mínimo mais percentual sobre vendas | Ciclo econômico; evitar monoativo; eventos como enchentes e incêndios |
| Tijolo: hotéis e imóveis atípicos (hospitais, educação) | Aluguel ou operação | Sensibilidade ao ciclo, inquilino único, dificuldade de relocar |
| Papel (CRI) high grade | Juros de recebíveis (CDI ou IPCA + spread) | Retorno mais modesto, risco de perda menor |
| Papel high yield | Taxas muito altas | Inadimplência, concentração em poucos devedores, dívida subordinada, garantias frágeis |
| Fundo de fundos | Cotas de outros FIIs | Dupla camada de custos; ganho pontual pode inflar o rendimento |
| Desenvolvimento | Construção e venda | Atrasos, custos, venda incerta; inadequado para renda corrente |
| Híbrido | Mistura | Perda de controle sobre o perfil de risco |
| Fiagro | Em geral CRAs do agronegócio | Crédito, execução lenta de garantias, clima e commodities, transparência menor |
| FI-Infra | Debêntures incentivadas de infraestrutura | Distribuição por competência contábil (pagamentos podem ser irregulares), mercado jovem, liquidez menor; rendimentos e ganho de capital isentos conforme a regra vigente |

## Indicadores e referências (fiis-fiagros.md, seção 3)
As faixas são referências, não regras absolutas; tipo de fundo, ciclo de juros e qualidade dos ativos podem justificar exceções.

| Indicador | Fórmula / o que mede | Referência |
|---|---|---|
| P/VP | Preço da cota / valor patrimonial por cota | Abaixo de 1: desconto (se o patrimônio for confiável); em torno de 1: justo; acima de 1: ágio. Muito baixo (por exemplo, abaixo de 0,50) costuma indicar problema grave |
| Dividend yield | Rendimentos 12m / preço da cota | Comparar com a taxa livre de risco e com fundos semelhantes; muito acima do mercado pede investigação |
| FFO / resultado recorrente e FFO yield | Receitas recorrentes menos despesas, sem ganhos pontuais; FFO por cota / preço | O rendimento deve ser coberto pelo resultado recorrente; DY maior que FFO yield indica distribuir mais do que gera |
| Cap rate | Receita líquida anual de aluguel (NOI) / valor do imóvel | Comparar com juros longos e imóveis semelhantes |
| Vacância física | Área vaga / área total | Quanto menor, melhor; persistência alta sinaliza problema. Ciclos de vacância maiores são comuns em lajes |
| Vacância financeira | Receita perdida por vagas e carências / receita potencial | Mostra o efeito real no caixa |
| WALT | Prazo médio ponderado dos contratos | Quanto mais longo, mais previsível; observar cronograma de vencimentos |
| Concentração de inquilinos e ativos | % da receita dos maiores inquilinos; número de imóveis e regiões | Alta concentração aumenta o risco |
| Indexação | % dos contratos corrigidos por IPCA ou IGP-M | Protege o poder de compra do rendimento |
| Inadimplência | Atrasos / receita total | Em tijolo, próxima de zero; em papel, observar carteira vencida e provisões |
| LTV (papel) | Dívida do devedor / valor da garantia | Quanto menor, maior a proteção (por exemplo, abaixo de 50% é mais seguro) |
| Alavancagem do fundo | Dívida / patrimônio líquido | Preferir baixa; verificar custo, prazo e indexador da dívida |
| Taxas | Administração, gestão, consultoria e performance | Até cerca de 1% a.a. em tijolo costuma ser razoável; 2% ou mais corrói o retorno; some todas as taxas |
| Liquidez e spread | Volume diário; diferença entre compra e venda | Quanto maior a liquidez, melhor; em fundos pouco líquidos use ordens limitadas |
| Spread (papel) | Taxa dos CRIs menos referência | Compare com o risco da carteira |

## Procedimento (fiis-fiagros.md, seções 6 e 11)
1. Identificar o tipo do fundo e a tese.
2. Coletar os dados atuais (relatório gerencial mais recente, regulamento, fatos relevantes, B3, sites agregadores de dados) com fonte e data.
3. **Tijolo**: inquilinos e saúde financeira, concentração (monoativo ou monolocatário), vencimentos, tipo de contrato, indexação, vacância física e financeira, localização, gestão ativa ou passiva.
4. **Papel, Fiagro e FI-Infra**: devedores e ratings, high grade ou high yield, concentração por devedor, garantias, LTV, indexador, prazos, inadimplência, provisões, histórico de renegociações.
5. **Preço**: P/VP e DY versus o histórico do fundo e os pares do mesmo tipo.
6. **Sustentabilidade** (seção 7): DY versus FFO yield, composição do resultado (recorrente versus ganho pontual), reservas, política de distribuição.
7. **Alavancagem, custos e liquidez**: dívida, soma das taxas, volume, número de cotistas.
8. **Gestão e governança**: histórico, transparência, emissões anteriores abaixo do valor patrimonial, conflitos de interesse.
9. **Cenário de juros** (seção 4): comportamento em alta e em queda de juros.
10. **Carteira**: peso por tipo e diversificação (ver alocação abaixo).

## Alocação de referência (fiis-fiagros.md, seção 9; montagem-de-carteira.md, seção 2)
Os pesos são ordens de grandeza, não recomendação individual.
- Fatia total de FIIs por perfil: cerca de 10% (conservador) a 15% (moderado e arrojado) do patrimônio, segundo a tabela de montagem-de-carteira.md.
- Dentro da fatia de FIIs: tijolo de alta qualidade como base (maior parte); papel high grade em parcela intermediária; papel high yield, Fiagro e FI-Infra em pequena parcela ou nula, sobretudo para perfis conservadores; fundos de fundos opcionais, observando custos; desenvolvimento mínimo e só para perfis arrojados.
- Diversificar entre segmentos, gestoras, regiões, inquilinos e indexadores; um número moderado de fundos (por exemplo, de oito a quinze em carteiras maiores) equilibra diversificação e acompanhamento.
- FIIs não devem concentrar todo o patrimônio só porque pagam mensalmente.
- Reinvestir os rendimentos acelera a acumulação; direcione ao fundo mais atraente no momento, não ao que pagou (seção 10).

## Filtros de exclusão sugeridos (fiis-fiagros.md, seção 5.2)
Monoativo ou monoinquilino sem justificativa, vacância alta e persistente, localização em decadência, gestão passiva em ativos com problemas, DY recorrentemente acima do FFO yield, P/VP extremamente baixo sem explicação, liquidez muito baixa, taxas altas, concentração em poucos devedores ou dívida subordinada em papel, rendimento dependente de vendas de ativos.

## Sinais de alerta (fiis-fiagros.md, seções 12 e 13)
- Rendimento acima do que o fundo gera, ou sustentado por vendas de imóveis.
- Emissões de cotas frequentes abaixo do valor patrimonial.
- Fundo de papel high yield em ciclo de juros altos com inadimplência e provisões subindo.
- Taxas e estruturas de remuneração elevadas ou complexas.
- Relatórios gerenciais vagos; falta de transparência na carteira de CRIs ou CRAs.
- Esperar de FI-Infra a regularidade de pagamentos de um fundo de tijolo.

## Formato de saída
1. Resumo e veredito (2 a 4 linhas).
2. Tipo, tese e composição do fundo.
3. Tabela de indicadores: valor, referência, leitura.
4. Sustentabilidade do rendimento (DY versus FFO).
5. Riscos específicos e sinais de alerta.
6. Encaixe na carteira (peso e diversificação).
7. Fontes e data dos dados.
