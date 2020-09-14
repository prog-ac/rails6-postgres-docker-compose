# Ruby on Rails 6 & Postgres docker-compose

## 初回

```
docker rm -f $(docker ps -aq)
docker-compose build
docker-compose up -d
docker-compose exec rails bash
rails new . -d postgresql
```

## 次回以降

```
docker rm -f $(docker ps -aq)
docker-compose build
docker-compose up -d
docker-compose exec rails bash
rails new . -d postgresql
```

[http://localhost:3000](http://localhost:3000)
