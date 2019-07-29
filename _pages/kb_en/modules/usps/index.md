---
lang: en
layout: article_with_sidebar
updated_at: '2018-12-17 11:32 +0400'
identifier: ref_158tuAaD
title: U.S.P.S.
order: 320
published: true
redirect_from:
  - /modules/u.s.p.s.html
  - /modules/usps.html
---
X-Cart is integrated with U.S.P.S. carrier services via the [U.S.P.S. addon](https://market.x-cart.com/addons/usps.html "U.S.P.S.") and can communicate with USPS API in two possible ways to retrieve shipping rates:

1. Direct connection with USPS Web Tools Ecommerce APIs to retrieve the list of available U.S.P.S. delivery methods and calculate the rates charged for shipping ordered items to international customers and customers within the United States.

   {% note info %}
   The addon calculates rates for orders shipped from the United States only. You just need to enter your USPS credentials to start using it.
   {% endnote %}

2. USPS via Pitney Bowes API (X-Cart 5.3.3 and later)

   With the X-Cart Pitney Bowes integration you get:
   - competitive, discounted USPS pricing (savings up to 20% on retail USPS rates and up to 49% on the other major carriers); 
   - automatic address verification;
   - daily shipping manifests to speed carrier processing;
   - a possibility to print shipping labels with ease and track USPS shipments from origin to delivery;
   - a possibility to identify USPS shipping services cost and estimated delivery time;
   - a possibility to manage refunds and cancellations.
   

To start using the U.S.P.S. addon, you need to make sure it is installed and enabled. General addon installation instructions are available in the section {% link "Installing Addons from the X-Cart App Store" ref_Vn1mMUw9 %}. 
   
   *  {% link "U.S.P.S. General Configuration" ref_whrpZnV3 %}
   *  {% link "U.S.P.S. Shipments via Pitney Bowes" ref_0TwynAXE %}
