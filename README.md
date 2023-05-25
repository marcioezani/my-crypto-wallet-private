# <p align="center"><b>CRUD App with Laravel 10 and MySQL</b></p>

<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

In this tutorial you'll be learning to use Laravel 10 to build a CRUD web app with a MySQL database from scratch starting with the installation of Composer (PHP package manager) to implementing and serving your application.

Read the full tutorial: [Laravel 10 Tutorial: Build your First CRUD App with Laravel and MySQL (PHP 8.1)](https://www.techiediaries.com/php-laravel-crud-mysql-tutorial/)

## Prerequisites

This tutorial assumes you have PHP and MySQL installed on your system. Follow the instructions for your operating system to install both of them.

You also need to be familiar with Linux/macOS bash where we'll be executing the commands in this tutorial.

Familiarly with PHP is required since Laravel is based on PHP.

For development I will be using a Ubuntu 20.04 machine so the commands in this tutorial are targeting this system but you should be able to follow this tutorial in any operating system you use.

# Laravel CRUD App - MY CRYPTO WALLET

A simple CRUD App with control login with Laravel 10.

- dashboard

- crud: COINS

- crud: WALLET

- crud: USERS

Created and modified with the bootstrap template free from COINEX ( https://templates.iqonic.design/lite/coinex/dashboard/html/dist/ )

## Installation

Clone the repository-
```
git clone ...
```

Then cd into the folder with this command-
``` 
cd my-crypto-wallet
```

Then do a composer install
```
composer install
```

Then create a environment file using this command-
```
cp .env.example .env
```

Then edit `.env` file with appropriate credential for your database server. Just edit these two parameter(`DB_USERNAME`, `DB_PASSWORD`).

Then create a database named `laravelcrud` and then do a database migration using this command
```
php artisan migrate --seed
```

Create the currency register with the CSV file already included in the application, create with custom command ( App\Console\Commands\ImportCoinsCSV ) created to import coins
```
php artisan coinscsv
```

## Run server

Run server using this command-
```
php artisan serve
```

Then go to `http://localhost:8000` from your browser and see the app.

User login:
```
e-mail: admin@crypto.com

password: admin123
```

## Screenshot

![](https://thumbs2.imgbox.com/77/68/6FgEewZ2_t.png)
![](https://thumbs2.imgbox.com/86/3e/w7o7Cluy_t.png)
![](https://thumbs2.imgbox.com/66/7f/1ecH4Em5_t.png)

## Credits

- [MEZ](https://github.com/marcioezani)
