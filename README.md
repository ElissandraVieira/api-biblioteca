#  API Biblioteca

Projeto desenvolvido como atividade acadêmica do curso de Análise e Desenvolvimento de Sistemas do Instituto Federal do Piauí (IFPI).

A API Biblioteca é uma aplicação REST desenvolvida com Java e Spring Boot, com o objetivo de realizar o gerenciamento de livros, permitindo cadastrar, listar e buscar livros por identificador.

## Tecnologias utilizadas

- Java 21
- Spring Boot
- Spring Web
- Spring Data JPA
- Banco de dados H2
- Maven
- Git e GitHub

##  Funcionalidades

- Cadastrar livros.
- Listar todos os livros cadastrados.
- Buscar um livro pelo ID.
- Retornar erro 404 quando um livro não for encontrado.
- Armazenar os dados no banco H2 com persistência em arquivo.

##  Endpoints da API

| Método | Endpoint | Descrição |
|---|---|---|
| POST | `/livros` | Cadastrar um livro |
| GET | `/livros` | Listar todos os livros |
| GET | `/livros/{id}` | Buscar livro pelo ID |

##  Exemplo de cadastro

**POST** `/livros`

```json
{
  "titulo": "Dom Casmurro",
  "autor": "Machado de Assis",
  "anoPublicacao": 1899,
  "disponivel": true
}
```

##  Como executar o projeto

1. Clone o repositório:

```bash
git clone https://github.com/ElissandraVieira/api-biblioteca.git
```

2. Entre na pasta do projeto:

```bash
cd api-biblioteca
```

3. Execute a aplicação pelo terminal:

```bash
.\mvnw.cmd spring-boot:run
```

4. Acesse a API:

```text
http://localhost:8080/livros
```

##  Banco de dados H2

A aplicação utiliza o banco de dados H2 com armazenamento em arquivo.

Para acessar o console, utilize:

```text
http://localhost:8080/h2-console
```

**Configurações de acesso:**

- JDBC URL: `jdbc:h2:file:./data/bibliotecadb`
- User Name: `sa`
- Password: deixar vazio.

##  Autora

**Elissandra Vieira**

Curso: Análise e Desenvolvimento de Sistemas (ADS)

Instituição: Instituto Federal do Piauí (IFPI)

---

Projeto acadêmico desenvolvido para praticar a criação de APIs REST utilizando Java e Spring Boot.
