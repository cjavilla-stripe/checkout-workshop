# 03 Checkout

You, Mamey, and Cherry are starting to have some tough conversations about the
future of the business. Their UXR shows that if we don't ship flavor selection
_this week_ then the business is [default dead](http://www.paulgraham.com/aord.html).


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
