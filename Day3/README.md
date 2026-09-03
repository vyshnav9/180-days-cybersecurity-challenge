# Day 03 — IPv4 & Subnetting

## 🎯 Objective

Learn IPv4 addressing and understand how subnetting is used to divide networks into smaller networks.

## 📚 Topics Learned

* IPv4 addressing
* IPv4 address structure
* Subnet masks
* CIDR notation
* Network address
* Broadcast address
* Host addresses
* Private IP ranges
* Subnetting
* Number of hosts per subnet
* Number of subnets

## 🌐 IPv4

IPv4 addresses are 32-bit addresses divided into four 8-bit octets.

Example:

`192.168.1.10`

Each octet can contain values from 0 to 255.

## 🔢 Subnet Mask

A subnet mask determines which portion of an IPv4 address represents the network and which portion represents hosts.

Example:

`192.168.1.10/24`

Subnet mask:

`255.255.255.0`

## 📌 CIDR

CIDR represents the number of network bits.

Examples:

| CIDR | Subnet Mask     |
| ---- | --------------- |
| /24  | 255.255.255.0   |
| /25  | 255.255.255.128 |
| /26  | 255.255.255.192 |
| /27  | 255.255.255.224 |
| /28  | 255.255.255.240 |

## 🏠 Private IPv4 Ranges

* `10.0.0.0/8`
* `172.16.0.0/12`
* `192.168.0.0/16`

These ranges are commonly used inside private networks.

## 🧮 Subnetting Practice

### Example

IP:

`192.168.10.70/26`

Subnet mask:

`255.255.255.192`

Block size:

`64`

Network:

`192.168.10.64`

First usable host:

`192.168.10.65`

Last usable host:

`192.168.10.126`

Broadcast:

`192.168.10.127`

Usable hosts:

`62`

## 💻 Practical Work

I practiced the following networking commands:

```bash
ipconfig
ping 8.8.8.8
ping google.com
nslookup google.com
tracert google.com
arp -a
```

I used these commands to inspect network configuration, test connectivity, examine DNS resolution, trace network paths, and view the local ARP cache.

## 🔐 Cybersecurity Relevance

Understanding IPv4 and subnetting is important for a SOC analyst because network traffic investigations often require identifying:

* Source IP
* Destination IP
* Local vs external addresses
* Network/subnet
* Hosts within a subnet
* Suspicious communication between systems

Subnet knowledge also helps analysts understand network segmentation and identify whether traffic is occurring within the same network or across different networks.

## 🧠 Key Formulas

### Total addresses

`2^host_bits`

### Traditional usable hosts

`2^host_bits - 2`

### Number of subnets

`2^borrowed_bits`

## 💡 Key Takeaways

1. IPv4 addresses contain 32 bits.
2. CIDR indicates the number of network bits.
3. The network address identifies a subnet.
4. The broadcast address communicates with all hosts on a subnet.
5. Private IP addresses are commonly used inside internal networks.
6. Subnetting divides a larger network into smaller networks.
7. Understanding subnetting is useful for network monitoring and SOC investigations.

## 📸 Evidence

Screenshots of my practical exercises are included in the `screenshots` folder.

## 🚀 Progress

**Day 03 / 180 completed ✅**
