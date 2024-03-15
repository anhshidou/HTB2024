Decrypted message... 

![image](https://github.com/anhshidou/HTB2024/assets/120787381/e24e41d3-6ebf-4f15-a7e4-bb0b62e9e22a)

At this challenge, it kinda hard for me at first, but when I thought for around 2 days, I saw it really easy

At this challenge, we will recieve a pcap file, that can open as Wireshark

![image](https://github.com/anhshidou/HTB2024/assets/120787381/2a11dc8e-fc9c-4faa-8bd6-6e02fd808b9d)

We found it kinda sus in SMTP, which is kind of Simple Mail Transfer Protocol, which is transfer email

Seeing Wireshark can't help me to solve this problem (because im suck) so I will use Network Miner

This ip address is the most important

![image](https://github.com/anhshidou/HTB2024/assets/120787381/b55005c4-655a-4e59-8864-c1e3c5b7ce5d)

We can see there are a lot of EML file, pick random one to open, we will see this shit, it kinda like base64 tho

![image](https://github.com/anhshidou/HTB2024/assets/120787381/768cc9fc-d195-4d03-926d-2712d1387263)

![image](https://github.com/anhshidou/HTB2024/assets/120787381/a8a9830b-f28e-4531-b92c-0e80dca21864)
