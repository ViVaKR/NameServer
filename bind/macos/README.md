# MAC Bind

```bash
    $ brew install bind
    $ /usr/local/sbin/rndc-confgen -a 
    # rndc.key location :  "/usr/local/etc/bind/rndc.key"

```

## Configuration Files

    * /etc/named.conf
    * /usr/local/etc/bind/rndc.key
    * /etc/bind/named.conf.options
    * /etc/bind/named.conf.local
    * /etc/bind/named.con.default-zones
    * /etc/bind/db.0
    * /etc/db.empty
    * /etc/db.127
    * /etc/db.255
    * /etc/db.local
    * /zones.rfc1918
    * /var/named/named.ca (download -> $ curl http://www.internic.net/domain/named.root > /var/named/named.ca )

## link : named.conf

`ln -s /usr/local/etc/bind/named.con /etc/named.conf`

## Check

`dig google.com`

## ssh file copy

`scp vivabm@ns.vivabm.local:/etc/resolv.conf $(pwd)`
