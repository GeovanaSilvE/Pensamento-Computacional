# 🏗️ Design do Projeto — MedSync

## 📚 Visão Geral

O MedSync foi projetado para representar uma solução digital inteligente voltada para gerenciamento hospitalar em larga escala.

O sistema busca automatizar processos médicos e administrativos através da centralização de informações, organização de consultas e gerenciamento digital de prontuários.

A estrutura do projeto foi construída utilizando conceitos de Pensamento Computacional e Abstração Computacional apresentados em aula. :contentReference[oaicite:0]{index=0}

---

## 🎯 Problema Identificado

Hospitais e clínicas enfrentam dificuldades relacionadas a:
- excesso de processos manuais;
- perda de informações;
- desorganização de prontuários;
- dificuldade no controle de consultas;
- grande volume de dados médicos;
- demora em atendimentos.

O MedSync foi desenvolvido para solucionar esses problemas através da automação e organização digital.

---

## 🧩 Decomposição do Sistema

Para facilitar o desenvolvimento da solução, o sistema foi dividido em módulos independentes.

### Módulo de Usuários
Responsável por:
- login;
- autenticação;
- cadastro de pacientes;
- cadastro de médicos;
- permissões de acesso.



### Módulo de Consultas
Responsável por:
- agendamento;
- remarcação;
- cancelamento;
- verificação de horários disponíveis.



### Módulo Médico
Responsável por:
- prontuários digitais;
- prescrições;
- exames;
- histórico clínico.



### Módulo Inteligente
Responsável por:
- chatbot;
- notificações automáticas;
- suporte virtual.



### Módulo Administrativo
Responsável por:
- relatórios;
- estatísticas;
- indicadores hospitalares;
- controle de atendimentos.

---

## 🔁 Reconhecimento de Padrões

Foi identificado que hospitais possuem processos repetitivos e padronizados:
- cadastro de pacientes;
- realização de consultas;
- armazenamento de exames;
- atualização de prontuários;
- geração de relatórios.

Esses padrões permitiram estruturar o sistema de forma organizada e reutilizável.

---

## 🎯 Abstração Aplicada

Durante o desenvolvimento do projeto, detalhes desnecessários foram removidos para focar apenas nos processos essenciais.

### Detalhes ignorados
- marca dos computadores;
- sistema operacional;
- modelo dos dispositivos;
- estrutura física do hospital.

### Foco principal
- fluxo de atendimento;
- gerenciamento de dados;
- organização das consultas;
- armazenamento de informações médicas.

---

## 🧠 Generalização da Solução

O MedSync foi projetado para funcionar em diferentes ambientes da área da saúde:

- hospitais;
- clínicas;
- laboratórios;
- consultórios;
- unidades de atendimento.

A solução pode ser adaptada para diferentes necessidades organizacionais.

---

## 📊 Níveis de Abstração Utilizados

### Nível 1 — Descrição Detalhada
Representação completa das ações realizadas pelos usuários do sistema.

Exemplo:
- login;
- seleção de pacientes;
- agendamento;
- cadastro de exames;
- geração de relatórios.



### Nível 2 — Representação Intermediária
Representação simplificada através de fluxogramas contendo apenas as principais etapas do sistema.



### Nível 3 — Abstração Computacional
Representação lógica do funcionamento do sistema através de pseudocódigo.

---

## 🔄 Fluxo Lógico do Sistema

```txt id="4c6u6q"
Início
   ↓
Login
   ↓
Selecionar Paciente
   ↓
Agendar Consulta
   ↓
Registrar Informações Médicas
   ↓
Gerar Relatórios
   ↓
Fim
