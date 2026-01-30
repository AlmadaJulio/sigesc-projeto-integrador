# Documento de Requisitos — SIGESC

## 1. Visão Geral
O SIGESC é uma plataforma digital para integrar cidadãos e prestadores de serviços, permitindo solicitar, acompanhar e concluir atendimentos comunitários, com foco em impacto social, segurança e acessibilidade.

## 2. Perfis de Usuário
- Cidadão: solicita e acompanha serviços
- Prestador: aceita e executa atendimentos
- Administrador/Gestor: acompanha indicadores e gerencia cadastros

## 3. Requisitos Funcionais (RF)

**RF01 — Cadastro de usuário**
- O sistema deve permitir cadastro com nome, e-mail e senha.
- Critério de aceite: usuário cadastrado consegue autenticar.

**RF02 — Login**
- O sistema deve permitir login por e-mail e senha.
- Critério de aceite: usuário autenticado acessa área logada.

**RF03 — Solicitar serviço**
- O cidadão deve registrar uma solicitação com categoria, descrição e localização (texto).
- Critério de aceite: solicitação fica com status “Aberta”.

**RF04 — Listar solicitações**
- O prestador deve visualizar solicitações abertas.
- Critério de aceite: lista exibe apenas solicitações com status “Aberta”.

**RF05 — Aceitar atendimento**
- O prestador deve aceitar uma solicitação.
- Critério de aceite: status muda para “Em andamento” e fica vinculado ao prestador.

**RF06 — Concluir atendimento**
- O prestador deve concluir o atendimento.
- Critério de aceite: status muda para “Concluído”.

**RF07 — Avaliar atendimento**
- O cidadão deve avaliar um atendimento concluído (nota e comentário).
- Critério de aceite: avaliação fica vinculada ao atendimento.

## 4. Requisitos Não Funcionais (RNF)

**RNF01 — Segurança e LGPD**
- Dados sensíveis devem ser protegidos e acessos controlados por perfil.

**RNF02 — Usabilidade e acessibilidade**
- Interface simples, com linguagem clara e navegação intuitiva.

**RNF03 — Desempenho**
- Operações principais devem responder em até 3 segundos em condições normais.

**RNF04 — Auditabilidade**
- Registrar eventos básicos (criação/aceite/conclusão) para rastreabilidade.

## 5. Restrições e premissas
- Ferramentas gratuitas
- Projeto consistente com o documento acadêmico (Univille)
- MVP prioriza web + API (mobile fica opcional)
