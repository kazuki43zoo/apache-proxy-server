# apache-proxy-server

## How to build and up (rebuild)

```
$ docker-compose up --build
Building apache-proxy
Step 1/3 : FROM httpd:2.4
 ---> 278cd55ca6c5
Step 2/3 : COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf
 ---> 2cb978fec9ad
Removing intermediate container cdbbc0cc2ba6
Step 3/3 : COPY ./.htpasswd /usr/local/apache2/conf/.htpasswd
 ---> 3b77a88585e8
Removing intermediate container dd1091799fa8
Successfully built 3b77a88585e8
Creating apacheproxyserver_apache-proxy_1
Attaching to apacheproxyserver_apache-proxy_1
apache-proxy_1  | AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
apache-proxy_1  | AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
apache-proxy_1  | [Tue Mar 28 19:25:39.148808 2017] [mpm_event:notice] [pid 1:tid 140594197616512] AH00489: Apache/2.4.25 (Unix) configured -- resuming normal operations
apache-proxy_1  | [Tue Mar 28 19:25:39.149390 2017] [core:notice] [pid 1:tid 140594197616512] AH00094: Command line: 'httpd -D FOREGROUND'
```

## How to stop

Ctrl + C

## Proxy Server Information

* Port : 9999
* User/Password: test/test


