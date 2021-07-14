# Insurance-App

## Run me

1. Make in the root directory a folder called:  `mysql`
2. docker-compose up -d --build site       
3. docker-compose exec php php /var/www/html/artisan migrate 
4. docker-compose exec php php /var/www/html/artisan passport:install
5. docker-compose run --rm npm run dev  
6. docker-compose run --rm --service-ports npm run watch 
7. Navigate to http://localhost/
8. Enjoy

## Architecture

* Docker
* MySQL
* Redis
* Dockerized PHP with version lookup (Can't get it wrong because the ini file is located inside.)
* Laravel
* Laravel Passport (Yes we can easily switch to OAuth here if we really wanted to)
* React
* React Flux
* MailGun (For all the mail spamming.)
