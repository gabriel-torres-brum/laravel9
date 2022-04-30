
# Setup Docker Para Projetos Laravel 9 com PHP 8

### Passo a passo
Clone Repositório
```sh
git clone https://github.com/gabriel-torres-brum/laravel9.git laravel9
```

```sh
cd laravel9/
```


<!-- Alterne para a branch laravel 8.x
```sh
git checkout laravel-9-com-php-8
``` -->


Remova o versionamento
```sh
rm -rf .git/
```


<!-- Crie o Arquivo .env
```sh
cd example-project/
cp .env.example .env
``` -->
## Instale o docker e siga os passos abaixo:

Suba os containers do projeto
```sh
docker-compose up -d
```

Acessar o container
```sh
docker-compose exec app bash
```

Instalar as dependências do projeto
```sh
composer update
```

Gerar a key do projeto na .env
```sh
php artisan key:generate
```


Acesse o projeto
[http://localhost:8000](http://localhost:8000)
