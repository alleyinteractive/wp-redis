# WP Redis <img align="right" src="https://travis-ci.org/alleyinteractive/wp-redis.png?branch=master" />

WordPress Object Cache using Redis. By Alley Interactive.


Pre-requisites
--------------

* [redis](http://redis.io/)
* [phpredis](https://github.com/nicolasff/phpredis)


Setup
-----

1. Install `object-cache.php` to the `wp-content/object-cache.php`.
2. In your `wp-config.php` file, add your server credentials:

  ```
  $redis_server = array( 'host' => '127.0.0.1', 'port' => 6379, 'auth' => '12345' );
  ```

  or

  ```
  $redis_server = array( 'socket' => '/tmp/redis.sock' );
  ```

3. Optionally, add a unique salt for the keys:

        define( 'WP_CACHE_KEY_SALT', 'my-unique-phrase' );

4. Engage thrusters.


