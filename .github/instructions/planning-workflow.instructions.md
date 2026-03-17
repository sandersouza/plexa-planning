---
description: "Use para guardrails gerais de workflow no repositório de planejamento da Plexa, incluindo documentação, GitHub, contexto e organização do backlog."
name: "Plexa Planning Workflow Guardrails"
applyTo: "**"
---
# Plexa Planning Workflow Guardrails

## Objetivo

- Garantir consistência operacional neste repositório de planejamento, mantendo documentação, backlog remoto e contexto local sincronizados.

## Natureza do repositório

- Este repositório é dedicado a planejamento, documentação, padrões, referências, modelos e instruções operacionais da Plexa.
- Não versionar código de aplicação neste repositório, salvo exemplos documentais pequenos e claramente identificados.
- Tratar `docs/` como área principal de trabalho e este repositório como base de coordenação para futuros repositórios de implementação.

## Workflow de documentação

- Organizar documentos por tema, com nomes claros e foco em rastreabilidade.
- Toda decisão relevante deve registrar contexto, motivação, impacto, riscos e próximos passos verificáveis.
- Atualizar `docs/handoff/<nome-da-branch>.md` ao final de cada ciclo relevante.
- Manter `CONTEXT.md` apontando para o handoff ativo da branch.

## Gestão no GitHub

- Usar GitHub MCP como preferência para operações de issues, PRs e demais itens de gestão suportados.
- Usar `gh` CLI como fallback quando MCP não suportar a operação ou estiver indisponível.
- Manter o backlog remoto coerente com o espelho local em `docs/milestones/`.
- Sempre que criar ou atualizar milestone/issue de forma relevante, refletir a mudança no espelho local no mesmo ciclo.

## Consistência de planejamento

- Separar claramente arquitetura de plataforma, planejamento de frontend, planejamento de backend, MVP e gestão operacional.
- Registrar hipóteses e validações pendentes explicitamente, principalmente quando houver decisões ainda abertas, como a estratégia `Python-first` para frontend.
- Evitar detalhamento prematuro de implementação quando o objetivo ainda for alinhamento de escopo, domínio ou arquitetura.
- Preferir artefatos curtos, conectados entre si e fáceis de transformar em backlog executável.

## Qualidade do backlog

- Issues devem nascer com contexto, resultado esperado, entregáveis e critérios de aceite.
- Milestones devem representar blocos claros de planejamento ou valor.
- O espelho local em `docs/milestones/` deve permanecer utilizável como histórico e ponto de consulta rápida.
