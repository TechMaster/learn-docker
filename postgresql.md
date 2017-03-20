# Hướng dẫn thực hành cài đặt Postgresql bằng Docker

## Hello World
docker run hello-world

## Sử dụng alpine
docker run -it alpine /bin/sh

## Pull image Postgresql 
docker pull postgres:9.6.2-alpine

docker run --name db -e POSTGRES_PASSWORD=abc -d postgres
docker run --name db -e POSTGRES_PASSWORD=abc -d postgres:9.6.2-alpine
docker run -p 127.0.0.1:5432:5432 --name db -e POSTGRES_PASSWORD=abc -d -t postgres:9.6.2-alpine

## kiểm tra những container nào đang chạy
docker ps -a

## stop một container
docker stop db

## remove một container
docker rm db
