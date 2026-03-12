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