# 🏥 CRUD - Farmácia

Este é um projeto de uma API REST desenvolvida com **Spring Boot**, que implementa um **CRUD** (Create, Read, Update, Delete) para gerenciar produtos de uma farmácia. Os produtos estão classificados por categorias e o sistema permite realizar operações essenciais sobre ambas as entidades.

---
## 🚀 Tecnologias Utilizadas
- **Java 17**
- **Spring Boot** (Spring Web, Spring Data JPA, Spring Validation)
- **Hibernate** (ORM para banco de dados relacional)
- **MySQL** (Banco de dados relacional)
- **Insomnia  (Para testar as requisições da API)
- **Maven** (Gerenciador de dependências)
---
## 📌 Funcionalidades
- **CRUD de Categorias** (6 endpoints)
- **CRUD de Produtos** (6 endpoints)
- **Relacionamento entre Produtos e Categorias** (OneToMany e ManyToOne)
- **Validações com Bean Validation**


---
## 🗃️ Estrutura do Banco de Dados
### **Tabela `tb_categoria`**
| Campo | Tipo |
|--------|--------|
| id | BIGINT (PK, Auto Increment) |
| descricao | VARCHAR(255) |

### **Tabela `tb_produtos`**
| Campo | Tipo |
|--------|--------|
| id | BIGINT (PK, Auto Increment) |
| nome | VARCHAR(100) |
| preco | DOUBLE |
| marca | VARCHAR(1000) |
| data_validade | VARCHAR(255) |
| categoria_id | BIGINT (FK - `tb_categoria.id`) |

---
## 🔄 Endpoints da API
### **CategoriaController** (`/categorias`)
- `GET /categorias` → Retorna todas as categorias
- `GET /categorias/{id}` → Retorna uma categoria por ID
- `POST /categorias` → Cadastra uma nova categoria
- `PUT /categorias` → Atualiza uma categoria existente
- `DELETE /categorias/{id}` → Remove uma categoria por ID

### **ProdutoController** (`/produtos`)
- `GET /produtos` → Retorna todos os produtos
- `GET /produtos/{id}` → Retorna um produto por ID
- `GET /produtos/nome/{nome}` → Busca produtos por nome
- `POST /produtos` → Cadastra um novo produto
- `PUT /produtos` → Atualiza um produto existente
- `DELETE /produtos/{id}` → Remove um produto por ID

---
## 📂 Estrutura do Projeto
```
📦 src
 ┣ 📂 main
 ┃ ┣ 📂 java.com.generation.farmacia
 ┃ ┃ ┣ 📂 controller  # Camada responsável pelos endpoints
 ┃ ┃ ┣ 📂 model       # Representação das entidades do banco
 ┃ ┃ ┣ 📂 repository  # Camada de acesso ao banco de dados
 ┃ ┃ ┗ 📜 CrudfarmaciaApplication # Classe principal do Spring Boot
 ┃ ┗ 📂 resources
 ┃ ┃ ┣ 📜 application.properties  # Configurações do banco de dados
```

---
## 📜 Licença
Este projeto foi desenvolvido como parte de um desafio de aprendizado e não possui fins comerciais.

📌 **Desenvolvido por:** Victoria Borges 🚀
# 🏥 CRUD - Farmácia

Este é um projeto de uma API REST desenvolvida com **Spring Boot**, que implementa um **CRUD** (Create, Read, Update, Delete) para gerenciar produtos de uma farmácia. Os produtos estão classificados por categorias e o sistema permite realizar operações essenciais sobre ambas as entidades.

---
## 🚀 Tecnologias Utilizadas
- **Java 17**
- **Spring Boot** (Spring Web, Spring Data JPA, Spring Validation)
- **Hibernate** (ORM para banco de dados relacional)
- **MySQL** (Banco de dados relacional)
- **Insomnia  (Para testar as requisições da API)
- **Maven** (Gerenciador de dependências)
---
## 📌 Funcionalidades
- **CRUD de Categorias** (6 endpoints)
- **CRUD de Produtos** (6 endpoints)
- **Relacionamento entre Produtos e Categorias** (OneToMany e ManyToOne)
- **Validações com Bean Validation**


---
## 🗃️ Estrutura do Banco de Dados
### **Tabela `tb_categoria`**
| Campo | Tipo |
|--------|--------|
| id | BIGINT (PK, Auto Increment) |
... (49 linhas)
