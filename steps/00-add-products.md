# 00 Add products

At this point, you've experimented with Payment Links and know they are a great
option for selling a single flavor. But your sister is bummed that she can't
unleash her creative inner child and start selling more flavors like Chocolate
Hazelnut 🍫, Funfetti 🌈, and Tiramisu 🍥!

You know that you need to create some products in Stripe, but rather than
creating each by hand, you'll want to make this a little faster.

### Setup

If you haven't already, [install the Stripe
CLI](https://stripe.com/docs/stripe-cli). It's not required, but it can help to quickly create
[Products](https://stripe.com/docs/api/products/create) and
[Prices](https://stripe.com/docs/api/prices/create).

### Inventory

Due to popular demand, here's a short list of flavors she wants to add:

```
amaretto-almond
cherry
chocolate-hazelnut
cookies-and-cream
espresso-coffee
funfetti-cake
salted-caramel
tiramisu
```

For now, you only sell by the pint. Customers should see a name, description,
image, currency, amount and tax ID.

You decide whether you want each flavor to be the same price or if you want to
charge more for those delicious chunks of cookie, or swirls of caramel. To keep
it easy, assume you'll only sell in one currency, to start.

### Considerations

🧠 Should you have one Product for the pint of ice-cream, then several prices for
each flavor? One Product for each price point? One Product with one Price per
price point? One Product per flavor each with one price for USD? Why?

🧠 How will you handle inventory running low?

🧠 What's a tax ID? Tax behavior? Tax category? How do I enable automatic tax
collection in the dashboard? If I enable tax collection, what changes about the
customer's experience.


### Hints

The tax ID for Food is: `txcd_40040000`. In case you're curious, you can look
that up here: https://stripe.com/docs/tax/tax-codes.


You'll find some `.jpeg` product images for each in the
[`assets/images`](../assets/images) directory.


A public URL for each file looks like:

```
https://github.com/cjavilla-stripe/checkout-workshop/raw/main/assets/images/amaretto-almond.jpeg
```

## Task

Programmatically create ice-cream shop inventory. At the end of this section,
you should have all of the flavors with pricing and image loaded into your
Stripe account.


Ideas:

- Script in your lingua franca
- ["Grab Shell Dude"](https://www.deviantart.com/11011997panic/art/Finding-Nemo-2-897262759) use the Stripe CLI and some sh magic
- Use [Stripe CLI fixtures](https://stripe.com/docs/cli/fixtures)
- Notebooks! 📓


🧠 (Not required, but...) How do you make this idempotent? If you haven't
already seen them, look at those Search endpoints.

🧠 Is it possible to decrease the number of API calls to achieve this?


---

[<- Back to TODO](../TODO.md)
|
[Next 01 Make a website ->](./01-website.md)
