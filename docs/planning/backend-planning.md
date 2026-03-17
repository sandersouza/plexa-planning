# Planejamento Inicial de Backend

## Objetivo

Definir a espinha dorsal do backend da plataforma Plexa, organizada por domínios, contratos e padrões de implementação futuros.

## Estratégia de arquitetura

- backend prioritariamente em Python
- FastAPI como framework base
- modularidade preparada para microserviços
- contratos REST como baseline

## Bounded contexts iniciais

- identidade e acesso
- clientes e CRM
- clínicas e unidades
- agenda e atendimento
- procedimentos e histórico
- marketing e comunicação
- fornecedores
- estoque e compras
- financeiro e contábil
- relatórios e indicadores

## Proposta inicial de agrupamento em serviços

- `identity-service`
- `crm-service`
- `clinic-operations-service`
- `procedure-history-service`
- `marketing-service`
- `inventory-supply-service`
- `finance-service`
- `reporting-service`

O agrupamento acima é inicial e deve ser refinado para evitar granularidade prematura.

## Estratégia de dados

### PostgreSQL

Usar prioritariamente para:
- cadastros estruturados
- agenda
- relacionamentos transacionais
- financeiro
- estoque
- compras

### MongoDB

Usar prioritariamente para:
- documentos flexíveis
- histórico agregado
- trilhas de comunicação
- snapshots operacionais quando fizer sentido

## Convenções iniciais de API REST

- versionamento explícito na rota
- contratos orientados a recursos de negócio
- separação entre APIs internas e externas quando necessário
- payloads e erros documentados por domínio
- eventos de integração catalogados mesmo quando a entrega inicial for síncrona

## Scaffold-alvo para repositórios futuros

- estrutura por domínio e aplicação
- camadas mínimas de API, serviço, domínio e persistência
- configuração padronizada para FastAPI
- testes organizados por nível
- observabilidade, config e autenticação previstos desde a fundação

## Catálogo inicial de contratos esperados entre domínios

- identidade fornece autenticação e contexto de acesso
- clientes/CRM fornece perfil, relacionamento e preferências
- clínicas e agenda expõem disponibilidade, agendamentos e contexto operacional
- procedimentos e histórico consomem cliente, atendimento e insumos
- estoque e compras interagem com fornecedores e operação clínica
- financeiro consolida eventos operacionais e transações relevantes

## Entregáveis esperados deste bloco

- mapa de bounded contexts
- proposta de serviços iniciais
- diretrizes de dados
- convenções REST
- scaffold-alvo documentado para FastAPI
