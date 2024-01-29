# Laravel_Docker_Env

Creare un nuovo progetto Laravel:
  - docker-compose run --rm composer create-project --prefer-dist laravel/laravel .

  IMPORTANTE: Bisogna modificare nel file .env in src il nome del db, nome utente e password di mysql e cambiare anche db_host in mysql

Startare i conteiner di nginx, php, mysql e phpmyadmin:
  - docker-compose up -d --build server

Spegnere i container:
  - docker-compose down

Comandi per usare artisan:
  - docker-compose run --rm artisan ...   --> es. Per la migrate: docker-compose run --rm artisan migrate

Accesso DB da phpmyadmin:
  - Nome Database: mysql  (Il nome del conteiner del nostro db)
  - Nome Utente: root     (Si può modificare nel file mysql.env)
  - Password: root        (Si può modificare nel file mysql.env)
