---
description: "Use para guardrails gerais de workflow neste repositorio de planejamento da Plexa, incluindo documentacao, GitHub e consistencia de contexto."
name: "Plexa Planning Workflow Guardrails"
applyTo: "**"
---
# Plexa Planning Workflow Guardrails

## Nivel das regras

- Tratar os itens abaixo como preferencias fortes de engenharia do projeto.
- Pode flexibilizar quando houver bloqueio tecnico real, registrando o motivo na documentacao afetada ou no PR.

## Natureza do repositorio

- Este repositorio e dedicado a planejamento, documentacao, padroes, referencias e instrucoes operacionais.
- Nao versionar codigo de aplicacao neste repositorio, salvo pequenos exemplos documentais quando estritamente necessarios.

## Workflow de documentacao

- Organizar documentos por tema, com nomes claros e foco em rastreabilidade.
- Toda decisao relevante deve indicar contexto, motivacao, impacto e proximos passos.
- Manter `docs/handoff/<nome-da-branch>.md` atualizado e `CONTEXT.md` apontando para o handoff ativo.

## Gestao no GitHub

- Usar GitHub MCP como preferencia para operacoes de issues e PRs.
- Usar `gh` CLI como fallback para operacoes nao suportadas no MCP ou quando houver falha operacional.
- Manter o backlog remoto consistente com o espelho local em `docs/milestones/`.

## Consistencia de planejamento

- Separar claramente arquitetura de plataforma, planejamento de frontend, planejamento de backend e backlog operacional.
- Registrar explicitamente riscos e validacoes pendentes, especialmente quando houver hipoteses como `Python-first` para frontend.
- Evitar detalhamento prematuro de implementacao quando o objetivo ainda for alinhamento de escopo e arquitetura.
