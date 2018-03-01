## LaravelShippingcart

A fork of [LaravelShoppingcart]() that adds support for shipping.

## Installation

Install the package through [Composer](http://getcomposer.org/). 

Run the Composer require command from the Terminal:

    composer require gloudemans/shoppingcart
    
If you're using Laravel 5.5, this is all there is to do. 

You can then replace the files in your /vendor/gloudemans/shoppingcart directory with the files from this repository.

## Usage

Adding an item to the cart is really simple, you just use the `add()` method, which accepts a variety of parameters.

In its most basic form you can specify the id, name, quantity, price and shipping of the product you'd like to add to the cart.

```php
Cart::add('293ad', 'Product 1', 1, 9.99, 1.99);
```

As an optional fifth parameter you can pass it options, so you can add multiple items with the same id, but with (for instance) a different size.

```php
Cart::add('293ad', 'Product 1', 1, 9.99, 1.99 ['size' => 'large']);
```
