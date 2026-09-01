# Day 01 — Networking Fundamentals

## 🎯 Objective

Understand the fundamentals of computer networking and learn how to inspect my own system's network configuration.

## 📚 Topics Learned

* What is a computer network?
* LAN vs WAN
* IP address
* MAC address
* Default gateway
* DNS
* DHCP
* TCP/IP
* Basic network troubleshooting

## 💻 Practical Commands

### Windows

```text
ipconfig
ipconfig /all
ping 8.8.8.8
tracert google.com
nslookup google.com
arp -a
```

## 🧪 Practical Exercise

### Exercise 1 — Find my network information

I used:

```text
ipconfig /all
```

I identified:

* IPv4 address
* Subnet mask
* Default gateway
* DNS server
* DHCP status

### Exercise 2 — Test connectivity

```text
ping 8.8.8.8
```

### Exercise 3 — Analyze ARP

```text
arp -a
```

This helped me understand how IP addresses are associated with MAC addresses on my local network.

## 🧠 What I Learned

Today I learned how a computer obtains an IP address, communicates with other devices, and uses DNS and the default gateway to communicate beyond the local network.

## 🔐 Cybersecurity Connection

Networking is fundamental to cybersecurity.

Understanding IP addresses, DNS, ARP, TCP/IP and network traffic will help me later with:

* SOC analysis
* Packet analysis
* Network attacks
* Intrusion detection
* Incident response
* Wireshark

## 📌 Key Takeaway

> Before learning how to defend a network, I need to understand how the network works.

**Day 01 Complete ✅**
