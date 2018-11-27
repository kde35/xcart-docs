---
lang: en
layout: article_with_sidebar
updated_at: '2018-09-04 10:52 +0400'
identifier: ref_3rhs1MJ8
title: Block Users by IP / Country / User agent
order: 41
published: true
---
The X-Cart module [Block Users by IP/Country/User Agent](https://market.x-cart.com/addons/block-users-by-IP-country-user-agent.html "Block Users by IP / Country / User agent") protects your store from bots and fraudulent users by limiting or completely restricting access to it with the help of flexible settings and filters taking into account the user IP, address and behavior.

{% toc %}

To install the module, follow the guidelines from the section {% link "Installing addons from the Marketplace" ref_Vn1mMUw9 %}.

## Installation and Set-up

After the module has been installed, proceed to the module settings page to configure it:

![buip-installed.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-installed.png)

The **Block Users by IP/Country/User Agent module settings page** includes 3 subsections:

1. IP based access control:
   ![buip-settings-1.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-settings-1.png)
   * **Access control mode** : Select between "Allow access from all but blacklisted IP addresses" and "Allow access from IP addresses in white list". 
     {% note info %}
     The first option will allow access to the store from any IP address except for those that are in the blacklist and will work even if there are no IP addresses in the back list. 
     
     The second option will allow access to the store only from IP addresses that are in the white list and will NOT work if there is no white list with IP addresses (i.e. you have to create a white list with IP addresses in the **Store setup** -> **Access filters** section to use this mode).
     {% endnote %}
   * **Link to bypass the IP based access control system** : Is generated automatiocally

2. Bot protection:
   ![buip-settings-2.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-settings-2.png)
   * **A visitor should be identified as a bot if** : Specify the corresponding time/pages paramethers.
   * **A visitor should be identified as a bot if the length of period between add to cart action and an attempt to buy is less than** : Specify the period in seconds.
     {% note info %}
     The time and pages values for the above settings are to be found out empirically as they differ depending on a particular site, server environment, etc.
     {% endnote %}
   * **Allow bots to make purchases** : Toggle the setting off if you don't want bots to make purchases in your store.
   * **Detect search engine bots via the user agent** : With this option enabled any visitor of a "crawler" type according to [https://browscap.org/](https://browscap.org/ "Block Users by IP / Country / User agent") is automatically blacklisted. 
     {% note info %}
     If this option is disabled the module will sort the visitors in accordance with the **A visitor should be identified as a bot if** and **A visitor should be identified as a bot if the length of period between add to cart action and an attempt to buy is less than** settings.
     {% endnote %}
   * **Add bot IP addresses to black list** : Decide if you want to add bot IP addresses to back list automatically or not and select one of the options.  
     {% note info %}
     When making a choice please keep in mind that any option starting with "Forbid ..." automatiocally adds any bot IP address (both good bots that help in creating the required visibility of the websites on the internet, and bad bots that are programmed to perform a variety of malicious jobs) to the black list and limits access to the store pages from the blacklisted IP  depending on the option you selected. 
     
     If you set the value to "Forbid access to entire site" the site will become inaccessible to all possible bots and as a result the site will NOT not be indexed by good bots as well.
     {% endnote %}

3. Address based protection:
   ![buip-settings-3.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-settings-3.png)
   * **Restrict purchases based on buyer address** : Select if you want to restrict purchases for buyers with a different billing and shipping address.
   * **Restrict purchases based on buyer location** : Select if you want to restrict purchases for buyers whose billing address doesn't match the IP address they used for the purchase.

Don't forget to **submit** the changes to make them active.

## Access Filters

When the module configuration is complete you can proceed to creating access filters if required. 

For this purpose:
1. Open the **Store setup** -> **Access filter** section in the admin area and click 'Create':
   ![buip-access-filters-create.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-access-filters-create.png)
2. You will be redirected to a new page where you can create an access filter based on the set of options available:
   ![buip-new-filter.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-new-filter.png)
   * **Condition type** : Select a condition type to distinguish a user (IP address, IP address mask, IP address country, User agent). Depending on the type you'll be able to specify: 
     * an exact IP address 
     * a mask for a group of IP addresses
     * a country IP addresses belong to
     * user agent pattern
   * **Filter type** : Choose if you want to give or forbid access to the site for users with the particular condition type.
   * **Filter range** : Select what part of your store should be inaccessible.
   * **Reason** : Specify the reason for applying the limitations if required.
   Click **Create** to complete the filter creation.
3. The newly created filter will become available on the **Access filters** page:
    ![buip-access-filters.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-access-filters.png)
    

Filters can also be created based on a particular order or user information if they look like fraud to you.

For this purpose:
1. Open either the **Order details page** of a particulat order (**Orders** -> **Order list**) or the **Account details page** of a particular user (**Users** -> **User list**)
   <div class="ui stackable two column grid">
     <div class="column" markdown="span">![buip-order-details.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-order-details.png)</div>
     <div class="column" markdown="span">![buip-user-details.png]({{site.baseurl}}/attachments/ref_3rhs1MJ8/buip-user-details.png)</div>
    </div>
2. Locate the IP address section.
3. Click the **Start creation of filter for this IP** button to add a new filter. You'll be redirected to the **Access filter** page.
4. Create a new filter for the chosen IP address. Be sure to click **Create** to complete the creation of your filter.

The newly created filter is added to the filter list.
