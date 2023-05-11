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

### Quick setup
- Run `cd docker`
- Run `docker-compose up -d --build`
- Enter to Php container via Docker Desktop
- Run `symfony new ../app --webapp`
- Make file `app/.env.local` from `app/.env`
- Configure database url in `.env.local`, use this `DATABASE_URL="mysql://root:secret@database:3306/symfony_docker?serverVersion=8.0"`

### Notes
- You need to clean `app` folder before start to create new symfony app
- Right database url: `DATABASE_URL="mysql://root:root@database:3306/db01?serverVersion=8.0"`
    - user = `root`
    - password = `root`
    - host = `database`
    - port = `3306`
    - base = `db01`
 