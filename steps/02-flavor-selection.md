# 02 Flavor selection

Customers love to identify with a specific flavor of ice-cream. "I'm a rocky
road kinda gal." says one of the regulars. "I'm a funfetti kinda kid" says our
neighbor. They want variety!

When starting out in beta, you didn't even have a website, so we kept it simple
and used PaymentLinks. It's killing Cherry and my sister that customer's can't
pick more flavors, tho.

There's a jira ticket sitting in my inbox to add "flavor selection" to the site.

(Who am I kidding, we can't afford jira yet, it's just a text from my
sister, but damn it feels like a jira ticket.)


## Actions

Update our UI so that we keep track of several requested flavors 🍨 in a "box."

Ideas for storing cart state:

* cookies
* localStorage
* a database
* metadata on a Stripe Customer object

Change that button from "Pay" to "Add to cart"

```html
<a href="#" class="add-to-cart relative flex bg-gray-100 border border-transparent rounded-md py-2 px-8 items-center justify-center text-sm font-medium text-gray-900 hover:bg-gray-200">Add to cart</a>
```

I would use data-* attributes to track what needed for redirecting to checkout.
(cough, price ID, cough). But feel free to use whatever you're most comfortable
with.


🧠 What was the difficulty level for implementing cart logic? What ideas do you
have for the product team about how to make this easier?

🧠 What are the tradeoffs in the approaches for storing cart state?

---

[<- Back to 01 website!](./01-website.md)
|
[Next O3 Shipping ->](./03-shipping.md)

[TODO](../TODO.md)
