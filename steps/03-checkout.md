# 03 Checkout

You, Mamey, and Cherry are starting to have some tough conversations about the
future of the business. Their UXR shows that if we don't ship flavor selection
_this week_ then the business is [default dead](http://www.paulgraham.com/aord.html).

You know there are a couple options that will not require high PCI compliance
burden: Elements and Checkout.

On one hand, Checkout is marked low-code somewhere in the Stripe docs, which
seems to indicate it would be a bit easier to integrate and maintain.

On the other hand, Elements would allow you to build flavor selection and payment
into the _same_ form. How do we feel about redirecting the customer out to Stripe?

Is it worth the extra dev work to add and maintain Elements, handle errors, manage
PaymentIntent state, coupons, taxes, line items, etc? Or should you offload all of
that to Stripe?


## Actions

Create a Checkout Session with the flavors and quantities and redirect to
Checkout. At the end of this section, customers should be able to pick
order 2 vanilla and 3 chocolate-hazelnut. They'll be charged appropriate
taxes and you'll know where to send the goods.


**Once you're able to redirect**:

- [ ] enable shipping address collection, so you know where to deliver
- [ ] improve your Checkout branding settings (how round or sharp can you make those corners?)
- [ ] enable tax collection
- [ ] enable another payment method
- [ ] make it possible to adjust quantities

🧠 Would you really use Elements or Checkout if this was a real side project,
why or why not? Would the beta Orders API change that decision?

🧠 Can the session be created client-side? server-side?

🧠 Can redirection be done client-side? server-side?

🧠 Is a Stripe [Customer](https://stripe.com/docs/api/customers/create) or
[Guest Customer](https://support.stripe.com/questions/guest-customer-faq)
created? Can you create or find one before redirecting? How can you uniquely
identify a customer? Is there a way to make it easier for the Customer to pay
if they come back again later?

🧠 If you make quantities adjustable in Checkout, how would you ensure a customer
doesn't order more than you have ready to deliver?

🧠 Why would you use `dynamic_tax_rates`, `tax_rates`, or `automatic_tax[enabled]=true`?


---

[<- Back to 02 flavor-selection](./02-flavor-selection.md)
|
[Next 04 Fulfillment ->](./04-fulfillment.md)

[TODO](../TODO.md)
