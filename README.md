#Scanning my Local Network for Open Ports

This project explains how to find your local IP range, how to perform TCP SYN scan and how to find open ports on your network using 'nmap'.

---

##Finding my Local IP range

1. Checked local IP with this command:
   
   ip a

   Where a = address

2. Finding my network interface:
   
   - Looked for my network interface (eth0)
   
   - Found the inet address inside (inet 192.x.x.105/24)
   
   Where:
   
     192.x.x.105 is my machines IP
     and
     /24 subnet mask indicates my IP range is 192.x.x.0 - 192.x.x.255
   
3. Scanning my local network using nmap:
   
   Command:
   nmap -sn 192.x.x.0/24
   
   Where:
   
     -sn = ping scan (to find which hosts are alive)

   Results:
   
   Active hosts:
   
    - Host A: 192.x.x.1
      
    - Host B: 192.x.x.105 (this Machine)



