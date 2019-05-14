---
lang: en
layout: article_with_sidebar
updated_at: '2017-09-01 01:22 +0400'
identifier: ref_7tvT7GEK
title: Shipping
categories:
  - home
order: 50
icon: shipping
description: Learn about shipping calculation and configure shipping methods for your store
published: true
---
Once an order has been paid for, you will need to deliver the ordered goods to the buyer. Unless those are products that do not require shipping (like {% link "digital goods" ref_lxNH6TFr %}, {% link "bookable products" ref_4IYL2Shf %} or {% link "PIN codes" ref_4JeE99n8 %}), you will have to arrange the packaging, pickup and delivery. 

{% note info %}
The topic of shipping configuration for products that do not require shipping is covered in the section {% link "Shipping Setup for Products That Do Not Require Shipping" ref_z5KmbFAu %}.
{% endnote %}

Depending on your business scope and the distance between your warehouse and the buyer's location, you will either have to deliver the goods to the buyer on your own or will have to use the services of a shipping company that will deliver the goods on your behalf. Considering all the costs associated with getting an order to the buyer - including the cost of packaging, shipping, tracking, insurance and customs/duties (if you cover them) - you may find shipping to be a major expense in your business. To keep things profitable, you will need to come up with an effective shipping strategy. 

First of all, it is a good idea to know the weight and size of every product you sell. This will give you an idea of what shipping methods and what type of packaging will have to be used for them as well as give you a good sense of your total costs. You will be able to specify the weight and dimensions for every product in your X-Cart store catalog for accurate shipping cost estimation. For products that need to be shipped separately from others, you will be able to set this option and specify the package dimensions required. 

Some key decisions will have to be made regarding your pricing strategy for shipping. Some popular options here are as follows:
     
   * **Charge Actual Carrier Rates**
     If you ship products using a third-party postal or delivery service, you can charge your customers the exact rates you pay to ship their order. X-Cart is integrated with a number of real-time shipping carriers - like UPS, USPS, FedEx, Royal Mail or Canada Post - which can calculate the shipping rates in real time based on the order weight, parcel dimensions, and delivery address. The available shipping options and live pricing provided by such carriers are shown at checkout so your customers can choose and pay for the exact service they want.

     If you are a small company that does its own delivery, or if your shipping carrier is not integrated with X-Cart to provide real-time shipping rate estimation, you may want to consider providing your own custom rate table with shipping rates based on the order weight, subtotal, number of items in the order, or any combination thereof.

     You can even combine the two approaches, if required, by providing some shipping methods with real-time calculated rates and shipping methods with table-based non real-time rates at the same time. 

     For more information, see:
     * {% link "Carrier-calculated Shipping Rates" ref_ybdiN8r0 %}
     * {% link "Custom Table Rates" ref_3TG6AuN0 %}
   
   * **Charge a Flat Rate**
     Another polular option is to charge buyers a fixed (flat) rate. X-Cart can be configured to use a flat rate per order or a flat rate per item.
     
     For more information, see:
     * {% link "Custom Table Rates" ref_3TG6AuN0 %}
     * {% link "Shipping Freight" ref_kioKBJIM %}
     
   * **Offer Free Shipping**
     Free shipping is a feature appreciated by most shoppers. It not only helps reduce shopping cart abandonment, but also encourages your customers to spend more. You can offer free shipping on specific products, on all orders, or on orders that meet certain conditions (for example, "free shipping on oders over $50"). You can also give specific customers a free shipping coupon. 
     
     For details, see:
     * {% link "Free Shipping" ref_BCq5l4MP %}
   
   * **Enable Local Pickup**
      If you wish to enable your local customers to pick up the order themselves, you can do so by enabling the Local pickup shipping method.

If, on top of regular shipping cost, you need to cover some additional expenses, like the cost of handling of a particularly heavy item, you can add a **handling fee**. For more information on this, see:

     * {% link "Handling Fee" ref_nFJTxPMR %}

It is also a good idea to consider the question of **labelling** your packaged orderes.

     * {% link "Shipping Labels " ref_7p59HzrS %}     

Note that your strategy might change as your business grows. It is never a bad idea to reevaluate your original decisions to ensure that you are delivering the absolute best possible service and experience for the best possible price to your customers. X-Cart offers flexible shipping settings, so should you decide to change your shipping strategy, you will be able to adjust your store's shipping configuration at any time to meet your business needs.

Do not forget about taxes. Tax regulations vary for different countries and states, so you will need to check with your local authorities whether you need to charge **tax on shipping**. If you do, you will need to configure your X-Cart store to charge tax on delivery costs. 
For more info on this, see:
     * {% link "Shipping Tax" ref_4nZM0iOX %}
     
     
_In this section:_

*   {% link "Carrier-calculated Shipping Rates" ref_ybdiN8r0 %}
*   {% link "Custom Table Rates" ref_3TG6AuN0 %}
*   {% link "Free Shipping" ref_BCq5l4MP %}
*   {% link "Shipping Freight" ref_kioKBJIM %}
*   {% link "Handling Fee" ref_nFJTxPMR %}
*   {% link "Shipping Labels " ref_7p59HzrS %}
*   {% link "Shipping Tax" ref_4nZM0iOX %}
*   {% link "Shipping Setup for Downloadable Products" ref_z5KmbFAu %}
