# Planejamento Inicial de Frontend

## Objetivo

Definir a visão de experiências, canais, personas e módulos de frontend da plataforma Plexa antes de qualquer implementação.

## Estratégia inicial

- tratar `Python-first` como diretriz de investigação e não como decisão irrevogável
- avaliar a estratégia por canal, e não de forma genérica
- separar claramente experiência administrativa, autoatendimento e mobile

## Canais

### Web administrativo

Foco:
- operação da clínica
- CRM operacional
- agenda, procedimentos, estoque e financeiro

### Portal

Foco:
- acesso assistido do cliente
- consulta de dados, histórico e comunicação
- interações com clínicas e jornadas específicas

### App mobile

Foco:
- cadastro, check-in e relacionamento contínuo
- lembretes, comunicação e campanhas direcionadas
- acompanhamento de consultas e histórico

## Personas iniciais

- cliente final
- recepção/atendimento
- gestão da clínica
- profissional da clínica
- operador administrativo/financeiro
- fornecedor/parceiro

## Superfícies e experiências prioritárias

- onboarding e cadastro
- autenticação e perfil
- agenda e confirmação
- histórico e relacionamento
- campanhas e comunicação
- visão operacional de atendimento
- estoque e compras
- visão financeira operacional

## Backlog inicial por frente

### Frontend foundation

- definir critérios de viabilidade de `Python-first`
- mapear canais por persona
- documentar jornadas principais
- definir módulos por canal

### Frontend web administrativo

- mapear navegação operacional macro
- identificar módulos comuns entre clínica, estoque, CRM e financeiro
- definir necessidades de responsividade e perfis de acesso

### Frontend portal e mobile

- mapear jornadas de cliente ponta a ponta
- definir quais fluxos serão compartilhados e quais serão exclusivos de mobile
- listar eventos de jornada que dependerão do backend e da comunicação

## Critérios para validar `Python-first`

- produtividade para equipe e velocidade de scaffold
- aderência ao canal web administrativo
- viabilidade real para mobile e experiência do usuário
- compatibilidade com autenticação, estados de interface e integrações planejadas
- custo de manutenção e risco de lock-in tecnológico

## Entregáveis esperados deste bloco

- matriz canal x persona
- catálogo inicial de superfícies
- jornadas principais
- backlog de módulos
- parecer documentado sobre viabilidade de frontend em Python por canal
