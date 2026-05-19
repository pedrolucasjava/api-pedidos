# Pedidos API

API REST desenvolvida para gerenciamento de pedidos, clientes e produtos.

O projeto foi criado com foco em aprendizado prático de desenvolvimento backend utilizando Java e Spring Boot, aplicando conceitos utilizados em sistemas corporativos reais.

---

# Objetivos do Projeto

* Praticar desenvolvimento backend moderno
* Construir uma API REST escalável
* Aplicar arquitetura em camadas
* Trabalhar com regras de negócio reais
* Implementar autenticação e segurança
* Desenvolver um projeto forte para portfólio

---

# Tecnologias Utilizadas

* Java 21
* Spring Boot
* Spring Web
* Spring Data JPA
* Spring Security
* JWT
* PostgreSQL
* Hibernate
* Swagger/OpenAPI
* Maven
* Lombok

---

# Funcionalidades

## Clientes

* Cadastro de usuarios
* Atualização de usuarios
* Remoção de usuarios
* Busca por ID
* Listagem paginada

## Produtos

* Cadastro de produtos
* Atualização de produtos
* Remoção de produtos
* Controle de preço
* Controle de estoque

## Pedidos

* Criação de pedidos
* Associação de múltiplos itens
* Cálculo automático do valor total
* Histórico de pedidos
* Busca por cliente
* Listagem paginada

## Autenticação

* Login com JWT
* Rotas protegidas
* Controle de acesso

---

# Regras de Negócio

* Não é permitido cadastrar produtos duplicados
* O estoque é atualizado automaticamente após pedidos
* Pedidos sem itens não são permitidos
* O valor total do pedido é calculado automaticamente
* Clientes não podem realizar pedidos sem autenticação

---

# Paginação e Filtros

A API possui suporte para:

* Paginação
* Busca por cliente

Exemplo:

```http
GET /pedidos?=0
```

---

# Estrutura do Projeto

```bash
src
 ├── controller
 ├── dto
 ├── entity
 ├── enums
 ├── repository
 ├── security
 ├── service
 └── config
```

---

# Documentação da API

A documentação da API é gerada automaticamente com Swagger/OpenAPI.

Após iniciar o projeto, acesse:

```bash
http://localhost:8080/swagger-ui/index.html
```

---

# Como Executar o Projeto

## Pré-requisitos

* Java 21
* PostgreSQL
* Maven

## Clone o repositório

```bash
git clone <URL_DO_REPOSITORIO>
```

## Configure o banco de dados

No arquivo `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/pedidos_api
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```

## Configuração do projeto

Para rodar o projeto, configure as variáveis de ambiente:

- MAIL_USERNAME = email utilizado para envio de notificações
- MAIL_PASSWORD = app password do Gmail
- JWT_SECRET = chave secreta para geração de tokens JWT
## Execute a aplicação

```bash
mvn spring-boot:run
```

---

# Melhorias Futuras

* Testes unitários
* Testes de integração
* Docker
* Deploy em nuvem
* Cache
* Logs centralizados
* CI/CD

---

# Autor

Desenvolvido por Pedro Lucas como projeto de estudo e portfólio para desenvolvimento backend Java.
