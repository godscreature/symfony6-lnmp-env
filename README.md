# symfony6-lnmp-env

### Symfony environment:
- Php 8.2
- Nginx 1.24
- Mysql 8.0
- Symfony-cli 5.5
- Composer 2.5

### Docker commands:
- `docker-compose up -d --build` - build containers and start services
- `docker-compose down --remove-orphans` - shut down services

### Symfony commands (should be run in Php container):
- `symfony check:requirements` - check requirements
- `symfony new app --webapp` - build a traditional web application
- `symfony new app` - build a microservice, console application or API

### Notes
- You need clean `app` folder before start to create new symfony app
