# netdiscover
Here i run mercury machine on my virtual box with Kali in it as well, so to discover the IP of the vulnerable machine i use netdiscover
- netdiscover -r 192.168.56.0/24

Here -r flag is used to specify the ip range, and we get the ip range from our ip address using ifconfig eth0
- ifconfig eth0

<img width="1920" height="903" alt="Screenshot_2025-10-06_02_30_04" src="https://github.com/user-attachments/assets/d48fb516-9de4-42d8-a2a8-0d3e77ceb23a" />

