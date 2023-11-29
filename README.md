# docker-drupal-postgres-setup

Docker compose file configuration for a multi-container project

### Images

- drupal:9
- postgres:14

### Instructions

1. Rename `.env-sample` to `.env` and add the variable values

2. Run docker compose

```bash
docker compose up
```

OR run in background

```bash
docker compose up -d
```

3. Once containers are up, open `http://localhost:PORT` in your browser and begin project setup

Note: In database config section. Under advanced, change Host value from `localhost` to `pgdb` which is the db service name in docker-compose.yml

#### final

Run the following commands to exit process and gracefully shutdown running services

```bash
ctrl + c
```

```bash
docker compose down -v
```
