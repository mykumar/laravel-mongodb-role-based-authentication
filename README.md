# laravel-mongodb-role-based-authentication
laravel and JensSegers mongodb Role Base Authentication Model

Installation
------------

Make sure you have the MongoDB PHP driver installed. You can find installation instructions at http://php.net/manual/en/mongo.installation.php

Mongo DB jenssegers is added to the composer.json file.

```
composer install
```

If you need to install sepeartely [Jenssegers\Mongodb library](https://github.com/jenssegers/laravel-mongodb/blob/master/README.md). 
You can install it using composer:

```
composer require jenssegers/mongodb
``` 

Following are the things added in this project
------------

* validate method role is added in the AuthController 
* register.blade.php has two options at registration
* AuthController checked each value i.e. not an array -- Security Issue for MongoDB
* App\User.php role method added
* App\Middlewares\ Folder Two MiddleWares Created InfluencerMiddleWare and BrandMiddleWare
* All the MiddleWares are registered In the Kernel.php 
* Two Controllers Added BrandController and Influencer Controller
* BrandController constructor added brand-middleware and InfluencerController constructor added influencer-middleware
