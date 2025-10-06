# netdiscover
Here i run mercury machine on my virtual box with Kali in it as well, so to discover the IP of the vulnerable machine i use netdiscover
- netdiscover -r 192.168.56.0/24

Here -r flag is used to specify the ip range, and we get the ip range from our ip address using ifconfig eth0
- ifconfig eth0

(Add screenshots here)
