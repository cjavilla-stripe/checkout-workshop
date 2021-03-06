# 07 Subscription

Business is going so well that Chip and Cherry are on a fieldtrip today with a
commercial realestate agent. They are looking for new warehouse space with a
massive industrial kitchen.

Ideally, a little closer to a bigger city, but far enough from major Airports
that Chip can still use his cottage drone delivery license from the FAA to make
lots of quick local ice-cream drops.

I was chatting with a regular, Lemon
the other day and had an idea. Lemon hosts a dinner party once per month and
she always provides several flavors for her guests. She asked if we would just
automatically charge her each month for 2 of each flavor and send her a box.

I started thinking about how we might automate this, but to start, I just created
a google calendar event "Make JoAnne's order (2xflavor)" that repeated each month.

This was a pain tho, because each month, I had to go into the Stripe Dashboard,
create a new custom charge, and that didn't track all of the same line items for the
flavors. It was really throwing off our reporting.

### Actions

Add support for subscribing to an ice-cream box on a monthly, or weekly basis.
You should know when customers subscribe and when they cancel, you should also
know if they change their selection or flavor preferences. And be able to
print orders when they are ready.


🧠 How will you support both one time and recurring orders? Still support
gifting?

🧠 How should you model products and prices?

🧠 How will you enable customers to manage their subscription (think cancel,
change frequency)?

🧠 How will you test your logic and that it is renewing successfully one week
in the future?

🧠  What `metadata` would come in handy to have on the Subscription object?
What about on the Checkout Session?


---

[<- Back to 06 Authentication](./06-authentication.md)
|
[Next 08 Customer portal ->](./08-customer-portal.md)

[TODO](../TODO.md)
