Installing CCDNComponent AttachmentBundle 1.0
=============================================

## Dependencies:

No dependencies.

## Installation:

Installation takes only 3 steps:

1. Download and install the dependencies.
2. Register bundles with autoload.php.
3. Run vendors install script.

### Step 1: Download and install the dependencies.

Add to your deps.

``` ini
[lib-geshi]
	git=http://github.com/codeconsortium/lib-geshi.git
	target=/geshi
```
### Step 2: Register bundles with autoload.php.

Add to your autoload.php

``` php
// app/autoload.php
$loader->registerPrefixes(array(
    'Geshi_' => __DIR__.'/../vendor/geshi/lib',
	**...**
));
```

### Step 3: Run vendors install script.

From your projects root Symfony directory on the command line run:

``` bash
$ php bin/vendors install
```

## Next Steps.

Installation should now be complete!

To use GeSHi use:

``` php
	$geshi = new \Geshi_Geshi($tag, $lang);	
```

If you need further help/support, have suggestions or want to contribute please join the community at [Code Consortium](http://www.codeconsortium.com)

[Return back to the docs index](http://github.com/codeconsortium/lib-geshi/blob/master/Resources/doc/index.md).
