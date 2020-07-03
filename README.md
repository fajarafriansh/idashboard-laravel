# iDashboard Laravel
I have implemented iDashboard into a fresh Laravel 7.x app. Simply clone this repo and start building your next Laravel project on top of this admin panel template. This project makes a very little and basic use of VueJS and compiled JS is already bundled with the project. If you want to make it more dynamic, you can update the Vue components or add your own.

## Installation
Clone the repo:
```shell
git clone https://github.com/fajarafriansh/idashboard-laravel.git
```

Install composer packages:
```shell
composer update
```

Copy and rename .env.example to .env, update the environmental variables and set an app key:
```shell
php artisan key:generate
```

After that, run all migrations and seed the database:
```shell
php artisan migrate
```
```shell
php artisan db:seed
```

Or if your database is fresh and you haven't done any work yet, then it's safe to call the commands in a single line:
```shell
php artisan migrate:refresh --seed
```

Note that seeding the database is compulsory as it will create the necessary roles and permissions for the user CRUD provided by the project.

After that, install laravel passport:
```shell
php artisan passport:install
```

Visit <div style="display: inline">http://yoursite.com/login</div> to sign in using below credentials:

### Demo
URL: https://stisla.rehmat.works

#### Demo Admin Login
*  Email: admin@example.com
*  Password: 1234

#### Demo Editor Login
*  Email: editor@example.com
*  Password: 1234

#### Demo User Login
*  Email: user@example.com
*  Password: 1234

P.S.: Password modification and user deletion is disabled in demo mode.

This project comes with a user CRUD and makes the use of [Spatie Roles and Permissions](https://github.com/spatie/laravel-permission) at a very basic level in order to give restricted access to the three roles provided above. You can move forward with the same logic to achieve more complex goals.

### Credits:
*   [Laravel](https://github.com/laravel/laravel)
*   [iDashboard Admin Panel Template](https://github.com/stisla/stisla)
*   [Spatie Laravel Roles and Permissions](https://github.com/spatie/laravel-permission)
*   [vue-ios-alertview](https://github.com/Wyntau/vue-ios-alertview)

### Contribution:
Contribution is welcomed and highly appreciated. Fork the repo, make your updates and initiate a pull request. I'll approve all pull requests as long as they are constructive and follow the Laravel standard practices.
