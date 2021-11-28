Start docker:           docker-compose up -d --build site
Composer:               docker-compose run --rm composer update
NPM:                    docker-compose run --rm npm run dev
Artisan:                docker-compose run --rm artisan migrate
Mix watch:              docker-compose run --rm --service-ports npm run watch
Sjekk Cron:             docker-compose exec php ps aux
Start Cron:             docker-compose exec -d php crond -f