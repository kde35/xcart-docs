---
lang: en
layout: article_with_sidebar
updated_at: '2016-10-04 17:28 +0400'
identifier: ref_KqsCJNRG
title: XC4 to XC5 Migration wizard system requirements and installation
order: 100
published: true
---
At the moment of the writing of this article, the module "XC4 to XC5 Migration wizard" is recommended for use on X-Cart versions 5.3.0.x and later. It provides a tool for the migration of data and settings from X-Cart 4 based online stores (versions 4.1.0 or later) to the X-Cart 5 platform. For the most up-to-date information on the module compatibility, please see the [module page](https://market.x-cart.com/addons/migration-wizard.html).

The system requirements for the module "XC4 to XC5 Migration wizard" are generally the same as those for the X-Cart 5 version you are using. However, for best performance we recommend using PHP 7.1 (or at least PHP 5.6+). 
If the X-Cart 4 store from which the data is going to be migrated to the X-Cart 5 platform has products with a large number of variants (like 50+ variants per product), it is necessary to ensure that the Request timeout on your server is set to a sufficient value.

   * _Apache configuration:_

     In the Apache config file, the TimeOut value must be set to 600 or higher; for example:
     
     ```TimeOut 600```

     In php.ini, if safe_mode = off, no additional settings need to be adjusted. If php.ini safe_mode = on, ensure that the max_execution_time setting is adjusted to 600 or higher; for example: 
     
     ```max_execution_time = 600```

   * _nginx configuration:_

     In the nginx config, the fastcgi_read_timeout value must be set to 600 or higher; for example: 
     
     ```fastcgi_read_timeout 600;```

     In the php-fpm config, the request_terminate_timeout value must be set to 600 or higher; for example:
     
     ```request_terminate_timeout = 600```

     In php.ini, if safe_mode = off, no additional settings need to be adjusted.  If php.ini safe_mode = on, ensure that the max_execution_time value is set to 600 or higher; for example: 
     
     ```max_execution_time = 600```


To migrate your X-Cart 4 store to X-Cart 5, you need:

   * Your existing X-Cart 4 store. 
   
   For the migration, you will need to provide the migration module with your X-Cart 4 database connection details and your store URL, so be sure to have those at hand when you launch the Migration wizard.
   
   * A fresh installation of X-Cart 5. 
     
     {% note warning %}
     **Important**: Be sure to use the default build configuration that you get right out of the distribution package. Do not install any additional modules and do not attempt any customizations of the X-Cart 5 store's default functionality or look & feel before your X-Cart 4 data and settings have been fully migrated. Be sure to remove any demo data that may be present in the X-Cart 5 store (A link to the "Remove data" tool will be provided at the first step of the Migration wizard).
     {% endnote %}
     
   * Migration wizard module installed on your X-Cart 5 store.
   
     To install and enable the Migration wizard module on your system, follow the general module installation instructions. See {% link "Installing modules from the Marketplace" ref_Vn1mMUw9 %}.
     
     {% note warning %}
     To be able to install the Migration wizard module you should have the [Order import](https://market.x-cart.com/addons/orders-import.html "XC4 to XC5 Migration wizard system requirements and installation") module installed and enabled. 
     
     Please make sure the Order import module is {% link "installed and enabled" ref_uEnDBBA7 %}.
     {% endnote %}
     
     As a result, you should have the module "XC4 to XC5 Migration wizard" installed on your X-Cart 5 store:
     
     ![migration-wizard-installed.png]({{site.baseurl}}/attachments/ref_KqsCJNRG/migration-wizard-installed.png)

After the module is installed you can proceed to the migration of your data and settings. See {% link "Using the module 'XC4 to XC5 Migration wizard'" ref_Ah935naM %} for detailed info.

_Related pages:_

   *   {% link "How XC4 to XC5 Migration wizard works" ref_37NAeGlf %}
   *   {% link "Using the module 'XC4 to XC5 Migration wizard'" ref_Ah935naM %}
