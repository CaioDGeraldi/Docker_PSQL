# Comandos Docker <a href="https://skillicons.dev"> <img src="https://skillicons.dev/icons?i=docker" width="30px" /></a>

```bash
docker images
```
> Verifica todas as imagens já instaladas.

```bash
docker ps -a
```
> Verifica todos os contêiners.

```bash
docker ps
```
> Verifica todos os contêiners inicializados.

```bash
docker pull postgres:latest
```
> **postgres** = Nome da imagem. <br> **latest** = Versão da imagem.

```bash
docker run -d --name postgresql -p 5432:5432 -e POSTGRES_PASSWORD=admin postgres
```
> Roda o contâiner. <br> Parâmetros: 
> * **-d** roda em segundo plano.
> * **--name** define o nome do contêiner.
> * **-p** define a porta.
> * **-e POSTGRES_PASSWORD=admin** define a senha do usuário POSTGRES como admin.
> * **postgres** é o serviço que vai rodar no contêiner.

```bash
docker start postgresql
```
> Inicia o contêiner.

```bash
docker stop postgresql
```
> Para o contêiner.

# Comandos Postgres <a href="https://skillicons.dev"> <img src="https://skillicons.dev/icons?i=postgres" width="30px" /></a>
```bash
docker exec -it postgresql createdb -U postgres banco_teste
```
> **createdb** Cria o banco de dados.

```bash
docker exec -it postgresql psql -U postgres banco_teste
```
> **psql** Abre o terminal do PostgreSQL.
