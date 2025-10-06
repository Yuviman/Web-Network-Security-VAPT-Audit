# nmap
since i found the ip of the vulnerable machine using netdiscover and found out that my kali ip is 192.168.56.103 and ip of the mercury machine is
192.168.56.102, now we will scan the machine using nmap to look for open services which we can use to try and infiltrate the machine.

- nmap -A 192.168.56.102

We found out that there are 2 services open, one is a ssh protocol at port 22 and another is a http service at port 8080, maybe we can look at the http service

(add screenshot here)
