<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# Books API
Simple API with CRUD operations to manage data for your book collection.
## Installation

### Install PHP
```sudo apt install php8.1-cli
sudo apt-get install php-common php-mysql
sudo apt-get install php-mbstring
sudo apt install php-xml
sudo apt install php-curl
```

### Install MySQL
```
sudo apt install mysql-server
```

### Install Composer
```php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === '55ce33d7678c5a611085589f1f3ddf8b3c52d662cd01d4ba75c0ee0459970c2200a51f492d557530c71c15d8dba01eae') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
sudo mv composer.phar /usr/local/bin/composer
```

## Usage

### Steps to run the project
Clone the repository
Create a database and configure your .env file in the project.
Run the following commands on the project directory path
```
composer install
php artisan key:generate
php artisan migrate
```
Run the project with the following command
```
php artisan serve
```
### Available endpoints
|HTTP method|CRUD|Endpoint|
|----------|:-------------:|------:|
|GET|Retrieve all books|api/books|
|POST|Create Book|api/books|
|GET|Search book by title|api/books/search/{title}|               
|GET|Retrieve book by id| api/books/{id}|   
|PUT|Update book|api/books/{id}|   
|DELETE|Delete book|api/books/{id}|   
|POST|Log In user|api/login|
|POST|Log out user|api/logout| 
|POST|Register user|api/register|   
