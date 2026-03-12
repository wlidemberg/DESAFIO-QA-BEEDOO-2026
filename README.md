# DESAFIO-QA-BEEDOO-2026

## 1. Introdução

Este repositório contém a análise, modelagem de testes e execução de testes realizada como parte do desafio técnico de QA da Beedoo.

A aplicação analisada disponibiliza um módulo para **cadastro e listagem de cursos**, permitindo ao usuário criar novos cursos e visualizar os cursos cadastrados.

Aplicação analisada:

https://creative-sherbet-a51eac.netlify.app/

---

# 2. Objetivo da Aplicação

A aplicação parece ser um sistema simples de **gerenciamento de cursos**, cujo objetivo é permitir que usuários:

- Cadastrem novos cursos
- Visualizem cursos cadastrados
- Excluam cursos existentes

Este tipo de funcionalidade é comum em plataformas de **gestão de treinamentos ou cursos online**.

---

# 3. Principais Fluxos da Aplicação

Durante a análise exploratória foram identificados os seguintes fluxos principais:

### Fluxo 1 — Cadastro de curso

1. Usuário acessa o formulário de cadastro
2. Preenche os campos do curso
3. Clica no botão de cadastro
4. O curso é salvo
5. O curso aparece na listagem

---

### Fluxo 2 — Listagem de cursos

1. Usuário acessa a página
2. O sistema exibe a lista de cursos cadastrados
3. Cada curso apresenta informações cadastradas

---

### Fluxo 3 — Exclusão de curso

1. Usuário localiza um curso na lista
2. Usuário clica no botão excluir
3. O sistema remove o curso da lista

---

# 4. Pontos Críticos do Sistema

Durante a análise foram identificadas áreas que exigem maior atenção durante os testes.

### 1️ Validação de Formulário

O formulário de cadastro é responsável pela integridade dos dados cadastrados.

Campos analisados:

- Nome do curso
- Descrição
- Data de início
- Data de fim
- Quantidade de vagas
- Imagem

Problemas de validação podem causar:

- Dados inválidos
- Informações incompletas
- Inconsistência no sistema

---

### 2️ Persistência dos dados

Após o cadastro, o curso deve aparecer corretamente na listagem.

Riscos:

- Cadastro não persistido
- Dados inconsistentes

---

### 3️ Exclusão de cursos

A exclusão deve remover o curso da listagem.

Riscos:

- Exclusão falsa
- Falha na atualização da interface

---

### 4️ Segurança de entrada de dados

Todos os campos de entrada foram testados contra:

- **XSS (Cross-Site Scripting)**
- **Injeção de HTML**

Esses testes são importantes pois campos sem sanitização podem permitir execução de código malicioso.

SQL Injection **não foi testado**, pois a aplicação não demonstra possuir integração com banco de dados ou backend que execute consultas SQL.

---

# 5. Estratégia de Testes

A estratégia utilizada foi baseada em:

### Exploratory Testing

Primeiramente foi realizada uma exploração da aplicação para compreender:

- funcionalidades disponíveis
- fluxos do sistema
- comportamento da interface

---

### Test Design

Após a exploração foram criados:

- cenários de teste
- casos de teste detalhados

Considerando:

- fluxo principal
- cenários negativos
- validações de campos
- comportamentos inesperados

---

# 6. Cenários, Casos de Teste e Bugs Report

Os cenários e casos de teste foram documentados na planilha abaixo:

[Planilha casos de teste](https://docs.google.com/spreadsheets/d/17iq2LDvsV4VmIwT0kCr4CoUbIBxb3e1tkAB0Ot6Y7RU/edit?gid=0#gid=0)   

[Planilha de bugs report](https://docs.google.com/spreadsheets/d/17iq2LDvsV4VmIwT0kCr4CoUbIBxb3e1tkAB0Ot6Y7RU/edit?gid=181569196#gid=181569196)

---

# 7. Execução dos Testes

Os testes foram executados manualmente na aplicação.

Os resultados foram registrados na planilha de testes.

Evidências da execução:

Evidencias estão na pasta evidencias/testes e evidencias/bugs e nas planilhas acima relacionada com seus respectivos casos de testes e bugs

---

# 8. Bugs Encontrados

Durante a execução dos testes foram identificados diversos problemas no sistema.

Os bugs estão documentados na planilha:

[Planilha de bug reports](https://docs.google.com/spreadsheets/d/17iq2LDvsV4VmIwT0kCr4CoUbIBxb3e1tkAB0Ot6Y7RU/edit?gid=181569196#gid=181569196)

---