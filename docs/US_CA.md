## User Stories e Criterios Aceite

## 1. User Story — Listar Cursos

**User Story**
Como usuário
Quero visualizar a lista de cursos cadastrados
Para consultar os cursos disponíveis.

### Critérios de Aceitação

- A página inicial deve exibir a lista de cursos cadastrados.
- Cada curso deve aparecer em formato de card.
- O card deve exibir as informações do curso.
- Cada card deve possuir um botão Excluir.

Caso não existam cursos cadastrados, o sistema deve exibir um estado vazio.

## 2. User Story — Cadastrar Curso

**User Story**
Como usuário
Quero cadastrar um novo curso
Para disponibilizá-lo na lista de cursos.

### Critérios de Aceitação

- O sistema deve possuir um formulário de cadastro.
- O formulário deve possuir os seguintes campos:
    - Nome
    - Descrição
    - Instrutor
    - URL da imagem
    - Data início
    - Data fim
    - Número de vagas 
    - Modalidade

O sistema deve permitir selecionar Presencial ou Online.
Dependendo da modalidade, campos adicionais devem aparecer.
Após o cadastro, o curso deve aparecer na lista.

## 3. User Story — Selecionar Modalidade do Curso
**User Story**
Como usuário
Quero selecionar a modalidade do curso
Para informar se o curso será presencial ou online.

### Critérios de Aceitação

- O campo modalidade deve possuir:
    - Presencial
    - Online

A seleção deve alterar o formulário.

## 4. User Story — Excluir Curso

**User Story**
Como usuário
Quero excluir um curso
Para remover cursos que não são mais necessários.

### Critérios de Aceitação

- Cada curso deve possuir botão Excluir.
- Ao clicar no botão, o curso deve ser removido da lista.