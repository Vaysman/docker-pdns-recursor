# docker-pdns-recursor

PowerDNS Recursor (logging endbled) inside docker container

### How to use

1. Start container with recursor ```docker run -d -p 172.17.42.1:53:53/udp vaysman/dns-logger:1.0 -name dnslogger```
1. Start other container with ```--dns 172.17.42.1```
1. Look at log ```docker logs -f dnslogger```
