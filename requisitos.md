# Documento de Requisitos

## 1. Visão Geral

O sistema visa oferecer uma plataforma unificada de gestão acadêmica e de acessibilidade (NAPNE) para estudantes, professores e administradores de um instituto federal. Ele terá uma interface web para os módulos administrativos e uma aplicação mobile (React Native) para o suporte aos estudantes com deficiência.

---

## 2. Escopo

### 2.1 Módulo Acadêmico

Gerenciamento de:
- Disciplinas
- Professores
- Horários
- Salas
- Blocos
- Pré-requisitos

### 2.2 Módulo NAPNE

Atendimento de acessibilidade para estudantes com deficiência:
- Solicitações por chat
- Solicitações por videochamada
- Solicitações de ajuda presencial via geolocalização

---

## 3. Perfis de Usuário

| Perfil                | Descrição                                                                 |
|----------------------|---------------------------------------------------------------------------|
| Estudante            | Usuário final. Acessa o sistema acadêmico e solicita suporte do NAPNE.    |
| Administrador Acadêmico | Gera e gerencia disciplinas, professores, horários, blocos e salas.     |
| Profissional NAPNE   | Atende solicitações dos estudantes com deficiência.                       |
| Voluntário NAPNE     | Atende solicitações como apoio informal.                                  |
| Administrador NAPNE  | Gerencia equipe, voluntários, critérios e dados estatísticos.             |

---

## 4. Requisitos Funcionais

### 4.1 Requisitos do Módulo Acadêmico

- RF01 – Cadastrar disciplinas com nome, código, carga horária, semestre e tipo.
- RF02 – Cadastrar professores com nome e link do currículo Lattes.
- RF03 – Associar disciplinas a horários, professores e salas.
- RF04 – Cadastrar blocos e suas salas, indicando andares e capacidade.
- RF05 – Cadastrar pré-requisitos entre disciplinas.
- RF06 – Gerar grade horária por semestre.
- RF07 – Permitir ao estudante visualizar suas disciplinas, horários e desempenho.
- RF08 – Permitir ao professor visualizar suas turmas e desempenho dos alunos.
- RF09 – Validar a consistência de pré-requisitos na matrícula.

### 4.2 Requisitos do Módulo NAPNE

- RF10 – Permitir que estudantes solicitem ajuda de três tipos: chat, videochamada e presencial.
- RF11 – Encaminhar solicitações para voluntários e profissionais por ordem de prioridade.
- RF12 – Permitir que voluntários/profissionais aceitem ou recusem chamadas.
- RF13 – Registrar o histórico dos atendimentos realizados.
- RF14 – Suporte a geolocalização para ajuda presencial.
- RF15 – Enviar notificações push com Firebase para novas solicitações.
- RF16 – Exibir status em tempo real da solicitação (pendente, aceita, finalizada).
- RF17 – Permitir videochamadas integradas via WebRTC ou similar.
- RF18 – Exibir lista de atendentes disponíveis por tipo de ajuda.
- RF19 – Permitir que o administrador do NAPNE adicione ou remova usuários da equipe.
- RF20 – Permitir que o administrador defina critérios de priorização.

---

## 5. Requisitos Não Funcionais

- RNF01 – O sistema deve funcionar em ambiente web (módulo administrativo) e mobile (NAPNE).
- RNF02 – A aplicação mobile deve ser desenvolvida com React Native.
- RNF03 – A comunicação push deve ser feita via Firebase Cloud Messaging.
- RNF04 – A interface deve ser acessível, responsiva e compatível com WCAG 2.1 AA.
- RNF05 – O sistema deve garantir o tempo de resposta rápido.
- RNF06 – O sistema deve registrar logs de ações sensíveis (atendimentos, edições de disciplina).
- RNF07 – O sistema deve utilizar banco de dados relacional (PostgreSQL).

---

## 6. Casos de Uso

### UC01 – Cadastrar Disciplina
**Atores**: Administrador Acadêmico  
**Descrição**: Cria uma nova disciplina com seus atributos e código.  

### UC02 – Solicitar Ajuda via NAPNE
**Atores**: Estudante  
**Descrição**: O estudante solicita ajuda escolhendo o tipo de atendimento.  
**Fluxo principal**:
1. Estudante seleciona tipo de ajuda
2. Sistema envia notificação via Firebase
3. Atendente aceita
4. Sessão (chat, vídeo ou presencial) é iniciada
5. Atendente encerra e registra atendimento

### UC03 – Atender Solicitação
**Atores**: Voluntário, Profissional NAPNE  
**Descrição**: Aceita uma solicitação e realiza o atendimento correspondente.  

### UC04 – Gerenciar Salas e Blocos
**Atores**: Administrador Acadêmico  
**Descrição**: Cadastra salas em blocos, define capacidade e número de andares.  

---

## 7. Tecnologias Previstas

| Componente           | Tecnologia                |
|----------------------|---------------------------|
| Backend              | Node.js + NestJS          |
| Banco de Dados       | PostgreSQL                |
| Frontend(Web)        | Next.Js                   |
| Mobile               | React Native              |
| Push Notifications   | Firebase Cloud Messaging  |
| Videochamada         | WebRTC / Jitsi / Agora    |
| Autenticação         | OAuth2 / JWT              |

---

## 8. Observações Finais

- A lógica de seleção de voluntários deve evitar sobrecarga dos mesmos usuários.
- O módulo NAPNE será projetado pensando em UX de acessibilidade.

