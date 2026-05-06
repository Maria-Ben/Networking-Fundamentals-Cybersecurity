<img width="477" height="376" alt="Screenshot 2026-05-06 122312" src="https://github.com/user-attachments/assets/c3939f27-01cd-44a8-b4f9-5909a1b498e9" />
# Networking-Fundamentals-Cybersecurity
# 🌐 Networking Fundamentals for Cybersecurity (My Learning Journey)

## 📌 Overview

This repository documents my journey of building a strong foundation in networking concepts for a career in cybersecurity.
I am starting from the basics and connecting theory with hands-on practice using tools like Wireshark.

---

## 🧠 1. IP Addresses

### What is an IP Address?

An IP address uniquely identifies a device on a network.

### Types of IP Addresses

#### 🔹 Private IP (Local Network)

* Used inside home/office networks
* Assigned by router (DHCP)
* Examples:

  * 192.168.x.x
  * 10.x.x.x
  * 172.16–31.x.x

#### 🔹 Public IP (Internet)

* Assigned by ISP
* Used to communicate on the internet
* Example:

  * 99.xxx.xxx.xxx

### Key Learning

* Private IP = internal identity
* Public IP = internet identity

---

## 🔄 2. Static vs Dynamic IP

* **Dynamic IP** → changes over time (most common)
* **Static IP** → fixed (used in servers/business)

✔ Private IP → usually dynamic
✔ Public IP → usually dynamic (home), static (business)

---

## 🌐 3. DNS (Domain Name System)

### What is DNS?

DNS converts domain names into IP addresses.

Example:
google.com → 142.xxx.xxx.xxx

### DNS uses:

* Port 53 (UDP/TCP)

### OS-Level DNS Commands

* `ipconfig /all` → view DNS server
* `ipconfig /displaydns` → view cache
* `ipconfig /flushdns` → clear cache
* `nslookup google.com` → manual query

---

## 🔌 4. Ports

### What is a Port?

A port identifies a specific service/application on a device.

### Common Ports:

* 80 → HTTP
* 443 → HTTPS
* 53 → DNS

### Key Learning:

* IP = device
* Port = service

---

## 🔐 5. HTTP vs HTTPS

* HTTP → unencrypted communication (port 80)
* HTTPS → encrypted communication (port 443)

✔ HTTPS is secure and widely used today

---

## 📡 6. TCP/IP

### TCP

* Reliable communication
* Ensures data delivery

### IP

* Routes data to correct destination

### Key Learning:

TCP + IP = foundation of internet communication

---

## 🔗 7. MAC Address vs IP Address

| MAC Address    | IP Address       |
| -------------- | ---------------- |
| Hardware-based | Network-based    |
| Permanent      | Can change       |
| Local network  | Internet + local |

---

## 🏠 8. Networking Devices

### Modem

* Connects home to ISP

### Router

* Assigns IPs (DHCP)
* Manages traffic

### Switch

* Connects devices in LAN
* Uses MAC addresses

---

## 📶 9. Private vs Public Communication

* Devices use private IP internally
* Router uses public IP to communicate externally
* NAT allows multiple devices to share one public IP

---

## 📊 10. Wireshark (Hands-On Learning)

Tool used: Wireshark (packet analyzer)

### What I learned:

* Captured live network traffic
* Observed DNS queries
* Identified TCP connections
* Understood HTTPS (TLS) traffic

### Filters used:

* `dns` → domain lookups
* `tcp` → connections
* `tls` → encrypted traffic

---

## 🔍 11. Mapping Traffic to Applications

Used:

* `netstat -ano`
* Task Manager (PID mapping)

### Learning:

* Connected IP + Port → Process
* Identified which application generates traffic

---

## ⚠️ 12. Normal vs Suspicious Traffic

### Normal:

* HTTPS to known domains
* DNS queries for visited sites

### Suspicious:

* Unknown IPs
* Unusual ports
* Unexpected applications

---

## 🧠 Key Takeaways

* Networking is the foundation of cybersecurity
* Every communication uses:

  * IP (device)
  * Port (service)
  * Protocol (rules)
* Tools like Wireshark help visualize real traffic
* Understanding “normal behavior” is critical to detect threats

---

## 🚀 Next Steps

* Learn network scanning (Nmap)
* Practice labs on TryHackMe
* Build more hands-on projects
* Explore basic security attacks

---

## 📌 Goal

To build strong fundamentals and transition into a cybersecurity role such as a SOC Analyst.
