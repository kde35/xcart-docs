---
lang: en
layout: article_with_sidebar
updated_at: '2018-01-26 13:35 +0400'
identifier: ref_5TMbPwNQ
title: Not Finished Orders
order: 100
published: true
description: not finished orders module
redirect_from:
  - /orders/not_finished_orders.html
---
When a buyer completes a payment process with a payment gateway and clicks _**Place Order**_  his cart in X-Cart front-end is cleared and the admin back-end registers an order for this buyer being an exact copy of the cart at the moment of payment.  Sometimes it can be that a buyer proceeds to paying a cart but doesn't complete it due to many reasons (a customer changes his mind, something distracts a customer from the payment, a computer crash, etc.). In this case the cart admin back-end doesn't register an order and if a merchant wants to have such not finished purchases registered it's necessary to use the **Not Finished Orders module** in X-Cart. This module is included in the Business edition and higher and can be {% link "enabled" ref_0fGEpvrh %} in the **My Addons** section of the cart admin back-end.

{% note info %}
The **Not Finished Orders** module works with the orders created with online payment processors. For the offline payment methods an order is created at the moment a buyer clicks the **Place order** button in the X-Cart front-end and an order gets an "Awaiting payment" status by default. 
{% endnote %}

To set up the **Not Finished Orders** module use the _Settings_ link.

![payment-transactions.png]({{site.baseurl}}/attachments/ref_5TMbPwNQ/payment-transactions.png)

The settings of the module are as follows:

* **Not finished order will be created** : Choose the conditions that if met will result in a not finished order creation.

* **Clear cart if administrator changes order** : Enable if you need a customer's cart to be cleared in the front-end once the corresponding order is changed by the store admin in the admin back-end.

{% note info %}
If this option is set to 'YES' a buyer's cart of a not finished order will be cleared as soon as the cart admin changes the order details, e.g. a payment status of a not finished order from _Status is not defined_ to _Awaiting payment_. By default the cart content is cleared only when an order is placed.  
{% endnote %}

* **Limit lifetime of not finished order** : If enabled, the cart admin will be able to define the the time to use the cart at its current state for future attempts in days. 

Once enabled and set up, the cart admin will see the not finished orders in the **Orders** section of the admin back-end.

![order.png]({{site.baseurl}}/attachments/ref_5TMbPwNQ/order.png)

A not finished order won't have an order number and the payment status will be _Status is not defined_. The order will get an orderID only when and if the cart admin changes the fulfilment status and payment status of the order.

The **Not Finished Orders** module is good for manual tracking of the purchases. If you want to automate the procedure use the {% link "Abandoned Cart Reminder" ref_Mf6yeSBE %} module. It works with any abandoned cart regardless of the payment method.
