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

# Autor

Jacques Araujo Trevia Filho
