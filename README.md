# Sistema de Lista de Produtos

Este é um projeto de um **Sistema de Lista de Produtos** desenvolvido em **Java (Spring Boot)** para o backend e **HTML/CSS/JavaScript** para o frontend e **Banco da Dados H2**. O sistema permite adicionar, editar, visualizar e excluir produtos em uma lista, com uma interface moderna e responsiva.

# Sistema de Lista de Produtos

[](https://github.com/Alexdevsoft/sistema-de-lista-produtos/actions/workflows/build.yml/badge.svg)
[![Java Version](https://img.shields.io/badge/Java-17-blue.svg)](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html)
[![Powered by Spring Boot](https://img.shields.io/badge/Powered%20by-Spring%20Boot-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![Database-H2](https://img.shields.io/badge/Database-H2-blue.svg)](https://www.h2database.com)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Maven](https://img.shields.io/badge/Maven-CC0000?style=flat&logo=apache-maven&logoColor=white)](https://maven.apache.org/)
[![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=flat&logo=thymeleaf&logoColor=white)](https://www.thymeleaf.org/)
---

## Funcionalidades

1. **Adicionar Produto:**
   - Abre um modal para inserir os dados do produto (nome, preço e quantidade).
   - O produto é salvo no banco de dados e a tabela é atualizada automaticamente.

2. **Editar Produto:**
   - Permite editar os dados de um produto existente.
   - Atualiza o produto no banco de dados e na tabela.

3. **Excluir Produto:**
   - Remove um produto da lista após confirmação.
   - Atualiza a tabela automaticamente.

4. **Visualizar Produtos:**
   - Exibe todos os produtos em uma tabela com colunas para ID, Nome, Preço, Quantidade e Total (preço × quantidade).

5. **Interface Moderna:**
   - Design limpo e profissional, com animações suaves e responsividade.

---

## Tecnologias Utilizadas

- **Backend:**
  - Java (Spring Boot)
  - Spring Data JPA
  - H2 Database (banco de dados em memória)

- **Frontend:**
  - HTML5
  - CSS3 (estilos modernos e responsivos)
  - JavaScript (manipulação do DOM e requisições AJAX)
 
- **Banco de Dados:**
  - H2

- **Ferramentas:**
  - Maven (gerenciamento de dependências)
  - Thymeleaf (templates HTML)
  - H2 (database)

---

## Como Executar o Projeto

### Pré-requisitos

- Java JDK 17 (ou superior) instalado.
- Maven instalado.
- Navegador moderno (Chrome, Firefox, Edge, etc.).

### Passos para Execução

1. Clone o repositório:

   ```bash
   git clone https://github.com/Alexdevsoft/sistema-de-lista-de-produtos.git
   cd sistema-lista-produtos

   mvn clean install
   mvn spring-boot:run

  ### Acesse o aplicativo
    http://localhost:8080
  ### Em outra aba do navegador acesse o Banco de Dados H2
    http://localhost:8080/h2-console

  # Detalhes Técnicos

## Backend

### ProdutoController:
- Controlador Spring Boot que gerencia as requisições HTTP (GET, POST, DELETE).
- **Endpoints:**
  - `GET /`: Exibe a lista de produtos.
  - `POST /adicionar-produto`: Adiciona um novo produto.
  - `DELETE /deletar-produto/{id}`: Exclui um produto pelo ID.

### Produto:
- Modelo que representa um produto com os atributos: `id`, `nome`, `preco`, `quantidade`.

### ProdutoRepository:
- Interface que estende `JpaRepository` para operações de banco de dados.

### H2 Database:
- Banco de dados em memória usado para armazenar os produtos.

---

## Frontend

### lista.html:
- Página principal que exibe a tabela de produtos e o modal para adicionar/editar produtos.

### styles.css:
- Estilos CSS para a página, incluindo animações e design moderno.

### scripts.js:
- Lógica JavaScript para manipulação do DOM, requisições AJAX e interações com o backend.

---

## Capturas de Tela

### Página Principal

[![Página principal](https://i.postimg.cc/cHdG6HQt/lista-de-produtos.png)](https://postimg.cc/JyY22RYR)

# Modal de Adicionar Produto

[![modal.png](https://i.postimg.cc/qRNGTfRh/modal.png)](https://postimg.cc/9Rj9dnyC)

# Produto Adicionado
[![lista-de-produtos2.png](https://i.postimg.cc/dtq2b8cd/lista-de-produtos2.png)](https://postimg.cc/kDpR8R4X)

# Banco de Dados H2

[![H2.png](https://i.postimg.cc/zBKnwvwJ/H2.png)](https://postimg.cc/5Y9YbxkG)

[![H2-PRODUTOS.png](https://i.postimg.cc/9MZn4Wr9/H2-PRODUTOS.png)](https://postimg.cc/7GPVdr1P)

---

# **Responsividade:**
   - Melhorar a experiência em dispositivos móveis.

---

# Contribuição

Contribuições são bem-vindas! Siga os passos abaixo:

1. Faça um fork do projeto.
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`).
3. Commit suas mudanças (`git commit -m 'Adicionando nova feature'`).
4. Push para a branch (`git push origin feature/nova-feature`).
5. Abra um Pull Request.

---

# Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

# Contato

- **Nome:** Alexsandro Almeida
- **Email:** alexhavilla2022@gmail.com
- **GitHub:** [Alexdevsoft](https://github.com/Alexdevsoft)
