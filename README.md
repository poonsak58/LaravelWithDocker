# LaravelWithDocker
Sample run laravel with Docker container. such as nginx, php, mariadb, composer, node

Credit : https://we.in.th/docker-laravel-docker-52eb2d039753

`$ docker-compose up`
`$ docker exec laravelwithdocker_php_1 php artisan migrate`

then open http://localhost:8000

```
$ docker exec laravelwithdocker_php_1 php artisan make:model Product -m
// Or
$ docker exec -it laravelwithdocker_php_1 bash
# php artisan make:model Product -m
```

## Use Cach Redis.
```
docker run --rm --interactive --tty \ 
--volume $PWD:/app \
composer require predis/predis
```
