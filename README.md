Laravel docker environment running on PHP8 with fpm, 
nginx as reverse proxy, mysql and redis.

To get up an running with an existing laravel project:

1.) clone and cd into this project.
2.) clone your laravel project and cd into it.
3.) install composer dependiences like: 
    docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/opt \
    -w /opt \
    composer install --ignore-platform-reqs
4.) set your aplication key, run migrations, install npm dependencies, compile assets etc.
