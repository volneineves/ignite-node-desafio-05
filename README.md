# Ignite Nodejs: CHAPTER III

![Logo do Markdown](./assets/ignite_node_capa.png)

<h3 align="center">
  Desafio 01 - Database Queries
</h3>

## :computer: Sobre o desafio

Realizar consultas no banco de dados com o TypeORM de três formas:

- ORM
- Query Builder
- Raw Query

### :keyboard: Instalação e Execução do Projeto

- Respositório do projeto

```
> git clone https://github.com/volneineves/ignite-node-desafio-05
```

- Navegue até o diretório principal do projeto

```
> cd ignite-node-desafio-05
```

- Instale as dependências com o Yarn

```
yarn install
```

- Execute container postgres no docker

```
docker run --name ignite-challenge-database-queries -e POSTGRES_DB=queries_challenge -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
```

- Coloque pra rodar os testes

```
yarn test
```

## :white_check_mark: Requisitos

#### UsersRepository
- [x] findUserWithGamesById
- [x] findAllUsersOrderedByFirstName
- [x] findUserByFullName

#### GamesRepository
- [x] findByTitleContaining
- [x] countAllGames
- [x] findUsersByGameId

### Específicação dos testes

#### UsersRepository
- [x] Should be able to find user with games list by user's ID
- [x] Should be able to list users ordered by first name
- [x] Should be able to find user by full name

#### GamesRepository
- [x] Should be able find a game by entire or partial given title
- [x] Should be able to get the total count of games
- [x] Should be able to list users who have given game id


## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](https://github.com/git/git-scm.com/blob/master/MIT-LICENSE.txt) para mais detalhes.

---

Feito por <a href="https://www.linkedin.com/in/volnei-neves">Volnei Neves</a> :wave:
