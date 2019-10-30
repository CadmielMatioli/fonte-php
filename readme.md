<p align="center"><img src="https://res.cloudinary.com/dtfbvvkyp/image/upload/v1566331377/laravel-logolockup-cmyk-red.svg" width="400"></p>

# Seguimento

    Os codigos a seguir serão apresentados a partir do laravel ja instalado
    o repositorio ja com develop, e clonado no meu computador, 
    a partir disso eu inicio esses comandos no meu terminal
    
## Heroku App Tutorial in Laravel 5.8.*
 
#### Procfile.
 
    Primeiro Criei um arquivo Procfile na pasta raiz do Laravel
    Depois eu dicionei o seguinte codigo dentro dela "web: vendor/bin/heroku-php-apache2 public/"
     
#### Inserido comandos para iniciar depois do laravel instalado e o Procfile criado
  
    heroku login
    heroku create
   
#### Não utilizei o git init ja tinha a develop então fui direto para o comando.
   
    git push heroku master 
    
#### Então foi adicionado meu repositório no app project no heroku
    
   https://shielded-dusk-86282.herokuapp.com/
   
#### Para adicionar o Database eu coloquei o comando.
   
    heroku addons:create heroku-postgresql:hobby-dev
    
   Voce consegue visualizar a sua database em Heroku->myapp->Resources
   Depois de acessar sua database ja criada vá em Settings->ViewCredentials...
   
#### Na minha .env do repositório local eu coloquei o seguinte comando.
   
    DB_CONNECTION=pgsql
    DB_HOST= 12-3-4-5-.asd-1.amazonaws.com
    DB_PORT= 5432
    DB_DATABASE= sua-base-de-dados(nome)
    DB_USERNAME= seu-nome-de-usuário(nome)
    DB_PASSWORD=sua-senha(nome)
    
#### Feito isso coloquei o seguinte comando.
   
    heroku run php /app/artisan migrate --seed
#### Como resposta...
   
    Do you really wish to run this command? (yes/no) [no]: y
    
### Todos os comandos foram executados dentro da minha pasta clonada do git localmente diretamente na master
