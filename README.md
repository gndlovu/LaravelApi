# Laravel Task Manager API
This is a laravel package that adds task management functionality to web applications.

It supports Laravel 5.0 and later

## Installation

[PHP](https://php.net) 5.4+ and [Composer](https://getcomposer.org) are required.

To get the latest version of Laravel LaravelApi, simply add the following line to the require block of your `composer.json` file.

```
"gndlovu/LaravelApi": "dev-master"
```

You'll then need to run `composer install` or `composer update` to download it and have the autoloader updated.

If you are using Laravel 5.5 or later, the service provider auto discovery feature will load the required classes after installation otherwise, you need to register the service provider. Open up `config/app.php` and add the following to the `providers` key.

* `gndlovu\LaravelApi\LaravelApiServiceProvider::class`


## Configuration

You need to run migrations to create tasks table

```bash
php artisan migrate"
```

You can publish the configuration file using this command:

```bash
php artisan vendor:publish --tag=public
```

Then you are ready to get runnings. Just visit 

```bash
http://{{site-url}}/api/v1/tasks
```

The front-end for this API can be found at (https://github.com/gndlovu/ng2-laravel)
