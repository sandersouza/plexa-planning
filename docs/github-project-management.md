# GitHub Project Management

Fonte de verdade do fluxo operacional deste repositório de planejamento.

## Objetivo

Organizar o planejamento da plataforma Plexa no GitHub com rastreabilidade entre backlog remoto e espelho local em `docs/milestones/`.

## Ferramentas

- Preferência: GitHub MCP para issues, PRs e operações suportadas.
- Fallback: `gh` CLI para milestones, projetos e operações não suportadas pelo MCP.

## Estrutura de backlog

O backlog inicial deve ser organizado em milestones que representem grandes blocos de planejamento:

1. Fundação do projeto
2. Arquitetura de plataforma
3. Planejamento do frontend
4. Planejamento do backend
5. Planejamento do MVP clínico

Cada milestone agrupa issues executáveis, com granularidade suficiente para ser concluída em ciclos curtos.

## Convenções de issues

Cada issue deve:
- ter título objetivo com verbo de ação
- pertencer a uma milestone quando fizer parte de um bloco planejado
- carregar labels de `tipo`, `área` e `prioridade` quando disponíveis
- ter descrição com contexto, resultado esperado, entregáveis e critérios de aceite

Sugestão de famílias de labels:
- `type:epic`
- `type:planning`
- `type:docs`
- `area:platform`
- `area:frontend`
- `area:backend`
- `area:project-management`
- `priority:p0`
- `priority:p1`
- `priority:p2`

## Fluxo de status

Fluxo padrão do board:

`Ready -> In progress -> In review -> Done`

Regras:
- itens novos entram em `Ready`
- ao iniciar trabalho ativo, mover para `In progress`
- ao consolidar material para revisão, mover para `In review`
- ao concluir e sincronizar documentação, mover para `Done`
- se houver retrabalho, retornar para `In progress`

## Branches e PRs

Para este repositório:
- a `main` mantém a base documental estável
- branches de trabalho devem ser vinculadas a uma issue quando o backlog já estiver estruturado
- branches de release devem seguir `release/<versao>`

Para repositórios futuros de implementação:
- cada branch deve nascer de uma issue ou bloco formal do backlog
- PR deve referenciar a issue correspondente
- labels do PR devem refletir o mesmo recorte semântico da issue

## Espelho local em `docs/milestones/`

Cada milestone remota deve ter uma pasta local.

Estrutura mínima:

```text
docs/milestones/<slug-da-milestone>/
  README.md
  CHALLENGES.md
  <numero>-<slug-da-issue>.md
```

Regras:
- `README.md` deve conter `Milestone remota: #<numero>`
- `CHALLENGES.md` registra desafios, decisões e encaminhamentos
- cada issue deve existir localmente, inclusive quando fechada

## Cadência de sincronização

Sincronizar no mesmo ciclo em que houver:
- criação de milestone
- criação ou atualização relevante de issue
- conclusão de bloco de planejamento
- decisão que afete arquitetura, escopo ou priorização

## Board inicial recomendado

Colunas:
- `Ready`
- `In progress`
- `In review`
- `Done`

Automação desejada:
- item criado entra em `Ready`
- issue fechada ou PR mergeado pode ir para `Done` após conferência documental

## Critérios de boa gestão

- backlog remoto e espelho local contam a mesma história
- contexto ativo da branch está atualizado
- milestones representam blocos de valor claros
- issues são pequenas o bastante para execução rastreável
- decisões arquiteturais relevantes aparecem também nos documentos temáticos
