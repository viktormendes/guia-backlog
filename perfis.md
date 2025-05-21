# Levantamento de Perfis de Usuário

Este documento descreve os perfis de usuários do sistema, suas responsabilidades e permissões de acesso. Os perfis foram definidos com base nos objetivos funcionais e administrativos da plataforma.

---

## 0. Estudante (Sem Login)

**Descrição**: Usuário final do sistema, com acesso ao módulo acadêmico.

**Permissões:**
- Acessar seu próprio dashboard acadêmico
- Visualizar disciplinas, notas e documentos (como declarações e histórico)
- Receber recomendações baseadas em desempenho acadêmico (módulo de IA)

---

## 1. Estudante

**Descrição**: Usuário final do sistema, com acesso ao módulo acadêmico e ao módulo de acessibilidade.

**Permissões:**
- Acessar seu próprio dashboard acadêmico
- Visualizar disciplinas, notas e documentos (como declarações e histórico)
- Solicitar ajuda de acessibilidade presencial ou por videochamada
- Escolher entre ajuda de voluntários ou profissionais do NAPNE
- Receber recomendações baseadas em desempenho acadêmico (módulo de IA)

---

## 2. Administrador Acadêmico

**Descrição**: Responsável pela gestão dos dados acadêmicos no sistema.

**Permissões:**
- Gerenciar cadastro de disciplinas (CRUD)
- Gerenciar cadastro de professores e sua vinculação com disciplinas
- Acompanhar estatísticas de uso da plataforma
- Gerenciar documentos institucionais visíveis aos estudantes

---

## 3. Profissional NAPNE

**Descrição**: Usuário qualificado para oferecer suporte especializado a estudantes com deficiência.

**Permissões:**
- Receber solicitações de ajuda em tempo real
- Atender chamados presenciais ou por videochamada
- Registrar observações e concluir o atendimento
- Visualizar histórico dos atendimentos realizados (caso necessário)

---

## 4. Voluntário NAPNE

**Descrição**: Estudante ou servidor do campus cadastrado como voluntário para auxiliar estudantes com deficiência.

**Permissões:**
- Receber solicitações de ajuda via notificação
- Atender chamados por proximidade ou disponibilidade
- Confirmar e finalizar atendimentos

---

## 5. Administrador NAPNE

**Descrição**: Responsável pela administração do módulo de acessibilidade.

**Permissões:**
- Gerenciar cadastro de voluntários e profissionais do NAPNE
- Definir critérios de triagem para atendimento
- Acompanhar histórico e métricas de atendimento
- Desabilitar usuários inativos no módulo de acessibilidade

---

## Resumo das Permissões por Perfil

| Perfil                  | Dashboard Acadêmico | Gerenciar Disciplinas | Solicitar Ajuda | Atender Ajuda | Gerenciar NAPNE | Visualizar IA |
|------------------------|---------------------|------------------------|------------------|---------------|------------------|----------------|
| Estudante              | Sim                 | Não                    | Sim              | Não           | Não               | Sim            |
| Administrador Acadêmico| Sim (de todos)      | Sim                    | Não              | Não           | Não               | Não            |
| Profissional NAPNE     | Não                 | Não                    | Não              | Sim           | Não               | Não            |
| Voluntário NAPNE       | Não                 | Não                    | Não              | Sim           | Não               | Não            |
| Administrador NAPNE    | Não                 | Não                    | Não              | Não           | Sim               | Não            |
