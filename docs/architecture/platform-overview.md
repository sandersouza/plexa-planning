# Visão Geral da Plataforma Plexa

## Propósito

A plataforma Plexa deve sustentar a operação completa de clínicas de estética, cobrindo relacionamento com clientes, operação clínica, fornecedores, estoque, financeiro e crescimento comercial.

## Ecossistema principal

- `Clientes`: cadastro, check-in, comunicação, histórico, relacionamento e engajamento
- `Clínicas`: operação administrativa, agenda, atendimento, prontuário operacional, estoque, financeiro e indicadores
- `Fornecedores`: catálogo, abastecimento, relacionamento comercial e integração com compras/estoque

## Canais previstos

- `Web administrativo`: operação interna e gestão
- `Portal`: autoatendimento e relacionamento assistido
- `App mobile`: jornada contínua de cliente e experiências operacionais selecionadas

## Domínios iniciais

- CRM e relacionamento
- Cadastro e identidade
- Agenda e atendimento
- Procedimentos e histórico
- Marketing e comunicação
- Estoque e compras
- Financeiro e contábil
- Gestão de clínicas e unidades
- Fornecedores e supply
- Relatórios e indicadores

## Princípios arquiteturais

- arquitetura modular preparada para microserviços
- contratos REST como baseline entre serviços
- separação clara entre domínio, experiência e governança operacional
- documentação antes da implementação para reduzir ambiguidade entre times e repositórios futuros

## Decisões iniciais

- backend prioritariamente em Python com FastAPI
- persistência híbrida com PostgreSQL e MongoDB
- frontend com diretriz `Python-first`, tratada como hipótese a validar por canal

## Riscos a validar cedo

- adequação de frontend em Python para web administrativo e mobile
- fronteiras corretas entre serviços para evitar fragmentação precoce
- distribuição coerente entre PostgreSQL e MongoDB por tipo de dado
- alinhamento entre necessidades clínicas, comerciais e contábeis sem inflar o MVP
