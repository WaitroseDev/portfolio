# PayPal Invoicing & Payments bot
---

## Table of Contents
1. [PayPal Invoicing & Payments bot](#h1-idpaypal-invoicing--payments-bot-1179paypal-invoicing--payments-both1)
2. [Table of Contents](#table-of-contents)
3. [Task:](#task)
4. [Commands:](#commands)
5. [Showcase](#showcase)
   1. [Request a payment using the "pay" command](#request-a-payment-using-the-pay-command)
   2. [What happens after an order is paid for...](#what-happens-after-an-order-is-paid-for)

---

## Task:
* Simplify payments process for clients
* Provide an easy-to-use and fool-proof way for a service provider to invoice their customer
* Create an efficient payment lookup system
* Provide automated payment tracking from end to end

## Commands:
| Command | Usage | Description | Category |
|---|---|---|---|
| newinvoice | newinvoice | Create a new invoice using the inovicing wizard | Invoicing |
| lookup | lookup \<Order Number\> | Lookup the status of an order  | Orders
| pay | pay \<amount> | Create a new order | Orders |
| help | help | Get a list of the bot's commands and command descriptions | System
| ping | ping | Check the API ping time from the host to Discord's servers | System

## Showcase
### Request a payment using the "pay" command
![Creation of a payment](https://waitrose.wtf/lIHvWPJt.gif)

When the user clicks on "Please click here to pay", they are taken to a PayPal checkout page, where they can use any normal PayPal payment method (Balance, Credit/Debit Card/Bank transfer)

### What happens after an order is paid for...
![Post payment completion](https://waitrose.wtf/E0R4rjo7.png)

After payment is complete and automatically confirmed, the bot will send a message to the channel where payment was requested, stating that the Payment is now complete, quoting the Order ID and the total amount of the order.

### Looking up a payment's status...
#### If an payment is not yet complete
![What is shown when a payment is not yet complete](https://waitrose.wtf/tT1vabLe.gif)

As you can see, when a payment is not complete, an embedded message is sent back containing the payment's description and a link to complete the payment. Furthermore, the Amount which is outstanding is also contained in the embed.

#### And when a payment is complete...
![And when a payment has been paid for...](https://waitrose.wtf/yHhN4DNw.gif)

Further to add to the payment lookup command, when looking up a completed payment, the bot will reply with another embedded message which shows that the payment is complete, along with the ID of the person who paid and the date/time of the payment
