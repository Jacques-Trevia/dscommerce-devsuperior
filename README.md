# DSCommerce - DevSuperior
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Jacques-Trevia/dscommerce-devsuperior/blob/main/LICENSE)

**DSCommerce** é um projeto desenvolvido no curso de Desenvolvedor Moderno da [DevSuperior](https://devsuperior.com.br/), focado no backend com **Spring Boot** e conceitos de **componentes e injeção de dependência**.

## 🛒 Sobre a Aplicação

A aplicação consiste em um **e-commerce completo**, permitindo que os usuários possam navegar por produtos, realizar pedidos e efetuar pagamentos. O sistema conta com um back-end robusto baseado em **Spring Boot**, garantindo segurança, escalabilidade e boa manutenção do código.

---

## Layout web
![Web 1](https://user-images.githubusercontent.com/91570669/206563257-9ed8ea6e-c18d-4893-a696-407e8a21a618.png)

![Web 2](https://user-images.githubusercontent.com/91570669/206563258-bddb163c-40a3-4ebb-9367-b960411c147c.png)

![Web 3](https://user-images.githubusercontent.com/91570669/206563261-d66c954c-985b-415c-b0ee-9eaeeab6c5a1.png)

![Web 4](https://user-images.githubusercontent.com/91570669/206563249-4ce550f1-fd7d-4088-9c55-0dd54b7d6ab1.png)

---

## Modelo conceitual
![Modelo Conceitual](https://user-images.githubusercontent.com/91570669/206563729-68b3128d-03f5-4870-8350-52c3655a8ac7.png)

---

## 🚀 Tecnologias Utilizadas

- **Java 17**
- **Spring Boot**
- **Spring Data JPA**
- **H2 Database**
- **PostgreSQL**
- **Maven**

---

## 📂 Estrutura do Projeto

O projeto segue a arquitetura de camadas, com:
- 📁 **Entities** (Entidades JPA)
- 📁 **Repositories** (DAO para banco de dados)
- 📁 **Services** (Regras de negócio e lógica da aplicação)
- 📁 **Controllers** (Endpoints da API REST)

---

## 🧪 Testes com Postman

Para facilitar os testes da API, disponibilizo uma coleção completa com todos os endpoints e um environment pré-configurado.

### 📁 Arquivos

| Arquivo | Descrição |
|---------|-----------|
| [DS-Commerce-Collection.json](./postman/DS-Commerce-Collection.json) | Coleção com todas as requisições (produtos, categorias, pedidos, usuários, autenticação) |
| [DS-Commerce-Environment.json](./postman/DS-Commerce-Environment.json) | Environment com variáveis (`base_url`, `token`, `client_id`, etc.) |

### 🚀 Como importar

1. Faça o download dos dois arquivos acima
2. Abra o **Postman**
3. Clique em **Import** (botão no canto superior esquerdo)
4. Arraste os arquivos para a janela ou selecione-os manualmente
5. No canto superior direito, selecione o environment **"DS-Commerce"**
6. A variável `{{base_url}}` já está configurada como `http://localhost:8080`. Altere se necessário.

### 🔐 Fluxo de autenticação

1. Execute a requisição **"Obter token"** na pasta `auth`
2. Use as credenciais padrão:
   - **Admin:** `admin@admin.com` / `123456`
   - **Operator:** `operator@operator.com` / `123456`
3. Após obter o token, as demais requisições protegidas já utilizam `{{token}}` automaticamente

### ⚙️ Variáveis do Environment

| Variável | Valor padrão | Descrição |
|----------|--------------|-----------|
| `base_url` | `http://localhost:8080` | URL base da API |
| `client_id` | `myclientid` | Client ID do OAuth2 |
| `client_secret` | `myclientsecret` | Client Secret do OAuth2 |
| `token` | *(preenchido automaticamente)* | Token JWT obtido no login |

---

## 📦 Como Rodar o Projeto

### 🔧 Configuração Inicial

1. Clone o repositório:
   ```sh
   git clone https://github.com/Jacques-Trevia/dscommerce-devsuperior.git
   ```
2. Importe o projeto no **Eclipse** ou **IntelliJ** como um projeto Maven.
3. Verifique se o **JDK 17** está instalado e configurado.

### 💾 Banco de Dados

O projeto usa **H2** para desenvolvimento e **PostgreSQL** para produção. Para acessar o console do **H2**:

- Execute a aplicação e acesse: [http://localhost:8080/h2-console](http://localhost:8080/h2-console)
- Configure:
  ```
  JDBC URL: jdbc:h2:mem:testdb
  Usuário: sa
  Senha: (deixe em branco)
  ```

### ▶️ Executando a Aplicação

1. No terminal ou IDE, execute:
   ```sh
   mvn spring-boot:run
   ```
2. Acesse a API via **http://localhost:8080**

---

## 📌 Funcionalidades

✔️ Cadastro e gerenciamento de produtos  
✔️ Autenticação e autorização de usuários  
✔️ Processamento de pedidos e pagamentos  

---

## 📜 Licença

Este projeto é parte do curso da **DevSuperior** e tem propósito educacional.

---

## 👨‍💻 Autor

**Jacques Araujo Trevia Filho**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jacques-trevia)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Jacques-Trevia)
