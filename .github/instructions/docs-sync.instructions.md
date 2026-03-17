---
description: "Use quando atualizar contexto de handoff, milestones/issues locais ou documentacao tecnica em docs/. Cobre sincronizacao entre docs, AGENTS.md e CONTEXT.md."
name: "Plexa Docs Sync"
applyTo:
  - "docs/**"
  - "AGENTS.md"
  - "CONTEXT.md"
---
# Plexa Docs Sync

## Objetivo

- Manter rastreabilidade entre decisoes de planejamento, estado operacional e backlog no GitHub.

## Regras de sincronizacao

- Toda mudanca relevante de planejamento deve incluir atualizacao minima em `docs/` quando aplicavel.
- Ao fim de cada ciclo relevante, atualizar `docs/handoff/<nome-da-branch>.md`.
- Manter `CONTEXT.md` apontando corretamente para o handoff ativo da branch.
- Alteracoes de fluxo e guardrails do projeto devem refletir em `AGENTS.md` quando necessario.

## Milestones e issues locais

- Seguir `docs/github-project-management.md` como fonte de verdade para workflow.
- Manter `docs/milestones/` sincronizado com remoto no mesmo ciclo de criacao/atualizacao.
- Cada milestone remota deve ter pasta local com `README.md` contendo `Milestone remota: #<numero>`.
- Cada pasta de milestone deve ter `CHALLENGES.md` com desafios por issue, decisao adotada e encaminhamentos.
- Cada issue da milestone deve ter arquivo local `<numero>-<slug>.md`, inclusive issues fechadas.

## Qualidade da documentacao

- Registrar decisoes tecnicas com contexto, trade-off e impacto.
- Referenciar documentos relacionados quando influenciarem o planejamento de uma capacidade.
- Evitar redundancia; priorizar estado atual, riscos em aberto e proximos passos verificaveis.
