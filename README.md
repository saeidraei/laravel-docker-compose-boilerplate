# Laravel Docker Compose Boilerplate

#### steps to run the project for development:
1. install [docker](https://docs.docker.com/install/)
2. install [docker-compose](https://docs.docker.com/compose/install/)
3. clone the repository
8. copy the `.env.example` file to `.env` using this command in project's root:
   ```bash
   cp src/.env.example src/.env
   ```
9. run `docker-compose up -d` and there you go ;
your development environment is ready at http://localhost:8060. if you want to
 have it running always in background run
 `docker-compose -f dev-docker-compose.yml up -d`.

## FAQ
1. how to run artisan or php commands?

   a: open an interactive shell to your app container using `docker exec -it ldb_app bash` then you have php and composer available.
