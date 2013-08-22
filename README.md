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

Ensure require is present in composer.json. This will install the plugin into Plugin/BoostCake:

	{
		"require": {
			"slywalker/boost_cake": "*"
		}
	}

### Enable plugin

You need to enable the plugin your app/Config/bootstrap.php file:

`CakePlugin::load('BoostCake');`

If you are already using `CakePlugin::loadAll();`, then this is not necessary.

## Documentation

[BoostCake - Bootstrap Plugin for CakePHP](http://slywalker.github.io/cakephp-plugin-boost_cake/)

## Development Policy

More Simple! Simple! Simple!

* Develop only those that method's $options in FormHelper unable to solve.
* Don't develop ajax/js helper

If you want to simplify the options, you can develop WrapBoostCake plugin.

### What is solve in this plugin

* Replace checkbox's and radio's `label`
* Add `div` wrapping input
* Add content before and after `input`
* Add error class in outer `div`
* Change pagination tags
* Change SessionHelper::flash()`s template
