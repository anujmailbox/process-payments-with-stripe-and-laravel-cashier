# [Process Payments With Stripe and Laravel Cashier][published url]
## Instructor: [Jason Lewis][instructor url]


Stripe is a payment processing service that comes with a suite of easy-to-use APIs that powers e-commerce for businesses of all sizes. Stripe makes it easy to implement secure credit-card transactions while providing your users the convenience of in-page checkout. Not only that, but Stripe has built-in support for subscriptions and recurring billing.

Laravel is the perfect back-end technology for implementing a Stripe-powered store. Along with Laravel's built-in object-relational mapping, routing and authentication functionality, there is also native support for Stripe with Laravel Cashier. 

In this course, Envato Tuts+ instructor Jason Lewis will show you how to process payments on Stripe using Laravel Cashier. You'll cover a number of key topics, including how to prepare your database for payments and pointers to the security concerns you should be aware of when handling cardholder data. You'll also learn how to process single, one-off payments for an online shopping cart, and even how to handle Stripe subscriptions.


## Source Files Description

This is a very minimal application with much of the code existing in the `app/Http/routes.php` file. This code base demonstrates how you can use
Cashier component to bill users of your web application. The other files that you might like to explore are the models, `app/User.php`, `app/Cart.php`, and `app/Product.php`. These
contain relationships that link the data to each other.

To get this code base up and running on your local machine you'll first need to clone this repository. Then, you'll need to run the following commands:

```
composer install
```

Once the dependencies are installed you'll need to configure your database settings by renaming `.env.example` to `.env`. You'll then need to provide a `STRIPE_SECRET` key in your `.env` file.

This secret can key be obtained from your Stripe account dashboard, make sure you use your testing key when developing locally.

You'll then be able to run the following commands:

```
php artisan migrate
php aritsan db:seed
```

You can then serve the application using `php artisan serve` or by utilizing Homestead.

------

These are source files for the Tuts+ course: [Process Payments With Stripe and Laravel Cashier][published url]

Available on [Tuts+](https://tutsplus.com). Teaching skills to millions worldwide.

[published url]: https://code.tutsplus.com/courses/process-payments-with-stripe-and-laravel-cashier
[instructor url]: https://tutsplus.com/authors/jason-lewis
