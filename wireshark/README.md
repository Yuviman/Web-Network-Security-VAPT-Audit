# Network & traffic analysis
# wireshark
Wireshark — GUI (Wireshark) is a packet capture and analysis tool. Used to inspect protocols,  
credentials in cleartext, TLS handshakes, etc.
When to use: capture evidence of insecure protocols, replayable traffic, or handshake problems.  
For practicising wireshark I used a pcap file which had udp packets which had a secret audio file embedded in it.  
In this file there were udp packets all whihc were of the size of 1442 and 714, which looked odd, so i decided to decode the udp packets to rtp packets and rtp is the standard packet used for audio communication. 
Then all I had to do was analyze the rtp stream and bam, I got the embedded audio file.  
<img width="1920" height="903" alt="Screenshot_2025-10-06_10_22_09" src="https://github.com/user-attachments/assets/b3aaa7e2-2c92-4e66-a715-d7312cbe7799" />
<img width="1920" height="903" alt="Screenshot_2025-10-06_10_21_41" src="https://github.com/user-attachments/assets/3070ac53-4ed1-46c2-ab13-edb3d06b812b" />
<img width="1920" height="903" alt="Screenshot_2025-10-06_10_21_34" src="https://github.com/user-attachments/assets/60b0cffb-ccc0-48a0-9878-b0808b024ae5" />

<img width="1920" height="903" alt="Screenshot_2025-10-06_10_21_23" src="https://github.com/user-attachments/assets/daf1d2fe-9e09-4d47-b9b9-8e18c0081568" />
