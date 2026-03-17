# Handoff da Branch `main`

## Estado atual

- Repositório reposicionado como base oficial de planejamento da plataforma Plexa.
- Instruções herdadas de outro projeto foram substituídas por guardrails alinhados a planejamento, gestão no GitHub e arquitetura da plataforma.
- Documentação base de gestão, arquitetura, frontend e backend foi criada.
- Backlog remoto inicial foi criado no GitHub com milestones, labels e issues para os próximos ciclos.
- O espelho local de milestones e issues foi inicializado em `docs/milestones/`.

## Documentos de referência

- `docs/github-project-management.md`
- `docs/architecture/platform-overview.md`
- `docs/planning/domain-map.md`
- `docs/planning/frontend-planning.md`
- `docs/planning/backend-planning.md`

## Próximos passos

- configurar o GitHub Project board inicial
- evoluir o recorte do MVP clínico a partir do mapa de domínios
- aprofundar a validação da hipótese `Python-first` para frontend
- detalhar convenções REST e scaffold FastAPI de referência

## Riscos e pontos em aberto

- falta estruturar o board/projeto remoto
- o CLI do GitHub está autenticado sem os escopos `project` e `read:project`, bloqueando a criação imediata do board remoto
- a diretriz de frontend em Python ainda depende de validação por canal
