Trezo_Core
===============

# General

The purpose of this module is to offer general functionality that is usefull for different Magento 2 projects.

Install in all projects and modules m2 by trezo

# Install

```
	composer require trezoteam/m2-core
```


# Create Trezo Admin Tab

```
	trezo
```


# Functions

## Product

### getCurrentCategory

You can get the current category by using this code in the view template:

```php
<?php
$_helper = $this->helper('Trezo\Core\Helper\Product');
$currentCategory = $_helper->getCurrentCategory();

echo $currentCategory->getName();
?>
```

### getCurrentProduct

You can get the current product by using this code in the view template:

```php
<?php
$_helper = $this->helper('Trezo\Core\Helper\Product');
$currentProduct = $_helper->getCurrentProduct();

echo $currentProduct->getName();
?>
```

## Store

### getCurrentStore

Return the current store

```php
<?php
$_helper = $this->helper('Trezo\Core\Helper\Store');
$currentStore = $_helper->getCurrentStore();
?>
```

### getLocale

Return the current locale associated with the current store.

```php
<?php
$_helper = $this->helper('Trezo\Core\Helper\Store');
echo $_helper->getLocale();
?>
```

## Customer

### isLoggedIn

Checks if the customer is logged in

```php
<?php
$_helper = $this->helper('Trezo\Core\Helper\Customer');
$isLoggedIn = $_helper->isLoggedIn();
?>
```

### getCurrentCustomer

Returns the current customer if logged in. If not logged in, it will return false.

```php
<?php
$_helper = $this->helper('Trezo\Core\Helper\Customer');
$customer = $_helper->getCurrentCustomer();
?>
```
