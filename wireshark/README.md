# Network & traffic analysis
# wireshark
Wireshark — GUI (Wireshark) is a packet capture and analysis tool. Used to inspect protocols,  
credentials in cleartext, TLS handshakes, etc.
When to use: capture evidence of insecure protocols, replayable traffic, or handshake problems.  
For practicising wireshark I used a pcap file which had udp packets which had a secret audio file embedded in it.  
In this file there were udp packets all whihc were of the size of 1442 and 714, which looked odd, so i decided to decode the udp packets to rtp packets and rtp is the standard packet used for audio communication. 
Then all I had to do was analyze the rtp stream and bam, I got the embedded audio file.  
(add screenhots )
