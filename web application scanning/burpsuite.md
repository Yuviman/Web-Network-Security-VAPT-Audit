# Burp Suite (Port Swigger)
Lab: 2FA simple bypass  
This lab's two-factor authentication can be bypassed. You have already obtained a valid username and password, but do not have access to the user's 2FA verification code. To solve the lab, access Carlos's account page.  
Your credentials: wiener:peter  
Victim's credentials carlos:montoya  

well you can login to the website using the given credentials, and since we have access to our mail we can get the verification code.  
Afterwards we try logging in to the targets account.  
The error with the web page is that when you login to the target's account with the credentials, it sets a cookie for the user, which can be accesed in the burp suite proxy server.
From here you change the cookie to gain access to /my-account directory. 
<img width="1920" height="1080" alt="Screenshot 2025-10-06 231223" src="https://github.com/user-attachments/assets/614ef111-3708-4ac1-b5e8-97128d3f2ef5" />
<img width="1920" height="1080" alt="Screenshot 2025-10-06 231345" src="https://github.com/user-attachments/assets/70561cdb-8073-4a44-a19d-8960bc894899" />
<img width="1920" height="1080" alt="Screenshot 2025-10-06 231927" src="https://github.com/user-attachments/assets/c4358c38-78f8-4643-b34b-86f1b940b07b" />
<img width="1920" height="1080" alt="Screenshot 2025-10-06 232400" src="https://github.com/user-attachments/assets/3ca0afb3-1e3a-4792-af87-d2c86eb2d4f7" />
<img width="1920" height="1080" alt="Screenshot 2025-10-06 232421" src="https://github.com/user-attachments/assets/82d347b4-5e1e-45d3-bd95-3e99433c2dad" />
<img width="1920" height="1080" alt="Screenshot 2025-10-06 232550" src="https://github.com/user-attachments/assets/789a8ad1-473c-4c90-8a3e-f42210e60f64" />

