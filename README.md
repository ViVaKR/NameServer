# NameServer

## bind9

>- named.conf

    - Comment
      - /* C Style */, // C++ Style , # Unix Shells and Perl
    - Block : 공통 기능을 간는 명령문
    - Statement : 특정 BIND 동작을 정의하고 제어 함.

>- Black
    - acl
    - contorls
    - dnssec-policy
    - key
    - key-store
    - logging
    - master

>- TTL 시간 단위 접미사
    - W, D, H, M, S
    - 1W, 3d12h
    - P3M10D(3개월 10일)

```bash
    named-checkconf /etc/named.conf
    named-checkzone vivarkr.com.zone /var/named/vivakr.com.zone

    rndc reload zonename

    rndc-confgen -a
    rndc-confgen > etc/rndc.conf
    head -n 6 /etc/rndc.conf > /etc/rndc.key

    service named status
    service named reload
    service named restart
    service named start
    service named stop

```
