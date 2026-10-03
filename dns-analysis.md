DNS Traffic Analysis

Objective

The objective of this experiment was to observe how DNS queries and responses work by capturing DNS traffic using Wireshark.

Tools Used

- Wireshark
- Windows Command Prompt
- "nslookup"

Experiment

I started a Wireshark capture and generated a DNS request using:

nslookup example.com

I then applied the following Wireshark display filter:

dns

What I Observed

The capture showed DNS queries and responses between my computer and the DNS server.

A DNS query was sent from the client to the DNS server requesting information about a domain name.

The DNS server then sent a response containing information about the requested domain.

The captured packets showed:

- Protocol: DNS
- Transport protocol: UDP
- Destination port: 53
- DNS query and response packets
- A records and AAAA records for domain names

Example DNS Communication

The basic communication observed was:

My Computer
     |
     | DNS Query
     | "What is the IP address of example.com?"
     ↓
DNS Server
     |
     | DNS Response
     | "Here are the IP addresses."
     ↓
My Computer

What I Learned

This experiment helped me understand that DNS converts domain names into IP addresses that computers can use to communicate.

I also learned how DNS traffic appears in Wireshark and how to use the "dns" display filter to identify DNS packets.

Conclusion

The experiment demonstrated the practical process of DNS name resolution and connected the networking concepts I learned with actual network traffic captured from my computer.