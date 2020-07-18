LEPP - Web Stack (Nginx+PHP+PostgreSQL)
=======================================

**TODO:** This is an attempted merge of the Turnkey Linux LAPP and
Nginx+PHP-fastcgi appliances. It's planned to retain Nginx, php-fastcgi,
PostgreSQL, and maybe Python, and eliminate Apache and MariaDB.

The LAPP stack is an open source web platform that can be used to run
dynamic web sites and servers. It is considered by many to be a powerful
alternative to the more popular LAMP stack and includes Linux, Apache,
PostgreSQL (instead of MySQL) and PHP, Python and Perl.

This appliance includes all the standard features in `TurnKey Core`_,
and on top of that:

- SSL support out of the box.
- PHP, Python and Perl support for Apache2 and PostgreSQL.
- `Adminer`_ administration frontend for PostgreSQL (listening on
  port 12322 - uses SSL).
- Webmin modules for configuring Apache2, PHP and PostgreSQL.
- PostgreSQL listening on localhost (security)
- PostgreSQL password encryption enabled by default (security).
- The *postgres* user is trusted when connecting over local unix sockets
  (convenience).

A separate appliance is available for the `LAMP stack`_ (featuring MySQL
instead of PostgreSQL).

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH: username **root**
-  PostgreSQL, Adminer: username **postgres**

.. _TurnKey Core: https://www.turnkeylinux.org/core
.. _Adminer: http://www.adminer.org/
.. _LAMP stack: https://www.turnkeylinux.org/lampstack
