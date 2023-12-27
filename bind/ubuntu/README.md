# bind9

```bash
    $ sudo netplan try
    $ sudo netplan apply
    $ sudo systemctl restart bind9
    $ sudo systemctl restart systemd-resolved

    # clear cache & view dump 
    $ rndc flush
    $ rndc reload
    $ rndc dumpdb -cache
    $ cd /var/cache/bind
    $ grep text.or.kr named_dump.db
```
