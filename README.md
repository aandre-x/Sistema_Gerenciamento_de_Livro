# 📚 Gerenciador de Livros

Este projeto consiste em uma API REST desenvolvida com **Spring Boot**, que oferece funcionalidades para gerenciar um catálogo de livros. Através dessa API, é possível **listar**, **adicionar** e **remover** livros por meio de endpoints RESTful.

---

## 🚀 Funcionalidades

- ✅ Visualizar todos os livros cadastrados
- ✅ Inserir um novo livro no catálogo
- ✅ Excluir um livro com base no ID

---

## 🛠 Tecnologias Utilizadas

- Java 17+
- Spring Boot
- Spring Web
- Jakarta Bean Validation (JSR 380)

---

## 📄 Endpoints da API

### 🔍 Visualizar livros

- **Método:** `GET /livros`  
- **Descrição:** Retorna todos os livros cadastrados no sistema.  
- **Resposta:**
  - `200 OK` com a lista de livros
  - `204 No Content` caso não haja livros cadastrados

📘 **Exemplo de resposta:**

```json
[
  {
    "id": "1",
    "titulo": "Dom Casmurro",
    "autor": "Machado de Assis"
  }
]
➕ Inserir um novo livro
Método: POST /livros

Descrição: Cadastra um novo livro no sistema.

Campos obrigatórios: titulo, autor

Corpo da requisição:

json
Copiar
Editar
{
  "titulo": "1984",
  "autor": "George Orwell"
}
Resposta: 201 Created

📘 Exemplo de resposta:

json
Copiar
Editar
{
  "id": "2",
  "titulo": "1984",
  "autor": "George Orwell"
}
❌ Excluir livro por ID
Método: DELETE /livros/{id}

Descrição: Remove o livro identificado pelo ID fornecido.

Resposta: 204 No Content em caso de sucesso

▶️ Como rodar o projeto
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/seuusuario/seu-repositorio.git
Acesse o diretório do projeto:

bash
Copiar
Editar
cd seu-repositorio
Execute a aplicação utilizando o Maven Wrapper:

bash
Copiar
Editar
./mvnw spring-boot:run
Nota: Certifique-se de ter o Java 17 ou superior instalado na sua máquina.

👤 Autor
Criado por @ancribeiro