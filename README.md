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

If you dont find something that you need here look at the documentation of the 
original plugin here:

[BoostCake - Bootstrap Plugin for CakePHP](http://slywalker.github.io/cakephp-plugin-boost_cake/)

### BoostCakeFormHelper

When using this helper, you may define the following options while initiating 
the Helper:

#### formClass
This defines which class would be set as default for the form. Default value is
'well form-inline' but you may change it to something else like this:

```
<?php
public $helpers = array(
    'Form' => array(
        'className' => 'BoostCake.BoostCakeForm',
        'formClass' => 'well'
    ),
```

