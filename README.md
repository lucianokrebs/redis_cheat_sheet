# Redis cheat sheet

One more redis cheat sheet to help decrease the learning curve to use Redis

## Recommended GUI

1. RedisInsight | [Link](https://redislabs.com/redis-enterprise/redis-insight/)

## Running redis with docker

1. Create a docker volume to store redis data:

```shell
 docker volume create redis_data
```

2. Use the `docker-compose.yml` inside this project to run redis locally with:

```shell
docker compose up --build -d
```

3. Connect to redis using the CLI

```shell
redis-cli
```

4. Test your local connection with the `PING` command:

![img.png](images/redis-cli.png)

## Insert values

```
SET users:101:timezone UTC-3
```
