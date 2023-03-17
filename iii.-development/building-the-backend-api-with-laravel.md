# Building the backend API with Laravel

Laravel is a popular PHP web framework that provides developers with the tools and features needed to build robust and scalable web applications. One of the key features of Laravel is its ability to quickly build and deploy web APIs. In this guide, we will provide a step-by-step tutorial on how to build a backend Laravel Web API in Laravel Homestead virtual machine.

Step-by-step Guide:

1. Install Laravel: First, you need to install Laravel on your system. You can install it using composer, which is a dependency manager for PHP. Open your terminal and run the following command:

```bash
composer create-project --prefer-dist laravel/laravel my-api
```

This command will create a new Laravel project in a directory named "my-api".

2. Create a Controller: Laravel follows the MVC (Model-View-Controller) pattern, and the controller is responsible for handling the incoming requests and returning the response. Create a new controller using the following command:

```bash
php artisan make:controller ApiController
```

This command will create a new controller named "ApiController" in the "app/Http/Controllers" directory.
