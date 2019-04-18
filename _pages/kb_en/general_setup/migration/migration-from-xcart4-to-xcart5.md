---
lang: en
layout: article_with_sidebar
updated_at: '2019-04-12 16:26 +0400'
identifier: ref_2h75KMlS
title: ''
order: 100
published: true
---
## Introduction
This article describes how you can upgrade your existing X-Cart 4 store to X-Cart 5.

[General overview of upgrade options on x-cart.com](https://www.x-cart.com/x-cart-migration.html).

Basically, you have three routes:
1. You can perform the upgrade yourself (DIY option);
2. You can hire X-Cart team to perform the upgrade for you (Professional and Custom options);
3. You can hire 3rd party to perform the upgrade for you.

This article assumes you are going for the first option and guides you through the whole process.

{% toc Table Of Contents %}

## What data will be migrated via module

The migration of data is done via our [Data Migration Wizard module](https://market.x-cart.com/addons/migration-wizard.html). Here is what data will be transferred by this module:

<table class="ui compact padded celled small table">
  <tbody>
    <tr class="top aligned">
      <td colspan="1" class="confluenceTd"><span>Сonfiguration settings</span>
      </td>
      <td colspan="1" class="confluenceTd">
- General settings;
<br />- Default customer address; 
<br />- Weight and Length symbols; 
<br />- Purchase limits; 
<br />- Defaut admin/customer language; 
<br />- Ship-from address;          
<br />- Contact Us information. Contact Us form settings are not migrated to X-Cart 5;
<br />- SEO-friendly URLs. Clean URLs are enabled in X-Cart 5 automatically;
<br />
<br />- The currency is NOT transferred and you need to define the currency in X-Cart 5 before the migration.
      </td>
    </tr>
    <tr class="top aligned">
      <td colspan="1" class="confluenceTd"><span>Сontent</span>
      </td>
      <td colspan="1" class="confluenceTd">
- Static pages (Only embedded ones);
<br />- Menu items from Speed bar section.
      </td>
    </tr>
    <tr class="top aligned">
      <td colspan="1" class="confluenceTd"><span>Products</span>
      </td>
      <td colspan="1" class="confluenceTd">
- General info (name, price, sku, etc);
<br />- Images and Detailed images;
<br />- Clean URLs;
<br />- Product options (including product variants and variant images);
<br />- International descriptions;
<br />- Product reviews and votes;
<br />- Related products;
<br />- Wholesale prices (for product variants as well);
<br />- Feature comparison;
<br />- Extra fields. They will be converted to Attributes in X-Cart 5;
<br />- Bestsellers. Bestsellers settings are not migrated to X-Cart 5;
<br />- E-Goods. Only the filepaths are migrated. The files themselves are not transitioned.
      </td>
    </tr>  
    <tr class="top aligned">
      <td colspan="1" class="confluenceTd"><span>Categories</span>
      </td>
      <td colspan="1" class="confluenceTd">
- General info (name, description, etc);
<br />- Images;
<br />- Clean URLs;
<br />- International descriptions;
<br />- Featured products.
      </td>
    </tr>
    <tr class="top aligned">   
      <td colspan="1" class="confluenceTd"><span>Users</span>
      </td>
      <td colspan="1" class="confluenceTd">
All info;
<br />
<br />How to transfer user passwords:
<br />- If you are migrating from X-Cart 4.1.x-4.4.x, you need to specify blowfish key on Hence all user passwords are migrated safely providing that a valid Blowfish key is specified at the <a href="https://kb.x-cart.com/modules/xc4_to_xc5_migration_wizard/using_the_xc4_to_xc5_migration_wizard.html#step-2---connect" target="_blank">Step 2 - Connect</a> of the migration wizard and passwords will be transferred properly;
<br />- If you are migrating from X-Cart 4.5.x and later, passwords will not work after the migration. In order to allow customers log in using old passwords, you need to install [Migration: Restore logins of X-Cart 4 users module](https://market.x-cart.com/addons/xcart-4-login.html) from the marketplace and specify X-Cart 4 blowfish key inside its settings.
      </td>
    </tr>
    <tr class="top aligned">   
      <td colspan="1" class="confluenceTd"><span>Memberships</span>
      </td>
      <td colspan="1" class="confluenceTd">
All info including multilanguage data.
      </td>
    </tr>
    <tr class="top aligned">   
      <td colspan="1" class="confluenceTd"><span>Zones</span>
      </td>
      <td colspan="1" class="confluenceTd">
All info.
      </td>
    </tr>
    <tr class="top aligned">
      <td colspan="1" class="confluenceTd"><span>Payment settings</span>
      </td>
      <td colspan="1" class="confluenceTd">  
Settings of the following methods are transferred:
<br />- AuthorizeNet;
<br />- EWay;
<br />- Moneybookers;
<br />- PayPal (Standard, Express Checkout, Payflow Link, Payflow Transparent Redirect, Paypal Advanced, Paypal WPS);
<br />- 2Checkout.
      </td>
    </tr>
    <tr class="top aligned">
      <td colspan="1" class="confluenceTd"><span>Shipping settings</span>
      </td>
      <td colspan="1" class="confluenceTd">
User defined shipping methods and rates;
<br />Settings of the following real-time shipping processors:
<br />- Australia Post;
<br />- Canada Post;
<br />- DHL;
<br />- FedEx;
<br />- USPS;
Settings of UPS are not migrated.        
      </td>
    </tr>
    <tr class="top aligned">
      <td colspan="1" class="confluenceTd"><span>Orders</span>
      </td>
      <td colspan="1" class="confluenceTd">
All info.
      </td>
     </tr> 
  </tbody>
</table>