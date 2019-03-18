---
lang: en
layout: article_with_sidebar
updated_at: '2019-03-14 17:55 +0400'
identifier: ref_168jPT7A
title: Setting VAT on Shipping Charges
order: 150
published: true
---
VAT/GST taxation may include the shipping costs as well as it is part of the service you are providing. The {% link "Value Added Tax / Goods and Services Tax  addon" ref_0GjdgNJx %} makes it possible to add special VAT rates on delivery options available for customers and display this information at checkout.

Once the "VAT/GST" addon is installed and enabled it adds a possibility to assign special tax classes to shipping methods enabled in the store to add VAT to the delivery costs. By default, all delivery costs are VAT-exclusive.

There are 2 defaut shipping tax classes that can be used to add VAT to shipping rates - **Zero VAT rate** and **Items Max VAT rate**. The difference between these two tax classes is that **Zero VAT rate** class doesn't add VAT to delivery costs while **Items Max VAT rate** do. The VAT rate added to the delivery costs by the **Items Max VAT rate** tax class equals the maximum VAT rate set on the products being added to cart. 

For example, there are 2 products in the cart - Product 1 at the cost of £100 (VAT 20% included, i.e. price £83.33 + VAT £16,67) and Product 2 at the cost of $100 (VAT 5% included, i.e. price £95,24 + VAT £4,76). In case **Items Max VAT rate** tax class is applied to the delivery method chosen by a customer, the VAT 20% rate will be added to the shipping costs and included into the total amount of VAT 20% displayed to a customer.

![vat-shipping-checkout.png]({{site.baseurl}}/attachments/ref_168jPT7A/vat-shipping-checkout.png)

In order to apply VAT/GST taxation to shipping complete the following steps:

{% note warning %}
PREREQUISITES:

Make sure the VAT/GST addon {% link "is installed and configured" ref_Rzp45QlN %} and the VAT rates are {% link "set" ref_1uXE2bZt %}.
{% endnote %}

1. Configure delivery options as described in the {% link "Shipping" ref_7tvT7GEK %} section of this manual.

2. Once the shipping methods are configured, add a special shipping tax class to them:
   * Locate the **Tax class** column on the Shipping methods settings page (**Store setup** -> **Shipping**):
     ![vat-shipping-tax-classes.png]({{site.baseurl}}/attachments/ref_168jPT7A/vat-shipping-tax-classes.png)

   * Click on a tax class opposite the shipping method name to change the settings:
     {% note info %}
     The options you'll see in the **Tax class** dropdown on the shipping settings page will vary depending on the {% link "Tax Classes" ref_pAWOdG8N %} you've set up in your store. 
     You can choose any tax class with the configured VAT rate and apply it to shipping.
     {% endnote %}
       
     * **Zero VAT rate** : Choose this tax class if you don't want to charge VAT on delivery costs.
     * **Items Max VAT rate** (default value) : Choose this tax class if you need to charge VAT on delivery costs. A VAT rate added to the delivery costs will equal the maximun VAT rate set on the products being added to cart. 
     *  **Any other tax class from the list** : Choose a tax class with a configured VAT rate if you need to charge VAT on delivery costs. A VAT rate added to the delivery costs will depend on the VAT rate set for the tax class you've chosen. 
       
3. Click **Save changes** to activate the settings.
