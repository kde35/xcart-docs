---
lang: en
layout: article_with_sidebar
updated_at: '2018-02-05 13:14 +0400'
identifier: ref_2LetICls
title: Shop by Brand
order: 245
published: true
description: shop by brand
---
[Shop by Brand](https://market.x-cart.com/addons/shop-by-brand.html "Shop by Brand") addon is included in X-Cart Ultimate edition (paid for X-Cart Business). The addon is aimed at promoting branded goods.

With this addon finding products of specific brands/manufacturers becomes much easier to customers. Especially to first-time visitors who don't know what exactly they are looking for.

To install the addon  please follow the steps described in {% link "Installing and activating addons" ref_0fGEpvrh %}.

Once installed, find the addon in the list of installed modules on the Addons page in the admin back-end, open the addon settings page and configure the addon according to your business needs.

![addon.png]({{site.baseurl}}/attachments/ref_2LetICls/addon.png)

The addon settings are as follows:

![settings.png]({{site.baseurl}}/attachments/ref_2LetICls/settings.png)

{:.ui.compact.celled.small.padded.table} 

| Which global attribute field is the product brand? | Here you can choose brands from the global attributes available. If you have no global attributes, please, {% link "configure" ref_HzMkgc0q %} them first. |
| Order brands on the Brands page by | Choose between "Brand names", "Admin-defined order" and "Number of products". |
| Enable pagination on the Brands page | Should be enabled only if you have a great deal of brands in the store. |
| Default number of brands per page | The number of brands to be displayed on the Brands page on the store front-end. |
| Show the Brands block on the home page | If enabled the Brands block will be displayed on the home page. |
| Order brands in the Brands block by | Choose between "Brand names", "Admin-defined order" and "Number of products". |
| Number of items in the Brands block |Set the number of brands to be displayed in the Brands block on the store front-end. |

Don't forget to **Submit** changes when done.

When the addon is enabled and configured, existing brands are collected through the store automatically based on the global attribute you specified and are displayed in the _Brands_ section (**Catalog** > **Brands**) in the admin back-end. 

![brands.png]({{site.baseurl}}/attachments/ref_2LetICls/brands.png)

Here the cart admin can change the order of appearance of the brands the way he needs. By default, the brands are sorted alphabetically. Also, it's possible to edit the existing brands and add new ones if required. 

To create a new brand click the **New brand** button, to edit an existing brand click the brand name in the list. The procedure is similar, in both cases you'll need to feel in the fields with the info and save the changes.

You can specify the following info for your brands, the only required filed being the brand name:
* **Brand name**: Use this field to specify or edit the brand name here.
* **Brand logo** : Use this field to upload a brand logo here (you can do it either via a URL or directly from your computer).
* **Description** : A brand description that will be displayed on the brand's page.
* **Meta keywords** : The keywords to be used in the keywords META tag on the category page (for SEO purposes).
* **Meta description** : The description to be used in the description META tag on the category page (for SEO purposes).
* **Clean URL** : The product page Clean URL (for SEO purposes).

The buyers will see the Brands block on the home page and on any category page on the store front-end. You can change the Brands block location using the [Webmaster mode](https://devs.x-cart.com/webinars_and_video_tutorials/using_webmaster_mode_in_x-cart_5.html "Shop by Brand"). The brands are also added to the store main {% link "menu" ref_BDykFBbw %}. If you want to disable the brands menu you can do it in the **Content** > **Menus** section of the store admin back-end.

![home.png]({{site.baseurl}}/attachments/ref_2LetICls/home.png)

The Brands block on the store front-end displays only the brands that have products that are in stock. If you want to show the brands with the out-of-stock products, please, enable the "Show all" option for the '_How to show out of stock products_' field in the {% link "Customer Zone settings" ref_qAZlJxZm %} (**Store setup** > **Cart & Checkout**). The brands that have no products assigned to them won't be displayed ever.

![general.png]({{site.baseurl}}/attachments/ref_2LetICls/general.png)

{% note warning %}
Enabling the "Show all" option for the '_How to show out of stock products_' field in the {% link "Customer Zone settings" ref_qAZlJxZm %} (**Store setup** > **Cart & Checkout**) will display the out-of-stock products throughout the whole store.
{% endnote %}
