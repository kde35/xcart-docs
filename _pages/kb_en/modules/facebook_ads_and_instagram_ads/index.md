---
lang: en
layout: article_with_sidebar
updated_at: '2017-11-16 01:48 +0400'
identifier: ref_LA0TBHEA
title: Facebook Ads and Instagram Ads Module
order: 95
published: true
redirect_from:
  - /modules/facebook_ecommerce/index.html
---

Social feeds are a good point to attract new visitors and boost sales, Facebook Marketing being one of the most popular and efficient. If you have a Facebook account, you can start using X-Cart's free [Facebook Ads and Instagram Ads](https://market.x-cart.com/addons/facebook-e-commerce.html) module (formerly known as "Facebook eCommerce") right away. This module enables you to upload your products to Facebook Catalog and to create personalized ads that will allow reaching the right audience in the right place at the right time. Facebook ads are synchronized with Instagram and are shown there as well even if you don't have an Instagram account.

You can learn more about Instagram ads [here](https://www.facebook.com/business/help/1634705703469129?helpref=faq_content "Facebook eCommerce Module") and [here](https://www.facebook.com/business/help/1513393428972189?helpref=faq_content "Facebook eCommerce Module"). 

If you do not have a Facebook account yet, you can create it at [https://www.facebook.com/business](https://www.facebook.com/business "Facebook eCommerce Module").

The module Facebook Ads and Instagram Ads uploads your products to Facebook Catalog automatically and syncs the product data always keeping the catalog up-to-date. 

To make use of Facebook and Instagram ads, you will need to:
{% toc %}

## Make sure the module Facebook Ads and Instagram Ads is installed and active

Install or activate the module; for help see the section {% link "Managing addons" ref_gTOegEua %} of this manual.
  
  ![xc5_fb_module.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fb_module.png)
  
Once the module has been activated, a new section will become available in your store's Admin area: **Sales Channels** > **Facebook E-Commerce**. 

Also, a new setting - **Add to Facebook product feed** - will be added for each of the products in your store's catalog. You will find it in the Marketing section of the product details page. Note that this setting is enabled by default. All the products with the setting **Add to Facebook product feed** enabled will be added automatically to the product feed and uploaded to your Facebook Catalog.

## Configure the module 

  You can configure the module settings for Facebook Ads and Instagram Ads in the Facebook E-Commerce section of the store's Admin area (**Sales Channels** > **Facebook E-Commerce**). 
  
  ![xc5_fb_module_settings.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fb_module_settings.png)
  
  Note that this section can also be accessed via the **Settings** link in the **My addons** section:
  
  ![xc5_fb_module_settings_link.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fb_module_settings_link.png)
  
  To configure the module, adjust the following settings:
  
  * **Frequency of Product Feed renewal** (hourly/daily/weekly): Specify how often you would like your product feed to be renewed. 
  * **Facebook Pixel ID:** Specify your Facebook Pixel ID. If you do not have a Facebook Pixel ID yet, you can generate it as described at [https://www.facebook.com/business/help/952192354843755](https://www.facebook.com/business/help/952192354843755 "Facebook eCommerce Module"). Facebook Pixel will enable the tracking of such events as _View Content/Search/Add to Cart/Initiate Checkout/Purchase_, and you will be able to get stats on these events to work with sales funnel, ads conversion and so on.
  
  Be sure to save your settings by clicking **Save changes**.
  
  After the settings have been properly adjusted, you can click the **Generate Product Feed** button to get a link for uploading the product feed to your Facebook Catalog.
  
  ![xc5_fecommerce_generate_prod_feed_w_id.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fecommerce_generate_prod_feed_w_id.png)
  
  The system will take some time to generate a Product Feed URL depending on the overall store inventory. Once the process is completed, copy the _Product Feed URL_ that has been generated and paste it into the appropriate field when specifying a source of products for your catalog (https://www.facebook.com/products/catalogs/new).
  
  ![xc5_fecommerce_url_generated.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fecommerce_url_generated.png)
  
  {% note info %}
  The _Frequency of Product Feed renewal_ setting itself will not make renewals automatical. You will need to {% link "configure your server to run scheduled X-Cart tasks" ref_lLqNzAaq %}.
  {% endnote %}
  
## Upload Product Feed to Facebook
  
  To upload your product feed to Facebook:
  
   1. Go to the [Catalog Manager](https://www.facebook.com/business/help/1659534074121655 "Facebook eCommerce Module") of your [Facebook Business account](https://business.facebook.com/overview/ "Facebook eCommerce Module") at https://www.facebook.com/products/.
   
      Click to create a new catalog or choose to edit an exisitng one. 
      ![facebook-catalog.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/facebook-catalog.png)
  
   2. At the step _Add Products to Your Catalog_, specify that you want to _Use Data Feeds_. 
      ![xc5_fb_use_feeds.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/xc5_fb_use_feeds.png)

   3. In the section  **How do you want to upload your data feed?**, choose 'Set a schedule' and paste the Product Feed URL generated for you by X-Cart in the **Data Feed URL** field:
      ![paste-product-feed.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/paste-product-feed.png)
  
   4. Schedule the automatic uploads and name the feed the way you like it better. 
   
   5. Click the **Start Upload** button to upload your products from X-Cart to Facebook.
  
After the products have been uploaded, you will see them on the **Products** tab.
      ![Products.png]({{site.baseurl}}/attachments/ref_LA0TBHEA/Products.png)
  
That's it! You can start advertising your products through Facebook.

_Related pages:_

   * {% link "Sales Channels" ref_ybdJste8 %}
