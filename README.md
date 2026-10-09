# AgentInvest

Agente de estudo e análise de investimentos para investidores brasileiros. O projeto reúne orientações para ações, FIIs, Fiagros, ETFs, ativos no exterior e renda fixa; não substitui aconselhamento financeiro personalizado.

## Conteúdo

- Agente Copilot: [agents/agentinvest.agent.md](agents/agentinvest.agent.md)
- Skills: [skills/](skills/)
- Base de conhecimento: [Docs/Base de conhecimento/](Docs/Base%20de%20conhecimento/)
- Manifestos de instalação: [.github/plugin/](.github/plugin/)

## Instalação

Adicione a pasta deste projeto como fonte local no gerenciador de plugins do VS Code Copilot, usando os manifestos em `.github/plugin/`. Mantenha `agents/`, `skills/` e `Docs/` juntos na raiz do projeto. A disponibilidade e o nome do comando de instalação dependem da versão do Copilot instalada.

Após instalar, invoque o agente **AgentInvest** e informe o ativo ou a dúvida. Para triagens no Oceans14, o fluxo é assistido: o usuário aplica os filtros no site e compartilha o resultado para análise.

## Uso responsável

As análises dependem de dados atuais e fontes verificáveis. O agente não deve inventar indicadores, prometer retornos nem executar operações em corretoras. Confira regras tributárias e regulatórias vigentes.