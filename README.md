# docker-compose: Laravel
Aiming at a simple [Laradock](https://github.com/laradock/laradock).  
This application makes use of the following:
- nginx
- php-fpm
- mariadb

## Feature

- Only one command to execute
- Not need to build a docker image
- Multiple versions can be selected


## Usage
## Up
    docker-compose up -d

## Clean
    docker-compose kill
    docker-compose rm -f
    rm -rf laravel

Now you can access `http://localhost`.
And development source code at `laravel` directory.

## Supported versions

|Laravel|PHP-FPM|
|-------|-------|
| 5.4   | 7.1   |
| 5.3   | 7.1   |
| 5.2   | 7.1   |
| 5.1   | 7.1   |

Edit `docker-compose.yml`.  
 
    image: shomatan/laravel:LARAVEL_VERSION-php-PHP-FPM_VERSION

Example:

    image: shomatan/laravel:5.1-php-7.1

## Configuration
### Change the access port
Edit `nginx.conf` and `docker-compose.yml`

## Author
Shoma Nishitateno