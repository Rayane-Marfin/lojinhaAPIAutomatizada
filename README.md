# Lojinha API Automação
Esse é um repositório que contém a automação de alguns testes de API Rest de um software denominado Lojinha. Os sub-tópicos abaixo descrevem algumas decisões tomadas na estruturação do projeto.

## Tecnologias Utilizadas

- Java
  https://www.oracle.com/br/java/technologies/downloads/#jdk20-windows
- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.8.0
- RestAssured
  https://mvnrepository.com/artifact/io.rest-assured/rest-assured/5.3.1
- Maven
  https://maven.apache.org/

## Testes Automatizados
Testes para validar as partições de equivalência relacionadas ao valor do produto da Lojinha, que estão vinculados diretamente à regra de negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais
- Sempre utilizo a anotação Before Each para capturar o token que será utilizado posteriormente nos métodos de testes
- Armazenei os dados que são enviados para a API através do uso de Classes POJO
- Criei dados iniciais através do uso de classe Data Factory, para facilitar a criação e controle.
- Nesse projeto fiz uso do JUnit 5, o que me deu a possibilidade de usar a anotação Display Name para dar descrições em português para os testes