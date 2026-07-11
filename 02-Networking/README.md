# 02-Networking

# 🌐 02-Networking

## Overview

This folder contains the networking concepts and commands I have learned during my cybersecurity journey.

## Network Types

A Local Area Network (LAN) connects devices within a small geographical area such as a home, school, or office.

A Metropolitan Area Network (MAN) connects multiple LANs across a city.

A Wide Area Network (WAN) connects networks over large geographical distances, such as the Internet.

A Personal Area Network (PAN) connects personal devices over a short distance using technologies such as Bluetooth.

## Network Devices

A router connects different networks together and forwards packets between them. It is commonly used to connect a local network to the Internet.

A switch connects devices within the same local network and forwards data using MAC addresses, making communication faster and more efficient.

## OSI Model

The OSI model consists of seven layers:

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

The OSI model helps explain how data travels from one computer to another.

## TCP/IP Model

The TCP/IP model has four layers:

1. Network Access
2. Internet
3. Transport
4. Application

It is the networking model used on the Internet.

## TCP and UDP

TCP is a connection-oriented protocol that establishes a connection before transmitting data. It is reliable because it checks for errors and ensures packets arrive in the correct order. It is commonly used by HTTP, HTTPS, SSH and FTP.

UDP is a connectionless protocol that sends data without first establishing a connection. It is faster than TCP but does not guarantee delivery or packet order. It is commonly used by DNS, VoIP, online gaming and video streaming.

## TCP Three-Way Handshake

A TCP connection is established using three steps.

Step 1: The client sends a SYN packet.

Step 2: The server responds with a SYN-ACK packet.

Step 3: The client replies with an ACK packet.

After these three steps, communication begins.

## IP Address

An IP address is a logical address that identifies a device on a network. IPv4 and IPv6 are the two versions of IP addresses.

Example:

192.168.1.10

## MAC Address

A MAC address is the unique physical address assigned to a network interface card by the manufacturer.

Example:

00:1A:2B:3C:4D:5E

## Difference Between an IP Address and a MAC Address

An IP address is a logical address that can change depending on the network, while a MAC address is a physical hardware address that is usually permanent. An IP address operates at Layer 3 of the OSI model, whereas a MAC address operates at Layer 2.

## DNS

The Domain Name System (DNS) translates domain names into IP addresses so that computers can locate websites.

Example:

google.com → 142.x.x.x

## DHCP

The Dynamic Host Configuration Protocol (DHCP) automatically assigns an IP address, subnet mask, default gateway and DNS server to devices joining a network.

## NAT

Network Address Translation (NAT) translates private IP addresses into public IP addresses, allowing multiple devices to share a single public IP address while improving security.

## NTP

Network Time Protocol (NTP) synchronizes the clocks of computers and network devices. Accurate time is important for security monitoring and log analysis.

## VPN

A Virtual Private Network (VPN) encrypts Internet traffic and creates a secure connection between a user and a remote network. It protects privacy and secures communication over public networks.

## Networking Commands

powershell
ping 8.8.8.8
Tests connectivity between your computer and another device.
powershell
ping 8.8.8.8 -t

Sends continuous ping requests until stopped with **Ctrl + C**.

powershell
tracert 8.8.8.8

Displays the path packets take to reach a destination.

powershell
ipconfig

Displays the current IP configuration.
powershell
ipconfig /all
Displays detailed network configuration.

## Skills Gained

I learned how computer networks communicate, how routers and switches operate, the OSI and TCP/IP models, the differences between TCP and UDP, how the TCP three-way handshake establishes connections, the differences between IP and MAC addresses, and the roles of DNS, DHCP, NAT, NTP and VPN in modern computer networks. I also practiced using common Windows networking commands for troubleshooting and network analysis.
Notes for 02-Networking go here.
