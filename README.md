munin\_redis\_celery
==================

Monitors celery queues stored in redis.

Installation
------------

As a non-privileged user:
```
git clone ...
```

As root:
```
ln -s /path/to/munin_redis_celery/redis_celery /etc/munin/plugins
```

Create /etc/munin/plugins-conf.d/redis_celery:
```
[redis_celery]
user _username_
env._setting1_ _value_
...
```

### Settings

`env.queues` (required) a comma-separated list of queues to mnitor,
`env.redis\_database` (optional) the number of the redis database where queues are stored (defaults to 0)

Licence
-------

GPL License (see [GPL-LICENSE.txt](./GPL-LICENSE.txt))

