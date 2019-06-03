---
lang: en
layout: article_with_sidebar
updated_at: '2019-05-20 16:45 +0400'
identifier: ref_19hsx4O9
title: 'Step 1: System requirements'
order: 20
published: true
---
[_X-Cart v4 to v5 Data Migration Wizard_ module](https://market.x-cart.com/addons/migration-wizard.html) has the same {% link "system requirements as X-Cart 5" ref_VG5mIoLT#server-requirements %}, but since the module runs resource-heavy processes, you need to make sure that the server will not time out them.

The way to set the server up will depend on the server's engine.

{% toc Table of Contents %}

## Apache

The `TimeOut` setting must be set to 600 or greater value in the Apache config file, e.g.:
     
```TimeOut 600```

If `php.ini` has `safe_mode = on`, ensure that the `max_execution_time` setting is defined as 600 or greater, e.g: 
     
```max_execution_time = 600```

If `safe_mode = off`, no additional setup is needed. 

## nginx configuration

The `fastcgi_read_timeout` setting must be set to 600 or higher in the `nginx` config file, e.g.: 
     
```fastcgi_read_timeout 600;```

The `request_terminate_timeout` parameter must be set to 600 or higher value in the `php-fpm` config file, e.g.:
     
```request_terminate_timeout = 600```

If `php.ini` has `safe_mode = on`, ensure that the `max_execution_time` setting is defined as 600 or higher, e.g: 
     
```max_execution_time = 600```

If `safe_mode = off`, no additional setup is needed.
