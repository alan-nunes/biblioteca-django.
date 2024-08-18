# Trilha 7 - Desenvolvimento Back-End (Python)

## Exercício Prático: ORM Django, Serializadores e Function-Based Views

### Contexto

Você está desenvolvendo um sistema de gerenciamento de biblioteca que permite a administração de livros, autores e categorias. Neste exercício, você vai praticar o uso do Django ORM para realizar operações de CRUD, além de criar serializers manualmente usando a classe `Serializer`. As views serão implementadas usando function-based views (FBVs).

### Objetivo

- Criar modelos para Livros, Autores e Categorias.
- Praticar operações de CRUD usando o Django ORM no shell.
- Criar serializers manuais com a classe `Serializer`.
- Implementar function-based views para uma API RESTful.
- Criar um repositório público no GitHub para a submissão do exercício.

### Funcionalidades

O sistema de gerenciamento de biblioteca possui as seguintes funcionalidades principais:

#### Modelos

1. **Categoria**
    - `nome`: Nome da categoria (ex.: "Ficção", "Ciência").

2. **Autor**
    - `nome`: Nome do autor (ex.: "Isaac Asimov", "Carl Sagan").

3. **Livro**
    - `titulo`: Título do livro (ex.: "Fundação", "Cosmos").
    - `autor`: Referência ao autor do livro.
    - `categoria`: Referência à categoria do livro.
    - `publicado_em`: Data de publicação do livro.

#### Operações CRUD no Django Shell

1. **Criação**
    - Criação de categorias, autores e livros com dados específicos.

2. **Consulta**
    - Listagem de livros por categoria.
    - Consulta de detalhes de um livro específico.

3. **Atualização**
    - Atualização de informações de um livro existente (ex.: título).

4. **Exclusão**
    - Exclusão de um livro do banco de dados.

#### API RESTful com Function-Based Views

1. **Listar e Criar Livros**
    - `GET /livros/`: Retorna uma lista de todos os livros.
    - `POST /livros/`: Cria um novo livro com base nos dados fornecidos.

2. **Detalhar, Atualizar e Deletar Livros**
    - `GET /livros/<id>/`: Retorna os detalhes de um livro específico.
    - `PUT /livros/<id>/`: Atualiza os dados de um livro específico.
    - `DELETE /livros/<id>/`: Remove um livro específico do banco de dados.
