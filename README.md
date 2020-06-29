# eve-microservice-template

Template repository for a microservice


### Usage

[Create repository from template](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template)

# Docs template

# Microservice name

Description

## Docs

Auto-generated API documentation located at /v1/doc route.

## Development
* Copy `config/jwt/public.pem` from [auth](https://github.com/f1monkey/auth) service to `config/jwt` folder

* Copy `docker-compose.override.yml.dist` to `docker-compose.override.yml`
```
cp docker-compose.override.yml.dist docker-compose.override.yml
```
* Run docker containers
```
$ docker-compose up -d
```
* Connect to php container
```
$ docker-compose exec php bash
```
## Testing
Run static analyse
```
$ composer phpstan
```

Run tests:
```
$ composer test
```
