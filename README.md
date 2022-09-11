git clone -b last https://gitlab.com/khoji2001/Laravel_Shop.git

docker-compose build && docker-compose up -d

docker-compose exec blog_app bash

composer install 

cp .env.example .env

php artisan key:generate

apt-get update && apt-get install nano

nano .env

DB_CONNECTION=mysql
DB_HOST=blog_db
DB_PORT=3306
DB_DATABASE=simple
DB_USERNAME=root
DB_PASSWORD=r0312327129oot

php artisan migrate

chmod -R 0777 storage/

mkdir images

mkdir videos

mkdir first

chmod -R 0777 public/


docker restart $(docker ps -q)
