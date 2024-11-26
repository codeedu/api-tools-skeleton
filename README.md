# API Tools usada no módulo de Comunicação do curso FullCycle

## ######## Aviso ########

Este repositório foi arquivado em detrimento do [https://github.com/devfullcycle/api-tools-skeleton](https://github.com/devfullcycle/api-tools-skeleton).

## Rodar a aplicação

Rode o comando

`docker-compose up`

Acessar `http://localhost:8080` para testar o projeto.

## Usar a aplicação com banco de dados

Crie um arquivo `database.sqlite` na raiz do projeto e crie uma tabela no banco de dados.
O container `apigility` já tem o sqlite3 instalado. Você pode acessar o container com o comando:

`docker-compose exec apigility bash`

E rodar o comando:

`sqlite3 database.sqlite`

Depois de acessar o sqlite, crie uma tabela com o comando:

```sql
CREATE TABLE users (id INTEGER PRIMARY KEY AUTOINCREMENT, name TEXT);
```
