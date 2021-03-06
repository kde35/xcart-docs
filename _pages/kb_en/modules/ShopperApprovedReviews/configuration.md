---
lang: en
layout: article_with_sidebar
updated_at: '2018-04-23 14:48 +0400'
identifier: ref_3otm3RBq
title: Configuring the Shopper Approved Reviews Addon
order: 100
published: true
redirect_from:
  - /modules/ShopperApproved/configuration.html
---
You can find out whether your X-Cart store has the addon Shopper Approved Reviews installed and enabled by checking the **My addons** section of your store Admin area. If not, the addon can be obtained via the X-Cart App Store.
![shopperapproved_addon.png]({{site.baseurl}}/attachments/ref_3otm3RBq/shopperapproved_addon.png)

To install the addon, follow the steps described in {% link "Installing Addons from the X-Cart App Store" ref_Vn1mMUw9 %}.

Before you start using the addon, you need to adjust the addon settings. Proceed to the Shopper Approved Reviews addon settings page: 
![settings.png]({{site.baseurl}}/attachments/ref_3otm3RBq/settings.png)

There you will be prompted to either sign up for Shopper Approved or to connect manually with your existing Shopper Approved account.
![settings-page.png]({{site.baseurl}}/attachments/ref_3otm3RBq/settings-page.png)

If you do not have a Shopper Approved account yet, you can hit **Sign Up**, and the system will automatically create a Shopper Approved account for you and link your X-Cart store to it. Please note, however, that in this case your credentials for access to the Shopper Approved dashboard will be sent to your main Site administrator email address as configured via the **Site administrator e-mails** setting in the Contact information section (**Store setup** -> **Contact information**) of your X-Cart store Admin area. Make sure this setting {% link "has been adjusted properly" ref_wKcxbiUf %}; otherwise you will not be able to get your Shopper Approved dashboard credentials.

If you have an existing Shopper Approved account, you can connect it to your X-Cart store by hitting the button **'Connect with existing account'** and providing the required connection information manually.
![settings-filled.png]({{site.baseurl}}/attachments/ref_3otm3RBq/settings-filled.png)

You will need to specify the following information:

   * **ShopperApproved Site ID**: Get this info in the ShopperApproved Dashboard -> [User Info section](https://www.shopperapproved.com/account/dashboard/userinfo/account-settings "Configuring the Shopper Approved") 
   * **ShopperApproved API Token**: Get this info in the ShopperApproved Dashboard -> [User Info section](https://www.shopperapproved.com/account/dashboard/userinfo/account-settings "Configuring the Shopper Approved") 
   * **ShopperApproved Site Domain**: Enter your X-Cart store URL; for example, myxcartstore.com

Once enabled, the Shopper Approved Reviews addon creates a static page titled _Read our reviews_; that page is aimed at promoting verified reviews you gain through the Shopper Approved addon. You can customize it to your liking in the **Content** -> **Pages** section of the Admin area or add the merchant reviews widget to any other static page. The _Read our reviews_ static page may appear empty until you receive your first reviews and approve them via the Shopper Approved dashboard.

Further addon setup can be done in the Shopper Approved section (**Content** -> **Shopper Approved**) of your X-Cart store Admin area.
![product_category_pages.png]({{site.baseurl}}/attachments/ref_3otm3RBq/product_category_pages.png)

This section provides two tabs:
   * Product and Category pages;
   * Merchant Review Survey.

On the Product and Category pages tab, you can configure the following settings:
* **Use Shopper Approved widget instead of the default one**: If this option is enabled, the widget will display the reviews submitted via the Shopper Approved addon only; any reviews submitted earlier will not be available to customers.
* **Star size**: Regular/Big
* **Maximum number of reviews to display**: Specify the number of reviews you require (from 3 to 20).
* **Date format**: Select the date format you require. 

More settings affecting the reviews on your store's product and category pages can be found in the **Product** -> **Code** section of your [ShopperApproved dashboard](https://www.shopperapproved.com/account/product/page-code) at “Step 2. Select Your Options”.
![code-step2.png]({{site.baseurl}}/attachments/ref_3otm3RBq/code-step2.png)

The Merchant Review Survey tab of the Shopper Approved section of your X-Cart store Admin area enables you to control the options pertaining to a brief survey which can be added onto the thank you page for your customers. Depending on your business needs, the survey can be enabled or disabled. It is also possible to specify whether comments should be mandatory. 

More survey related settings can be found in the **Merchant** -> **Surveys** section of your [ShopperApproved dashboard](https://www.shopperapproved.com/account/merchant/surveys/options) (For example, you can specify in how many days after a customer completed checkout at your store a followup email with a link to the survey should be sent to them).
![survey.png]({{site.baseurl}}/attachments/ref_3otm3RBq/survey.png)

Since ShopperApproved uses the {% link "Google feed" ref_2gQBB6qM %} data format, you will need to install and enable the Google Product Feed addon and generate a data feed using it. The data feed will be automatically imported to ShopperApproved, and you will be able to find a link to it in the **Dashboard** -> **Product** -> **Integration** section at [ShopperApproved](https://www.shopperapproved.com/account/product/integration "Configuring the Shopper Approved"). 

![sa-data-feed.png]({{site.baseurl}}/attachments/ref_3otm3RBq/sa-data-feed.png)

Once the Google data feed has been submitted to ShopperApproved, your product reviews should become available in the [ShopperApproved dashboard](https://www.shopperapproved.com/account/dashboard) where you will be able manage them further.
![Dashboard.png]({{site.baseurl}}/attachments/ref_3otm3RBq/Dashboard.png)

The reviews will be updated automatically every time you re-generate the Google feed in X-Cart.

Provided that a customer survey has been enabled via the addon settings, after placing an order at your X-Cart store, your customers will be prompted to provide feedback. They will see a pop-up screen where they will be able to rate their customer experience and answer the survey questions:
![checkout-popup.png]({{site.baseurl}}/attachments/ref_3otm3RBq/checkout-popup.png)
