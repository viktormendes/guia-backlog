# 📦 Product Backlog

## Épico 1: Navegação Indoor com AR e Narração para Deficientes Visuais

### US1.1 - Receber instruções por áudio para se orientar dentro da faculdade
**Funcionalidades:**
- Início rápido da rota até um destino (ex: “Biblioteca”)
- Narração por voz com instruções passo a passo
- Integração com TTS (Text-to-Speech)

### US1.2 - Mapear ambientes internos para permitir navegação precisa
**Funcionalidades:**
- Interface para cadastro de salas, corredores, elevadores etc.
- Definição de obstáculos fixos e móveis
- Sincronização de mapas com dispositivos móveis

### US1.3 - Receber alertas de obstáculos no caminho
**Funcionalidades:**
- Alertas por voz e vibração
- Atualização em tempo real de obstáculos temporários

## Épico 2: Videochamada para Suporte em Tarefas

### US2.1 - Iniciar chamada de vídeo para pedir ajuda
**Funcionalidades:**
- Botão “Pedir Ajuda” com acesso rápido
- Digitação por voz ou seleção de tarefa
- Início de chamada com câmera traseira ativa

### US2.2 - Voluntário recebe chamada e pode aceitar ou recusar
**Funcionalidades:**
- Notificações push para novas chamadas
- Visualização do local e descrição da ajuda
- Botões de aceitar/recusar

### US2.3 - Administrador gerencia e visualiza histórico de chamadas
**Funcionalidades:**
- Registro de data/hora, duração e envolvidos
- Exportação em CSV/PDF
- Painel com estatísticas de uso

## Épico 3: Sistema de Chamados

### US3.1 - Solicitar ajuda de voluntários próximos
**Funcionalidades:**
- Formulário simples para envio de chamado
- Geolocalização automática
- Verificação de perímetro da faculdade

### US3.2 - Voluntário visualiza chamados próximos e escolhe qual atender
**Funcionalidades:**
- Lista com distância e tempo estimado
- Botão “Aceitar chamado”
- Visualização de rota

### US3.3 - Voluntário atualiza status do chamado
**Funcionalidades:**
- Botões “A Caminho”, “Cheguei”, “Atendimento Concluído”
- Registro de tempo de resposta
- Avaliação do atendimento pelo usuário

### US3.4 - Administrador acompanha históricos e métricas
**Funcionalidades:**
- Filtros por voluntário, data, tipo
- Mapa de calor dos chamados
- Exportação de relatórios

## Épico 4: Sistema Administrativo Acadêmico (CRUD)

### US4.1 - Gerenciar disciplinas
**Funcionalidades:**
- Cadastro com nome, código, pré-requisitos, carga horária
- Associação com professores e horários
- Ativação/desativação de disciplinas

### US4.2 - Gerenciar salas
**Funcionalidades:**
- Cadastro com nome, bloco, capacidade e recursos
- Horários de disponibilidade
- Localização no mapa

### US4.3 - Gerenciar professores
**Funcionalidades:**
- Cadastro com nome, matrícula, área de atuação
- Disciplinas associadas
- Disponibilidade de horários

### US4.4 - Gerenciar blocos da faculdade
**Funcionalidades:**
- Cadastro com nome e localização
- Listagem das salas
- Informações de acessibilidade

### US4.5 - Gerenciar horários
**Funcionalidades:**
- Tabela com dias e turnos
- Validação de conflitos entre professor, sala e disciplina

## Épico 5: Acompanhamento de Progresso Acadêmico

### US5.1 - Registrar disciplinas cursadas
**Funcionalidades:**
- Lista com status: cursada, em andamento, pendente
- Validação de pré-requisitos completados

### US5.2 - Simular próximo semestre
**Funcionalidades:**
- Escolha de disciplinas com validação de conflitos
- Sugestões baseadas no histórico
- Visualização do plano semestral

### US5.3 - Estimar data de formatura
**Funcionalidades:**
- Cálculo da carga horária restante
- Projeção dos próximos semestres
- Aviso de riscos (atrasos, pendências)

### US5.4 - Administrador visualiza relatórios de progresso
**Funcionalidades:**
- Percentual de conclusão por aluno
- Tempo médio até formatura
- Alunos em risco de atraso

## Épico 6: Autenticação e Acessibilidade

### US6.1 - Fazer login com e-mail ou conta institucional
**Funcionalidades:**
- Login por e-mail/senha
- Login com Google
- Recuperação de senha

### US6.2 - Acessar sistema com leitor de tela e comandos por voz
**Funcionalidades:**
- Compatibilidade com leitores (VoiceOver, TalkBack)
- Botões com contraste alto e acessibilidade
- Comandos básicos por voz
