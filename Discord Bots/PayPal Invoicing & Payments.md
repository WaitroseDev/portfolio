# PayPal Invoicing & Payments bot
---

## Table of Contents
- [# PayPal Invoicing & Payments bot](#h1-idpaypal-invoicing--payments-bot-1179paypal-invoicing--payments-both1)
- [Table of Contents](#table-of-contents)
- [Task:](#task)
- [Commands:](#commands)
- [Showcase](#showcase)
  - [Request a payment using the "pay" command](#request-a-payment-using-the-pay-command)
  - [What happens after an order is paid for...](#what-happens-after-an-order-is-paid-for)

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