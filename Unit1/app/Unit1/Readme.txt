============================================================================================================
MAGENTO 2 FUNDAMENTALS — UNIT 1 EXERCISES
============================================================================================================

1.3.1.(module name: Unit1_Test and Unit1_Test2) Create a new module. Make a mistake in its config.
Create a second module dependent on the first.

GOALS: Learn the structure of a module in Magento 2 and also the following commands:

+ ENABLE MODULE

php bin/magento module:enable Unit1_Test

+ DISABLE MODULE

php bin/magento module:disable Unit1_Test

+ CLEAR CACHE

php bin/magento cache:clean

+ FLUSH CACHE

php bin/magento cache:flush

============================================================================================================

1.5.1 — Change to develop mode using the .htaccess and throw an exception as a text (the exception should
be displayed)

============================================================================================================

1.5.2 — Cache: Under what circumstances will cleaning the var/cachefolder not work?

Answer: When cache storage is different (separate) from the var/cachefolder. For example, it could be memory
caching like Redis or Memcached. Also, if you are using Varnish, it will be necessary to restart the service:

sudo service varnish restart


