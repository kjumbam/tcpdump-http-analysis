# tcpdump-http-analysis
Project using tcpdump to capture and analyze HTTP packets.

## Overview  
This project demonstrates how to capture and analyze basic HTTP traffic using tcpdump.  

## Steps  
1. Installed tcpdump on my system.  
2. Identified my active network interface using `tcpdump -D`.  
3. Captured 10 HTTP packets with:  
   sudo tcpdump -i en0 tcp port 80 -c 10 -w http_traffic.pcap
4. Opened https://www.youtube.com in my browser while capturing traffic.
5. Read the packets with 'tcpdump -r http_traffic.pcap' and observed the TCP 3-way handshake.

## Key Takeaways
- Learned how to capture live traffic.
- Understood the TCP 3-way handshake (SYN → SYN-ACK → ACK).
- Practiced filtering by port (HTTP on port 80).
