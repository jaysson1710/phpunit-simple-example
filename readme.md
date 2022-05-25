## Status buils

|branch|[![PHP Composer](https://github.com/jaysson1710/phpunit-simple-example/actions/workflows/php.yml/badge.svg)](https://github.com/jaysson1710/phpunit-simple-example/actions/workflows/php.yml)|


A Simple PHPUnit Example
========================

This is a simple example of unit testing in PHP with PHPUnit. I used these examples as part of a talk given at Sheffield PHP on the 18th January 2018. The talk has been written up as a blog post: [PHPUnit: What, Why, How?](https://andy-carter.com/blog/phpunit-what-why-how).

Please feel free to download this repository and give the unit tests a try.

As mentioned in my blog post try adding a second test case for the `Average::median` method to test when an even set of numbers is passed to the method.

If you succeed at that, then try taking a test driven development approach to adding a new method to `Average` for calculating the modal average by writing a test first.

Getting Started
---------------

Clone this repository and then run Composer:-

```
composer install
```

You will then be able to run the unit tests using:-

```
./vendor/bin/phpunit
```

## Comandos de instalacion PHP version 7.4 

```bash
#!/bin/bash

apt-get update
export DEBIAN_FRONTEND=noninteractive
apt update     && apt install -y software-properties-common    && add-apt-repository -y ppa:ondrej/php     
apt-get update     && apt-get install -y wget git unzip nano
 
apt-get install -y curl php7.4-cli php7.4-mbstring  phpunit php7.4 php7.4-common php7.4-opcache php7.4-mcrypt php7.4-cli php7.4-gd php7.4-curl php7.4-mysql php7.4-xml php7.4-intl php7.4-intl php7.4-mbstring php7.4-zip php7.4-mbstring php7.4-xdebug
   
    
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
COMPOSER=906a84df04cea2aa72f40b5f787e49f22d4c2f19492ac310e8cba5b96ac8b64115ac402c8cd292b8a03482574915d1a8
php -r "if (hash_file('SHA384', 'composer-setup.php') === '$COMPOSER') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php --install-dir=/usr/local/bin --filename=composer
  
wget https://phar.phpunit.de/phpunit.phar
chmod +x phpunit.phar
mv phpunit.phar /usr/local/bin/phpunit


############ comandos unasvez instalado el PHP y el composer

git clone https://github.com/drmonkeyninja/phpunit-simple-example.git
cd phpunit-simple-example/

composer update
composer require cviebrock/eloquent-sluggable
composer install

export XDEBUG_MODE=coverage
vendor/bin/phpunit --log-junit junit.xml
phpunit --coverage-clover coverage-report.xml

```
