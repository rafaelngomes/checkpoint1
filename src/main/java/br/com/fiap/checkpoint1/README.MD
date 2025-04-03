# Checkpoint 1 - Microservice and Web Engineering
*Rafael Nascimento Gomes - RM550843*
*Rafael Arcoverde Melo - RM550206*


# Documentação da API Checkpoint1

Este é um projeto de API Spring Boot para o Checkpoint1.

## Instalação

* Limpe e crie a pasta */target*:

```bash
mvn clean package
```

* Configuração do Swagger

https://springdoc.org/properties.html
- application.properties
    
    ```
    spring.application.name=checkpoint1
    springdoc.swagger-ui.path=/
    ```

## Navegação
### Executando a API
* Execute usando **Maven**:
```bash
mvn spring-boot:run
```

### Documentação da API (Swagger)
- Acesse o Swagger UI em: *http://localhost:8080/*

## Estrutura do Projeto
O projeto está organizado como uma aplicação Spring Boot padrão:
- `src/main/java/br/com/fiap/checkpoint1`: Código principal da aplicação
- `src/test/java/br/com/fiap/checkpoint1`: Classes de teste


Criação de API para responder as requisições HTTP (POST, GET, DELETE e PUT):

Criar Paciente (POST);
Atualizar Paciente (PUT);
Deletar Paciente (DELETE);
Buscar Paciente por Id (GET);
Buscar todos os Pacientes (GET);

A aplicação está organizada nos seguintes pacotes:

model: Contém as classes de entidade (Paciente).
service: Camada de regra de negócio.
controller: Responsável por expor os endpoints da API.
dto: Objetos de transferência de dados para as requisições e respostas.

## Dependências
Este projeto utiliza as seguintes dependências principais:
- Spring Boot 3.4.3
- Spring Boot DevTools
- Spring Boot Test
- SpringDoc OpenAPI UI 2.5.0

## Referências
- [Documentação SpringDoc OpenAPI](https://springdoc.org/)
- [Documentação Spring Boot](https://spring.io/projects/spring-boot)