# 📚 Biblioteca Digital – Projeto de Programação Orientada a Objetos  
Este projeto é uma aplicação Java desenvolvida com foco nos princípios de Programação Orientada a Objetos (POO). Ele simula um sistema de cadastro e gerenciamento de livros, com interface web, persistência em banco de dados MySQL e estrutura modular baseada no padrão MVC.

## 🚀 Tecnologias Utilizadas  
- Java 8+  
- Maven (gerenciador de dependências)  
- MySQL (persistência de dados)  
- JDBC (mysql-connector-java)  
- HTML/CSS/JS (interface)  
- IntelliJ IDEA ou Eclipse  
- Padrão MVC (Model - View - Controller)

## ⚙️ Como Executar o Projeto  
1. Pré-requisitos:  
  - Java JDK 8 ou superior  
  - MySQL instalado  
  - Maven instalado  
  - IDE Java (como IntelliJ ou Eclipse)

2. Configurar o banco de dados:  
  - No MySQL, crie o banco de dados:  
    ```sql
    CREATE DATABASE biblioteca;
    ```  
  - Execute o script `codigo_sql.sql` disponível no projeto para criar a tabela de livros.

3. Ajuste o arquivo `application.properties` com suas credenciais do MySQL:  
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/biblioteca  
    spring.datasource.username=seu_usuario  
    spring.datasource.password=sua_senha
    ```

4. Compile e execute o projeto:  
    No terminal:
    ```bash
    mvn clean install  
    mvn exec:java
    ```  
    Ou execute diretamente a classe `App.java` pela IDE.

## ✅ Funcionalidades  
- Cadastro de novos livros  
- Pesquisa de livros por título  
- Edição de informações de livros  
- Exclusão de livros do catálogo  
- Interface web com HTML, CSS e JavaScript  
- Integração com banco de dados MySQL

## 📸 Imagem  
A interface utiliza a imagem `Capa_Livro.jpg` como destaque visual.

## 🛠 Dependências  
As dependências são gerenciadas pelo `pom.xml`. Exemplo:  
```xml
<dependency>  
    <groupId>mysql</groupId>  
    <artifactId>mysql-connector-java</artifactId>  
    <version>8.0.25</version>  
</dependency>
