# Sile 2.0 redis service provider
Redis service provider for silex 2.0


## install 

> composer require cnam/redis-service-provider:0.0.1

Or add your composer.json

> require "cnam/redis-service-provider":"0.0.1"

## Configure

```php

$app['redis.options'] = [
    'host'     => 'redis',
    'port'     => 6379,
    'timeout'  => 0,
    'dbname'   => 'my_box',
    'password' => 'qwerty'
];

$app->register(new Silex\Provider\RedisServiceProvider());

```

## Usage

```php

/**
* @var $redis \Redis
**/
$redis = $app['redis'];

```

