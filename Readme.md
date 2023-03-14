# Golang Clean Web API (Dockerize) with a full sample project (Car Sale project)

## System Design Diagram

<p align="center"><img src='/docs/files/system_diagram.png' alt='Golang Web API System Design Diagram' /></p>

## Database Design Diagram

<p align="center"><img src='/docs/files/db_diagram.png' alt='Golang Web API System Design Diagram' /></p>

## Used Tools

1. [Gin as web framework](https://github.com/gin-gonic/gin)
2. [JWT for authentication and authorization](https://github.com/golang-jwt/jwt)
3. [Redis for caching](https://github.com/redis/redis)
4. [Elasticsearch for logging database](https://github.com/elastic/elasticsearch)
5. [Beat for log shipping](https://github.com/elastic/beats)
6. [Kibana as log viewer](https://github.com/elastic/kibana)
7. [Postgresql as main database engine](https://github.com/postgres/postgres)
8. [PgAdmin as database management tool](https://github.com/pgadmin-org/pgadmin4)
9. [Prometheus for metric database](https://github.com/prometheus/prometheus)
10. [Grafana for metric dashboards](https://github.com/grafana/grafana)
11. [Validator for endpoint input Validation](https://github.com/go-playground/validator)
12. [Viper for configurations](https://github.com/spf13/viper)
13. [Zap for logging](https://github.com/uber-go/zap)
14. [Zerolog for logging](https://github.com/rs/zerolog)
15. [Gorm as ORM](https://github.com/go-gorm/gorm)
16. [Swagger for documentation](https://github.com/swaggo/swag)
17. Docker compose for run project with all dependencies in docker

## How to run

### Start

```
docker compose -f "docker/docker-compose.yml" up -d --build
```

#### Web API

##### Run local manually [http://localhost:5005](http://localhost:5005)

##### Run in docker [http://localhost:9001](http://localhost:9001)

```
GetTokenUrl: http://localhost:5005/api/v1/users/login-by-username
Username: admin
Password: 12345678
```

#### Kibana

##### [http://localhost:5601](http://localhost:5601)

```
Username: elastic
Password: changeme
```

#### Grafana

##### [http://localhost:3000](http://localhost:3000)

```
Username: admin
Password: foobar
```

#### PgAdmin

##### [http://localhost:8090](http://localhost:8090)

```
Username: h.naimaei@gmail.com
Password: 123456
```

Postgres Server info:

```
Host: postgres_container
Port: 5432
Username: postgres
Password: admin
```

#### Prometheus

##### [http://localhost:9090](http://localhost:9090)

### Stop

```
docker compose --file 'docker/docker-compose.yml' --project-name 'docker' down
```

## Project preview

<p align="center"><img src='/docs/files/swagger.png' alt='Golang Web API preview' /></p>
