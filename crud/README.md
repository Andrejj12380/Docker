
## 1. Building image / Создание образа

```
docker build ./ --tag=stocks_products

```

## 2. Running the container / Запуск контейнера

```
docker run --name=crud_docker -d -p 6060:6060 stocks_products

```