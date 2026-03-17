---
description: "Use para regras de gestao de issues, milestones, branches, PRs e sincronizacao do espelho local em docs/milestones."
name: "Plexa Project Management"
applyTo:
  - "docs/github-project-management.md"
  - "docs/milestones/**"
  - "AGENTS.md"
  - "CONTEXT.md"
  - "docs/handoff/**"
---
# Plexa Project Management

## Objetivo

- Manter fluxo previsivel de planejamento entre backlog remoto no GitHub e espelho documental local.

## Fonte de verdade

- Seguir `docs/github-project-management.md` como referencia principal de processo.
- Este arquivo define guardrails compactos; detalhes operacionais ficam no documento de gestao.

## Ferramentas GitHub

- Preferir **GitHub MCP** para operacoes de gestao sempre que estiver disponivel e funcional.
- Usar **`gh` CLI apenas como fallback** quando MCP estiver indisponivel, sem suporte ou com erro de permissao/autenticacao.

## Branches

- A branch `main` concentra a fundacao documental e a referencia mais atual do planejamento.
- Branches futuras de trabalho devem ser vinculadas a issue de origem.
- Branches de release devem seguir o padrao `release/<versao>`.
- Nunca reescrever historico da `main`.
- Antes de remover branch local, confirmar com o usuario.

## Ciclo de issue e board

- Atualizar status do item no projeto: `Ready` -> `In progress` -> `In review` -> `Done`.
- Se uma atividade voltar a exigir refinamento, retornar o item para `In progress`.
- Ao concluir uma issue, sincronizar o espelho local no mesmo ciclo.

## PRs

- Ao concluir um bloco estavel de trabalho, abrir PR para `main`.
- Enviar o link do PR para aprovacao/review antes de seguir para o proximo bloco relevante.
- Garantir labels coerentes entre issue e PR.

## Espelho local de milestones e issues

- Manter `docs/milestones/` sincronizado com o backlog remoto.
- Cada milestone remota deve ter pasta local com `README.md` e campo `Milestone remota: #<numero>`.
- Cada pasta de milestone deve conter `CHALLENGES.md` com desafios, decisoes e encaminhamentos por issue.
- Cada issue da milestone deve ter arquivo `<numero>-<slug>.md`, inclusive fechadas, para historico.
