# 🌐 02-Networking

## Overview

This folder documents the networking concepts, protocols, commands and practical skills I have learned since beginning my cybersecurity journey in **May 2026**.

The knowledge documented here was primarily gained through **Hack The Box Academy**, where I completed the **Network Foundations** and **Introduction to Networking** modules. I also reinforced these concepts through practical exercises on both Windows and Linux systems.

Networking is one of the most important foundations in cybersecurity because every device, application and service communicates over a network. Understanding networking is essential for penetration testing, system administration, incident response and security operations.

---

# 📅 Learning Journey

I began studying networking in **May 2026** after completing the Introduction to Information Security module on Hack The Box Academy.

During my studies, I learned how devices communicate across networks, how data is transmitted between hosts, how common networking protocols work and how network infrastructure supports secure communication.

I also learned how to connect securely to the **Hack The Box VPN using OpenVPN** on both **Windows and Linux**, allowing me to access Hack The Box Academy laboratories for hands-on practice.

---

# 🎓 Learning Platform

- Hack The Box Academy

---

# ✅ Modules Completed

- Network Foundations
- Introduction to Networking

---

# 🎯 Learning Objectives

The objectives of these modules were to:

- Understand how computer networks operate.
- Learn the purpose of networking protocols.
- Understand how devices communicate.
- Learn the OSI and TCP/IP models.
- Understand network addressing.
- Learn common networking services.
- Practice network troubleshooting.
- Build a networking foundation for cybersecurity.

---

# 📚 Topics Covered

## Computer Networks

A computer network is a collection of interconnected devices that communicate and share resources. Networks allow computers, servers, mobile devices and applications to exchange information efficiently and securely.

---

## Types of Networks

### Local Area Network (LAN)

A Local Area Network (LAN) connects devices within a limited geographical area such as a home, office or school.

### Metropolitan Area Network (MAN)

A Metropolitan Area Network (MAN) connects multiple LANs across a city or metropolitan area.

### Wide Area Network (WAN)

A Wide Area Network (WAN) connects networks across large geographical distances. The Internet is the largest WAN.

### Personal Area Network (PAN)

A Personal Area Network (PAN) connects personal devices over short distances using technologies such as Bluetooth.

---

## Network Devices

### Router

A router connects different networks together and forwards packets using IP addresses. It enables communication between a local network and external networks such as the Internet.

### Switch

A switch connects devices within the same local network and forwards traffic using MAC addresses. Switches improve communication efficiency by sending data only to the intended destination.

---

## OSI Model

The Open Systems Interconnection (OSI) Model explains how data travels across a network using seven layers.

The seven layers are:

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

The OSI Model provides a standardized framework for understanding network communication and troubleshooting networking problems.

---

## TCP/IP Model

The TCP/IP Model is the networking model used on the Internet.

It consists of four layers:

1. Network Access
2. Internet
3. Transport
4. Application

Unlike the OSI Model, the TCP/IP Model focuses on the protocols used in real-world networking.

---

## TCP

Transmission Control Protocol (TCP) is a connection-oriented protocol that establishes a connection before transmitting data.

TCP guarantees reliable communication by ensuring that packets arrive correctly, in order and without loss.

Common protocols using TCP include:

- HTTP
- HTTPS
- SSH
- FTP
- SMTP

---

## UDP

User Datagram Protocol (UDP) is a connectionless protocol that sends data without first establishing a connection.

UDP is faster than TCP but does not guarantee delivery or packet order.

Common protocols using UDP include:

- DNS
- VoIP
- DHCP
- Online Gaming
- Video Streaming

---

## Difference Between TCP and UDP

TCP provides reliable, connection-oriented communication by performing error checking and guaranteeing packet delivery.

UDP is connectionless and prioritizes speed over reliability, making it suitable for applications where fast communication is more important than guaranteed delivery.

---

## TCP Three-Way Handshake

TCP establishes reliable communication using a three-way handshake.

Step 1

The client sends a SYN packet requesting a connection.

Step 2

The server responds with a SYN-ACK packet acknowledging the request.

Step 3

The client replies with an ACK packet.

After these three steps, the connection is established and data transmission begins.

---

## IP Address

An IP address is a logical address assigned to a device on a network.

It enables devices to communicate with each other across local and global networks.

The two versions are:

- IPv4
- IPv6

Example:

```
192.168.1.10
```

---

## MAC Address

A MAC address is the unique physical hardware address assigned to a network interface card by the manufacturer.

Example:

```
00:1A:2B:3C:4D:5E
```

---

## Difference Between an IP Address and a MAC Address

An IP address is a logical address assigned by the network and can change depending on network configuration.

A MAC address is a physical hardware address that is permanently assigned to a network interface.

IP addresses operate at Layer 3 of the OSI Model, while MAC addresses operate at Layer 2.

---

## DNS

The Domain Name System (DNS) translates domain names into IP addresses.

Instead of remembering numerical IP addresses, users can access websites using domain names.

Example:

```
google.com → 142.x.x.x
```

---

## DHCP

The Dynamic Host Configuration Protocol (DHCP) automatically assigns network configuration information including:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Server

DHCP simplifies network administration by eliminating manual IP configuration.

---

## NAT

Network Address Translation (NAT) converts private IP addresses into public IP addresses.

It allows multiple devices on a private network to share a single public IP address while improving security and conserving IPv4 addresses.

---

## NTP

Network Time Protocol (NTP) synchronizes the clocks of computers and network devices.

Accurate system time is essential for security monitoring, authentication, digital forensics and log analysis.

---

## VPN

A Virtual Private Network (VPN) encrypts network traffic and creates a secure connection between a user and a remote network.

During my studies, I learned how to connect to the **Hack The Box VPN** using **OpenVPN** on both **Windows** and **Linux** to securely access Hack The Box Academy labs.

---

# 💻 Networking Commands

## Windows

```powershell
ping 8.8.8.8
```

Tests connectivity between your computer and another device.

```powershell
ping 8.8.8.8 -t
```

Sends continuous ping requests until stopped with **Ctrl + C**.

```powershell
tracert 8.8.8.8
```

Displays the route packets take to reach a destination.

```powershell
ipconfig
```

Displays the current IP configuration.

```powershell
ipconfig /all
```

Displays detailed network configuration.

```powershell
arp -a
```

Displays the ARP cache.

```powershell
netstat
```

Displays active network connections.

```powershell
nslookup google.com
```

Queries DNS records.

---

## Linux

```bash
ip a
```

Displays network interfaces and IP addresses.

```bash
ping google.com
```

Tests network connectivity.

```bash
traceroute google.com
```

Displays the path packets take to reach a destination.

```bash
netstat
```

Displays active network connections.

```bash
ss
```

Displays active network sockets.

```bash
dig google.com
```

Queries DNS records.

---

# 🛠️ Practical Skills Developed

During these modules I developed practical skills in:

- Understanding computer networking concepts.
- Identifying different network types.
- Understanding routers and switches.
- Understanding the OSI Model.
- Understanding the TCP/IP Model.
- Differentiating between TCP and UDP.
- Understanding the TCP Three-Way Handshake.
- Configuring and identifying IP addressing.
- Understanding MAC addressing.
- Understanding DNS, DHCP, NAT and NTP.
- Troubleshooting networking issues.
- Using networking commands on Windows.
- Using networking commands on Linux.
- Connecting securely to Hack The Box labs using OpenVPN.

---

# 💻 Tools and Technologies

During this stage of my learning journey I used:

- Hack The Box Academy
- Windows
- Ubuntu Linux
- PowerShell
- Linux Terminal
- OpenVPN
- Git
- GitHub
- Visual Studio Code

---

# 🌍 Real-World Applications

The networking knowledge gained during these modules is directly applicable to:

- Network Administration
- Security Operations Centers (SOC)
- Penetration Testing
- Incident Response
- Cloud Computing
- Network Troubleshooting
- System Administration
- Enterprise Security

---

# 📖 Source

- Hack The Box Academy – Network Foundations
- Hack The Box Academy – Introduction to Networking
- Pysical practices on my home network Muranga county head quaters Kenya
---

# 📌 Summary

Completing the **Network Foundations** and **Introduction to Networking** modules gave me a strong understanding of how modern computer networks operate. I learned how devices communicate, how common networking protocols function, how network services support communication and how to troubleshoot basic networking issues.

These modules also provided practical experience using networking tools on both Windows and Linux and taught me how to securely connect to Hack The Box Academy using OpenVPN. This networking knowledge forms a critical foundation for my continued studies in Linux, Windows, Web Security, Active Directory and Penetration Testing.