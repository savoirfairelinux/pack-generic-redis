pack-generic-redis
==================

Dependencies
************

Shinken Modules
~~~~~~~~~~~~~~~

Plugins
~~~~~~~

This pack will create services which need the following plugin :

https://github.com/savoirfairelinux/monitoring-tools/tree/master/plugins/plugin-check-redis

and it's here:

`/usr/lib/nagios/plugins/check_redis.py`

Network
~~~~~~~

This pack will create services which need the following protocol :

* TCP 6379 to connect with Redis
* SSL

Installation
************

Copy the pack folder in the packs folder defined in shinken.cfg (`cfg_dir=packs`)

How to use it
*************

Settings
~~~~~~~~

This is the list of settings which can be redefined in the host definition

_REDIS_PORT
-----------

:type:              integer
:description:       port of redis
:default:           6379

_REDIS_CONNECT_WARNING
----------------------

:type:              integer
:description:       warning threshold for the connection time to the server
:default:           2

_REDIS_CONNECT_CRITICAL
-----------------------

:type:              integer
:description:       critical threshold for the connection time to the server
:default:           4

_REDIS_CONNECTED_CLIENTS_WARNING
--------------------------------

:type:              integer
:description:       warning threshold for the number of connected clients
:defaut:            70

_REDIS_CONNECTED_CLIENTS_CRITICAL
---------------------------------

:type:              integer
:description:       critical threshold for the number of connected clients
:defaut:            80

_REDIS_USED_MEMORY_WARNING
--------------------------

:type:              integer
:description:       warninig threshold for the used memory
:defaut:            15

_REDIS_USED_MEMORY_CRITICAL
---------------------------

:type:              integer
:description:       critical threshold for the used memory
:defaut:            30

_REDIS_USED_MEMORY_HUMAN_WARNING
--------------------------------

:type:              integer
:description:       warning threshold for the used memory human
:defaut:            50

_REDIS_USED_MEMORY_HUMAN_CRITICAL
---------------------------------

:type:              integer
:description:       critical threshold for the used memory human
:defaut:            75

_REDIS_USED_MEMORY_RSS_WARNING
------------------------------

:type:              integer
:description:       warning threshold for usage of memory rss
:defaut:            20

_REDIS_USED_MEMORY_RSS_CRITICAL
-------------------------------

:type:              integer
:description:       critical threshold for usage of memory rss
:defaut:            28

_REDIS_LATENCY_WARNING
----------------------

:type:              integer
:description:       warning threshold for the latency
:defaut:            20

_REDIS_LATENCY_CRITICAL
-----------------------

:type:              integer
:description:       critical threshold for the latency
:defaut:            28


