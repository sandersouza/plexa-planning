# Mapa Inicial de Domínios

## Núcleos de negócio

### Clientes

- cadastro e perfil
- consentimentos e preferências
- check-in e presença
- comunicação e relacionamento
- histórico de consultas e procedimentos

### Clínicas

- unidades e configuração operacional
- agenda e capacidade
- profissionais e alocação
- execução de atendimento
- faturamento e indicadores

### Fornecedores

- cadastro e qualificação
- catálogo e negociação
- abastecimento
- integração com compras e estoque

## Capacidades transversais

- CRM
- marketing direcionado
- mensageria e notificações
- estoque
- compras
- financeiro
- contábil
- relatórios
- auditoria

## Dependências iniciais entre domínios

- `Agenda e atendimento` depende de `Clientes` e `Clínicas`
- `Procedimentos e histórico` depende de `Clientes`, `Atendimento` e eventualmente `Estoque`
- `Marketing e comunicação` depende de `CRM`, consentimentos e eventos de jornada
- `Estoque e compras` depende de `Clínicas` e `Fornecedores`
- `Financeiro e contábil` depende de faturamento, estoque, compras e operação clínica

## Sequência sugerida de planejamento

1. Fundação do projeto e governança
2. Arquitetura de plataforma
3. Frontend por canal e persona
4. Backend por domínio e contrato
5. MVP clínico inicial com foco em operação de clínicas
