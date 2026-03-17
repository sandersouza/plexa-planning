---
description: "Use para diretrizes base de arquitetura da plataforma Plexa, incluindo dominios, canais, integracoes e principios de modularidade."
name: "Plexa Platform Architecture"
applyTo:
  - "docs/**"
  - "AGENTS.md"
  - "CONTEXT.md"
---
# Plexa Platform Architecture

## Objetivo

- Garantir consistencia entre a arquitetura de negocio, os canais de experiencia e a estrategia de plataforma.

## Diretrizes de arquitetura

- Tratar a plataforma como um ecossistema integrado para `Clientes`, `Clinicas` e `Fornecedores`.
- Priorizar arquitetura modular, orientada a dominios e preparada para evolucao por microservicos.
- Separar claramente responsabilidades de frontend, backend, integracoes e dados, mesmo quando o planejamento estiver em um unico repositorio.
- Documentar dependencias entre modulos e contratos esperados entre dominios antes de detalhar implementacao.

## Stack-alvo inicial

- Backend prioritariamente em Python com FastAPI.
- Frontend com diretriz `Python-first`, a ser validada por viabilidade tecnica por canal.
- Persistencia combinando PostgreSQL e MongoDB conforme natureza dos dados.
- APIs internas e externas orientadas a REST como baseline.

## Canais e superficies

- Considerar, no minimo, `web administrativo`, `portal` e `app mobile` no planejamento inicial.
- Mapear experiencias por persona e por canal antes de detalhar telas, componentes ou fluxos tecnicos.
- Explicitar quando uma capacidade pertence a um unico canal ou precisa ser compartilhada entre multiplos.

## Qualidade de planejamento

- Registrar contexto, trade-offs, riscos e criterios de validacao para decisoes arquiteturais.
- Evitar assumir detalhes irreversiveis de implementacao sem justificativa tecnica.
- Preferir artefatos curtos, rastreaveis e versionados por tema.
