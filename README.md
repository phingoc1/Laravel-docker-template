- Containing nginx server, mysql, php, redis, composer, npm, artisan, phpmyadmin, queue worker, cron.  

- Start docker: docker-compose up -d --build site
- Composer: docker-compose run --rm composer update
- NPM: docker-compose run --rm npm run dev
- Artisan: docker-compose run --rm artisan migrate
- Mix watch: docker-compose run --rm --service-ports npm run watch
- Check Cron: docker-compose exec php ps aux
- Start Cron: docker-compose exec -d php crond -f
