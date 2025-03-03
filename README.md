# docker-compose-travel-list

Documentation:
https://drive.google.com/file/d/1iVp9a3oYjshrISeccIb1o95K0d4R87Si/view?usp=sharing

Instructions:

```
cd travellist-demo
cp .env.example .env
docker-compose build app
docker-compose up -d
docker-compose exec app rm -rf vendor composer.lock
docker-compose exec app composer install
docker-compose exec app php artisan key:generate
```

Access site: http://server_domain_or_IP:8000. For example, http://192.168.85.128:8000/

Live site:
![image](https://github.com/pavelrahman619/docker-compose-travel-list/assets/96363207/88e87aae-a189-425d-a770-51db305d9e85)



References:
https://www.digitalocean.com/community/tutorials/how-to-install-and-set-up-laravel-with-docker-compose-on-ubuntu-22-04
