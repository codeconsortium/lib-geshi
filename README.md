CCDNForum Forum Bundle(s) README.
=================================

This is a lib file for use in a project with Symfony2.

Notes: 
------

This bundle is for the symfony framework and thusly requires Symfony 2.0.x and PHP 5.3.6
  
This project uses Doctrine 2.0.x and so does not require any specific database.
  

This file is part of the CCDNForum Bundle(s)

(c) CCDN (c) CodeConsortium <http://www.codeconsortium.com/> 

Available on github <http://www.github.com/codeconsortium/>

For the full copyright and license information, please view the LICENSE
file that was distributed with this source code.

See also: [Add third party libraries to symfony 2](http://www.kiwwito.com/article/add-third-party-libraries-to-symfony-2)

Installation:
-------------

1) Add to your deps.

```sh
[libgeshi]
	git=http://github.com/codeconsortium/geshi.git
	target=/geshi
```

2) Add to your autoload.php

```sh
# app/autoload.php

$loader->registerPrefixes(array(
    'Geshi_' => __DIR__.'/../vendor/geshi/lib',
));
```

3) To use GeSHi use:

```php
	$geshi = new \Geshi_Geshi($tag, $lang);	
```
