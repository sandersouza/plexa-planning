# AGENTS
## Objetivo do projeto
Planejamento central dos projetos da Plexa Group.

Este repositório existe para concentrar documentação, padrões, referências, modelos, instruções operacionais e backlog de planejamento da plataforma.

## Fonte canônica de regras de fluxo
As regras operacionais estão centralizadas em `.github/instructions/`.
Regra única: sempre carregar e aplicar **todos** os arquivos `*.instructions.md` dessa pasta.

Prioridade interna:
- Novas regras devem ser adicionadas dentro de seus arquivos de contexto.
- Regras que impactam o fluxo geral do projeto devem ser adicionadas em `docs-sync.instructions.md`.
- Regras que impactam a organização do trabalho e o ciclo de desenvolvimento devem ser adicionadas em `project-management.instructions.md`.
- Regras que impactam arquitetura e organização da plataforma devem ser adicionadas em `platform-architecture.instructions.md`.
- Caso o arquivo de instruções específico ainda não exista, crie um novo arquivo.
- Regras marcadas como imutáveis/obrigatórias têm precedência máxima.
- Regras de preferência podem ser flexibilizadas apenas com justificativa técnica registrada.

## Referências rápidas
- Contexto persistente da branch: `docs/handoff/<nome-da-branch>.md`
- Ponteiro de contexto atual: `CONTEXT.md`
- Fonte de verdade de gestão: `docs/github-project-management.md`
- Espelho local do backlog: `docs/milestones/`
