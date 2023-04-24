<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# Books API
Simple API with CRUD operations to manage data for your books collection.

## Installation and Usage

### Install Docker Desktop (https://www.docker.com/products/docker-desktop/)

### Clone the main branch on this repo

In the root directory there is a file called .env.example. Duplicate this file and name it .env and run the following command to generate the APP_KEY
```
php artisan key:generate
```
Run the migrations with the following command:
```
php artisan migrate
```
Run the project with the following command
```
./vendor/bin/sail up
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
