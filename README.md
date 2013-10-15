munin\_redis\_celery
==================

Monitors celery queues stored in redis.

Installation
------------

As any user:
```
git clone https://github.com/joeyates/munin_redis_celery.git
```

As root:
```
ln -s /path/to/munin_redis_celery/redis_celery /etc/munin/plugins/redis_celery
```

Create /etc/munin/plugins-conf.d/redis_celery:
```
[redis_celery]
user USERNAME
env.SETTING1 VALUE (see below for settings)
...
```

### Settings

* `env.queues` (required) a comma-separated list of queues to mnitor,
* `env.redis_database` (optional) the number of the redis database where queues are stored (defaults to 0)

Licence
-------

GPL License (see [GPL-LICENSE.txt](./GPL-LICENSE.txt))

