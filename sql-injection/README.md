# Exploitation & attack automation
# metasploit
Metasploit Framework — modular exploitation framework with payloads, auxiliaries, and post-exploitation modules.  
When to use: exploit known service vulnerabilities in a controlled lab.  
Example: msfconsole, then use exploit/unix/ftp/vuln ...  

# sqlmap
sqlmap — automated SQL injection detection and exploitation tool with extraction capabilities.  
When to use: confirm SQLi, enumerate databases, dump data (lab only).  
Example: sqlmap -u "http://10.0.2.15/item?id=1" --batch --dump  

# hydra
Hydra — fast password brute-forcer for many protocols (http-form, ssh, ftp, etc.).  
When to use: test weak credentials (only where authorized).  
Example: hydra -l admin -P passwords.txt ssh://10.0.2.15  
