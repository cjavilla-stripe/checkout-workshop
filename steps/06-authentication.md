# 06 Authentication

Support volume around gifts died down, thankfully! You decide to retroactively
create an `OKR: Drive down support volume for #1 ask "gifts"` and send an org wide
shipped email (to all 4 employees). 😎

That was fun, so you turn back to the support queue and try to find a theme for #2.

Since Airborn Treats flavors are so zaney, we get a lot of questions from customers
who don't recall the exact flavors they ordered last time. They want to re-order
but they can't see past orders. Inbound emails like:

> I couldn't figure out how to login. Where can I see my past orders?

> Can you just send me the same order I had last time?

> Last month, I had the most delightful fruity ice-cream from Airborne Treats.
> Can you tell me what I ordered?

🤔 I guess we need a way for customers to log-in and see their past orders.


### Actions

Add customer authentication so that returning customers can login and see their past
orders. Feel free to take short cuts to keep the time to about 20 min for implementation.

Ideas for shortcuts:

- Store the customer ID in a cookie
- Store the customer ID in localStorage
- Magic link login
- Assume the email is both the email and password
- Simple email / password auth


🧠 How do we associate all of the past orders to a single user?

🧠 How should we display those to the customer? How about the Customer portal?

🧠 If we're not already creating a Stripe customer, when and how should we do that?


---

[<- Back to 05 Gifts](./05-gifts.md)
|
[Next O7 Subscription ->](./07-subscription.md)

[TODO](../TODO.md)


