# 📚 Biblioteca Digital – Projeto de Programação Orientada a Objetos

Este projeto é uma aplicação Java desenvolvida com foco nos princípios de **Programação Orientada a Objetos (POO)**. Ele simula um sistema de cadastro e gerenciamento de livros, com interface web, persistência em banco de dados MySQL e estrutura modular baseada no padrão **MVC**.

---

## 🚀 Tecnologias Utilizadas

- **Java 8+**
- **Maven** (gerenciador de dependências)
- **MySQL** (persistência de dados)
- **JDBC** (`mysql-connector-java`)
- **HTML/CSS/JS** (interface)
- **IntelliJ IDEA** ou **Eclipse**
- **Padrão MVC** (Model - View - Controller)

---

## 🗂 Estrutura do Projeto

Case_POO-main/
├── pom.xml # Configuração Maven
├── mysql-connector-java-8.0.25.jar # Driver JDBC
├── src/
│ └── main/
│ ├── java/
│ │ └── br/com/fecaf/
│ │ ├── App.java # Classe principal
│ │ ├── Model/Livro.java # Entidade Livro
│ │ ├── Repository/LivroRepository.java # Acesso ao banco
│ │ ├── Service/Livro_Service.java # Regras de negócio
│ │ └── RestController/LivroRestController.java # API REST
│ ├── resources/
│ │ ├── application.properties # Configuração do BD
│ │ ├── templates/
│ │ │ ├── index.html # Página inicial
│ │ │ ├── css/style.css # Estilo visual
│ │ │ ├── js/script.js # Lógica do frontend
│ │ │ └── img/Capa_Livro.jpg # Imagem decorativa
│ └── Database/codigo_sql.sql # Script SQL do banco


---

## ⚙️ Como Executar o Projeto

### 1. Pré-requisitos

- Java JDK 8 ou superior
- MySQL instalado
- Maven instalado
- IDE Java (como IntelliJ ou Eclipse)

### 2. Configurar o banco de dados

1. No MySQL, crie o banco de dados (ajuste o nome se quiser):
```sql
CREATE DATABASE biblioteca;

2. Execute o script disponível em:

src/main/java/br/com/fecaf/Database/codigo_sql.sql

3. Ajustar application.properties
No arquivo src/main/resources/application.properties, configure com seu usuário e senha do MySQL:

properties
spring.datasource.url=jdbc:mysql://localhost:3306/biblioteca
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

4. Compilar e executar
No terminal:

bash
mvn clean install
mvn exec:java

✅ Funcionalidades
📖 Cadastrar novo livro

🔍 Pesquisar livro por título

✏️ Editar informações de um livro

❌ Excluir livro do catálogo

🌐 Interface amigável com HTML/CSS

🗃️ Conexão com banco de dados MySQL
