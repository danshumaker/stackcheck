stackcheck
==========

simple python script that checks the version and running processes of the LAMP stack (debian oriented).

It prints out software versions for solr, mysql, apache, os, git, memcached, varnish, and php

It also prints out hardware stats and running processes filterd on apache, memcache, varnish and solr.

Sample output:

```


=====SOFTWARE=======
Description:    Ubuntu 14.04.2 LTS
Server          version: Apache/2.4.12 (Ubuntu)
/usr/bin/mysql  Ver 14.14 Distrib 5.5.43, for debian-linux-gnu (x86_64) using readline 6.3
PHP             5.6.10-1+deb.sury.org~trusty+1 (cli)
/usr/sbin/varnishd command not found
memcached       1.4.14
/usr/bin/java command not found
APC not found
git             version 1.9.1


=====HARDWARE=======
MemTotal:       501748 kB
cpu             cores : 1
Processors      = 1
model           name : Intel(R) Xeon(R) CPU E5-1620 v2 @ 3.70GHz
cpu             MHz : 3700.264


===== RUNNING ======
memcache  1239  0.0  0.2 325392  1176 ?        Sl   13:10   0:00 /usr/bin/memcached -m 64 -p 11211 -u memcache -l 127.0.0.1
root      1345  0.0  4.5 486520 22960 ?        Ss   13:10   0:00 /usr/sbin/apache2 -k start
vagrant   1349  0.0  1.7 486552  8720 ?        S    13:10   0:00 /usr/sbin/apache2 -k start
vagrant   1350  0.0  1.7 486552  8720 ?        S    13:10   0:00 /usr/sbin/apache2 -k start
vagrant   1351  0.0  2.5 486876 12848 ?        S    13:10   0:00 /usr/sbin/apache2 -k start
vagrant   1352  0.0  2.4 486876 12380 ?        S    13:10   0:00 /usr/sbin/apache2 -k start
vagrant   1353  0.0  1.7 486552  8720 ?        S    13:10   0:00 /usr/sbin/apache2 -k start
vagrant   1678  0.0  1.7 486552  8720 ?        S    13:11   0:00 /usr/sbin/apache2 -k start
```
