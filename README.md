# CRUD com Spring Boot, Spring MVC, MySQL e Thymeleaf

## Sobre o Projeto
Este projeto é um sistema CRUD (Create, Read, Update, Delete) desenvolvido com **Spring Boot** e **Spring MVC**, utilizando **MySQL** como banco de dados e **Thymeleaf** para renderização de templates no frontend. 

## Tecnologias Utilizadas
- **Spring Boot**
- **Spring MVC**
- **Spring Data JPA**
- **Thymeleaf**
- **MySQL**
- **Spring Boot DevTools**
- **Spring Validation**
- **Spring Boot Starter Test**

## Funcionalidades
- Criar novos registros
- Listar registros existentes
- Editar registros
- Excluir registros

## Dependências
No arquivo `pom.xml`, foram utilizadas as seguintes dependências principais:

```xml
<dependencies>
    <!-- Spring Data JPA -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-data-jpa</artifactId>
    </dependency>

    <!-- Thymeleaf -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-thymeleaf</artifactId>
    </dependency>

    <!-- Spring Validation -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-validation</artifactId>
    </dependency>

    <!-- Spring Web -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>

    <!-- Spring Boot DevTools -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-devtools</artifactId>
        <scope>runtime</scope>
        <optional>true</optional>
    </dependency>

    <!-- MySQL Driver -->
    <dependency>
        <groupId>com.mysql</groupId>
        <artifactId>mysql-connector-j</artifactId>
        <scope>runtime</scope>
    </dependency>

    <!-- Spring Boot Starter Test -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-test</artifactId>
        <scope>test</scope>
    </dependency>
</dependencies>
```

## Configuração do Banco de Dados
No arquivo `application.properties`, configure o acesso ao banco de dados MySQL:

```properties
# Configuração de conexão com o banco de dados MySQL
spring.datasource.url=jdbc:mysql://localhost:3306/shop?useSSL=false&serverTimezone=UTC
spring.datasource.username=
spring.datasource.password=
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# Configuração JPA
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

## Como Rodar o Projeto
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd nome-do-projeto
   ```
3. Configure o banco de dados no `application.properties`.
4. Execute o projeto:
   ```bash
   mvn spring-boot:run
   ```
5. Acesse no navegador:
   ```
   http://localhost:8080
   ```

## Estrutura do Projeto
```
├── src
│   ├── main
│   │   ├── java
│   │   │   ├── com.paulo.shop
│   │   │   │   ├── controllers (Controladores)
│   │   │   │   ├── models (Modelos)
│   │   │   │   ├── services (Serviços)
│   │   │   │   ├── ShopApplication.java (Classe principal)
│   │   ├── resources
│   │   │   ├── templates.products (Views Thymeleaf)
│   │   │   ├── static (html)
│   │   │   ├── application.properties (Configuração)
├── pom.xml
```

## Autor
Desenvolvido por **[Paulo André]**.  
Entre em contato via [pauloandre050619@gmail.com] ou pelo GitHub [Pauloand05](https://github.com/Pauloand05).
