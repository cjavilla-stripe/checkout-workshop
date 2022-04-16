# 04 Fulfillment

You, Mamey, and Cherry are on a rocket ship 🚀. All of the lines are up and to
the right 📈.

The scrapy startup system where Mamey and Cherry depend on the [Slack
integration with Stripe](https://stripe.slack.com/apps/A0F81FNVC-stripe) to
know about new orders isn't scaling well. Furthermore, now that customers can
pick multiple flavors, fulfillment is getting chaotic.

Also, after chatting with Chip, you learn that it would be more efficient
from a delivery perspective to have a collection of several orders from the
same zip code made in the same hour. That way he can dispatch a freezer truck
with several drones to one location to make multiple deliveries at once.

Cherry also posted an idea in the #what-if channel a few weeks ago:

> What if we could deliver locally via drone and nationally in affordable
> ice-chests with dry ice?

You decide it's time to build your own fulfillment system.

### Actions

Set up a webhook handler to know when a customer successfully pays for a new
order. By the end of this section, you should have a webhook handler that
prints an order summary including:

- customer email
- customer phone
- list of flavor X quantity


🧠 Checkout supports limiting shipping by country, how would you limit just to
Ashville? If you collect the address before redirecting to Checkout is there a
way to make sure the customer doesn't _change_ the shipping address?

🧠 How would you collect the hourly orders by zip code to help Chip?

🧠 How would you separate out the orders that are sent nationally vs. locally?

🧠 Is there a way to offer the customer sevaral options for them to choose the
cost related with shipping nationally? How would you go about showing those only
when the delivery will be national and not local?



---

[<- Back to 03 checkout](./03-checkout.md)
|
[Next 05 Gifting 🎁 ->](./05-gifts.md)

[TODO](../TODO.md)
