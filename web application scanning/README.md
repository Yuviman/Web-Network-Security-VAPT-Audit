# Web scanning & vulnerability discovery

# nikto
Nikto is a web server scanner that finds common misconfigurations, outdated components, and risky files.  
When to use: quick server-level checks (vulnerable headers, outdated servers).  
Example: nikto -h http://10.0.2.15 -output nikto.txt

# owasp zap
OWASP ZAP — free, GUI web-app scanner that offers passive/active scanning, spidering, and scripting.  
When to use: automated scanning of web apps and APIs; good for beginners.  
Example: run ZAP, set browser proxy, spider site, run active scan.  

# burp suite
Burp Suite (Community/Pro) — industry-standard web proxy for intercepting, modifying, and scanning HTTP(S) traffic. It has strong manual testing features (Repeater, Intruder, Scanner in Pro).  
When to use: manual verification, crafting exploit requests, and comprehensive testing.  
Example: configure browser proxy to 127.0.0.1:8080, intercept requests in Burp.  
