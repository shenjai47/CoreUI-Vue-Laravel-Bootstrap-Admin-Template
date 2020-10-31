# Installation
▶clone the repo

$ git clone https://github.com/shenjai47/CoreUI-Vue-Laravel-Bootstrap-Admin-Template.git my-project

▶go into app's directory

$ cd my-project/laravel

▶install app's dependencies

$ composer install

▶install app's dependencies

$ npm install
# If you choose MySQL
Copy file ".env.example", and change its name to ".env". Then in file ".env" complete this database configuration:

DB_CONNECTION=mysql

DB_HOST=127.0.0.1

DB_PORT=3306

DB_DATABASE=laravel

DB_USERNAME=root

DB_PASSWORD=
# Next step
▶generate laravel APP_KEY

$ php artisan key:generate

▶generate jwt secret

$ php artisan jwt:secret

▶run database migration and seed

$ php artisan migrate:refresh --seed

▶go to coreui directory

$ cd ../coreui

▶install app's dependencies

$ npm install
# test usage
$ php vendor/bin/phpunit
# If you need separate backend and frontend
▶back to laravel directory

$ cd ../laravel

▶start local server

$ php artisan serve

$ cd ../coreui

$ npm run serve

Open your browser with address: localhost:8080

If you need change backend adress go to file /coreui/src/main.js And change line:

Vue.prototype.$apiAdress = 'http://127.0.0.1:8000'
# When you have project open in browser
Click "Login" on sidebar menu and log in with credentials:

E-mail: admin@admin.com

Password: password

This user has roles: user and admin
