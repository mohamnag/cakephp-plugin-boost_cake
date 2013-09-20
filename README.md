# BoostCakeExtended

This is an extension for BoostCake to provide default options for each element 
to make it simple while using the standard notation of CakePHP. BoostCakeExtended
is a plugin for CakePHP using Bootstrap.

* [The original BoostCake (not needed)](https://github.com/slywalker/cakephp-plugin-boost_cake)
* [Bootstrap(2.3.2)](http://getbootstrap.com/2.3.2/)
* [Bootstrap(3.0.0)](http://getbootstrap.com/)

## Requirements

* CakePHP >= 2.3
* Bootstrap >= 2.3 (3.0 support)

## Installation

Clone the code from Github.

### Enable plugin

First you need to load the plugin in your app/Config/bootstrap.php file:

`CakePlugin::load('BoostCake');`

If you are already using `CakePlugin::loadAll();`, then this is not necessary.

Then you have to replace the default helpers with the ones from this plugin:

```
<?php
class AppController extends Controller {

	public $helpers = array(
		'Session',
		'Html' => array('className' => 'BoostCake.BoostCakeHtml'),
		'Form' => array('className' => 'BoostCake.BoostCakeForm'),
		'Paginator' => array('className' => 'BoostCake.BoostCakePaginator'),
	);

}
```

## Documentation

There is no separate documentation for this plugin right now, the original 
documentation can be found here:

[BoostCake - Bootstrap Plugin for CakePHP](http://slywalker.github.io/cakephp-plugin-boost_cake/)