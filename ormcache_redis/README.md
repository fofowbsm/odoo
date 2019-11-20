# odoo-orm-cache

## Dependencies
`odoo-orm-cache` uses [`redis`](https://redis.io/) to store cache into redis server. You will need to install it.


## Compatibility
This module is compatible with **Odoo 11** and **Python 3**. For older versions, you can refer to the original source code (see credits below).

## Configuration
In order to use `odoo-orm-cahe` you will need to switch to "Developer mode" and define a new system parameter as follows:
* modify the master odoo.conf file:
```
    ormcache_redis_url=redis://@redis-ip:6379/0 
    max_cron_threads = x
```

## Additional Information and Credits
This code is [custom from this repo](https://github.com/openliu/Odoo-Cluster) who ported the [original code from tvanesse](https://github.com/tvanesse/odoo-s3) to Odoo v11.0 and using it as modular.

