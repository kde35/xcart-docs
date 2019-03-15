---
lang: en
layout: article_with_sidebar
updated_at: '2019-03-14 17:55 +0400'
identifier: ref_168jPT7A
title: VAT and Shipping Charges
order: 150
published: false
---
VAT/GST taxation may include the shipping costs as well as it is part of the service you are providing. The "Value Added Tax / Goods and Services Tax" addon makes it possible to add special VAT rates on delivery options available for customers and display this information at checkout.

Once the "VAT/GST" addon is installed and enabled it adds a possibility to assign special tax classes to shipping methods enabled in the store. By default, there are 2 possible shipping tax classes that can be used to add VAT to shipping rates - **Zero VAT rate** and **Items Max VAT rate**. The difference between these two tax classes is that **Zero VAT rate** class doesn't add VAT to delivery costs while **Items Max VAT rate** adds the VAT rate of the к шиппингу добавляется VAT рассчитываемый по максимальному рейту товаров в текущем заказе

In case you need to apply VAT/GST to shipping complete the following steps:

{% note warning %}
PREREQUISITES:

Make sure the VAT/GST addon {% link "is installed and configured" ref_Rzp45QlN %} and the VAT rates are {% link "set" ref_1uXE2bZt %}.
{% endnote %}

1. Configure delivery options as described in the {% link "Shipping" ref_7tvT7GEK %} section of this manual.

2. Once the shipping methods are created, add a special shipping tax class to them:
   * Locate the **Tax class** column on the Shipping methods settings page (**Store setup** -> **Shipping**):
     ![vat-shipping-tax-classes.png]({{site.baseurl}}/attachments/ref_168jPT7A/vat-shipping-tax-classes.png)

   * Click on a tax class opposite the shipping method name to change the settings:
     * **Low VAT rate** : Choose this tax class if you don't want to add VAT to delivery costs.
     * **Items Max VAT rate** (default value) : Choose this tax class if you need to add a VAT rate to the delivery costs. The VAT rate added to the delivery costs will be calculated as 
       
       {% note info %}
       The options you'll see in the **Tax class** dropdown on the shipping settings page will vary depending on the {% link "Tax Classes" ref_pAWOdG8N %} you've set up in your store. 
       
       Only two abovementioned tax classes can be applied to shipping methods. The rest of the tax classes you see in the list should not be used with shipping methods.
       {% endnote %}
 
 3. Click **Save changes** to activate the settings. 
