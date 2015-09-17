# docker-pdns-recursor

PowerDNS Recursor (logging endbled) inside docker container

### How to use

1. Start container with recursor  
```docker run -d -p 172.17.42.1:53:53/udp --name dnslogger vaysman/dns-logger:1.0```
1. Start other container with **--dns** option  
```--dns 172.17.42.1```
1. Look at log  
```docker logs -f dnslogger```
