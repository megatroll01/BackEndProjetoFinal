# MyWorkManager Backend

Este é o projeto final da pos graduação desenvolvido com Spring Boot. O projeto fornece uma API para gerenciar funcionários e outras funcionalidades.

## Requisitos

Antes de iniciar o projeto, certifique-se de que você tem as seguintes ferramentas instaladas:

- [Java JDK 17](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html)
- [Apache Maven](https://maven.apache.org/download.cgi)
- [MySQL](https://dev.mysql.com/downloads/)

## Configuração do Banco de Dados

As configurações do banco de dados estão localizadas no arquivo `src/main/resources/application.properties`. 

Aqui está um exemplo de como as configurações podem estar configuradas:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/mydatabase
spring.datasource.username=root
spring.datasource.password=secret
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

- `spring.datasource.url`: URL de conexão do banco de dados.
- `spring.datasource.username`: Nome de usuário do banco de dados.
- `spring.datasource.password`: Senha do banco de dados.
- `spring.jpa.hibernate.ddl-auto`: Configura o comportamento do Hibernate para criar/atualizar as tabelas no banco de dados. `update` faz com que as tabelas sejam criadas ou atualizadas automaticamente ao iniciar o projeto.
- `spring.jpa.show-sql`: Configura o Spring Data JPA para mostrar as consultas SQL executadas.

## Como Rodar o Projeto

1. Clone o repositório:

    ```bash
    git clone https://github.com/seuusuario/myworkmanager_back.git
    cd myworkmanager_back
    ```

2. Compile e inicie o projeto usando Maven dentro da masta do projeto /myworkmanager_back:

    ```bash
    ...myworkmanager_back> mvn clean install
    ...myworkmanager_back> mvn spring-boot:run
    ```

    Ou você pode usar o comando `mvn` para rodar diretamente:

    ```bash
    ...myworkmanager_back> mvn spring-boot:run
    ```

3. O aplicativo será iniciado na porta padrão `8081`. Você pode acessar a API via [http://localhost:8081](http://localhost:8081).

## Dependências

Este projeto usa as seguintes dependências:

- **Spring Boot Starter Data JDBC** e **Spring Boot Starter Data JPA** para acesso ao banco de dados.
- **Spring Boot Starter Web Services** para suporte a Web Services.
- **Spring Boot DevTools** para facilidades durante o desenvolvimento.
- **MySQL Connector** para conectar o MySQL ao Spring Boot.
- **Lombok** para reduzir o boilerplate de código.
## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
