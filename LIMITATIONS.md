# Limitations of Checkout in 2022

### No custom fields

Today, you cannot add custom fields to the form on the Checkout page. If you
need to collect some information that is not already collected by Checkout,
then you'll need to implement your own form to collect that.

### Some features work in one mode, but not others

E.g. You can't use some payment method types in `subscription` and `setup`
mode.

### Shipping can only be limited by country

You can only limit the specific country code you ship to. You cannot
limit to a local region or city, for instance.


### Styling

You can only set:

- primary color
- secondary color
- logo
- one of three border radius: sharp, pill, ???
- one of a couple dozen fonts

### Only _creates_ subscriptions

In `subscription` mode, Checkout only creates new Subscriptions. There isn't a
way to update or manage Subscriptions easily with Checkout (you can technically
use `setup` mode to get a new payment method, but then you have to add the
logic for updating the PM on the customer/subscription).

Instead, users should use the Customer portal to _manage_ subscriptions. A lot
of people are confused by why you cannot start a subscription with the Customer
portal or manage a subscription with Checkout.

At the end of the day it's: **Use Checkout to create a Subscription, and the
Customer portal to manage a Subscription**.
