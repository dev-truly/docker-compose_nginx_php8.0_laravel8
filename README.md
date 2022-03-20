## docker-compose
### * 셋팅 환경
#### ubuntu:20.04, nginx, php8.0, laravel8

### * 실행 순서  
```bash
# 로컬 터미널
$ docker-compose up -d --build
$ docker exec -it nginx_php8_laravel8 bash
# ------------------------------------------

# 도커 컨테이너 쉘(shell)
$ laravel new laravel8
$ chown -R www-data laravel8
$ service php8.0-fpm start
$ service nginx start
```

* [http://localhost:8080/index.php](http://localhost:8080/index.php) 접속

참고 URL : [도찐개찐 Docker nginx + php8.0 + laravel8 설치하기](https://dev-truly.tistory.com/entry/6-Docker-nginx-php80-laravel8-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0)