# 01 Build a website!

Your startup's ice-cream is super fresh and your website should be just as fresh 🍉.

Spin up a basic website and use
[this](https://gist.github.com/cjavilla-stripe/37347c9a3413ad1dd7c6d476fe8fd862)
(or something like it) as your landing page.


Take a look around, checkout the medicine cabinets, see if there are any spots
on the silverware 🥄. Feel free to tweak a bit to make it your own.

For now, we'll just keep using Payment Links on each product, but Cherry isn't going to
be okay with this for long. We learned at work that we can do this thing called
"fast follow" after GA, so we'll just tell Cherry that.


### Actions

Set up your page so that it fetches the flavors from inventory. At the end of
this section you should have a simple index page rendering all of the flavors.
No need to actually implement Checkout, yet. Feel free to start from a Stripe
Sample to save time: `stripe samples create accept-a-payment` then follow the
pre-built flow.


Ideas:

* Pull from the Stripe API
* Hard code some client side JSON
* Retrieve from a database and use SSR
* Render back JSON from a server side endpoint


🧠 What are the tradeoffs with each of those approaches? What data do you
_really_ need for display? What about data required for ultimately [creating the
Checkout Session](https://stripe.com/docs/api/checkout/sessions/create)?


---

[<- Back to 00 Add products](./00-add-products.md)
|
[Next 02 Flavor selection ->](./02-flavor-selection.md)


[TODO](../TODO.md)
