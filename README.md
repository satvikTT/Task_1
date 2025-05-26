# NETWORK SCANNING & ANALYSIS PROJECT (TASK-1)

Learn how to discover open ports on devices within your local network using **Nmap** to assess network exposure. This task also includes optional network packet capturing using **Wireshark** to deepen your understanding of network behavior and improve security awareness.

---

## Objective

Discover and analyze open ports on devices in your local network. This process helps:
- Assess network exposure
- Identify running services
- Pinpoint potential security risks

---

## Tools Used

| Tool           | Purpose                                                  |
|----------------|----------------------------------------------------------|
| **Nmap**       | Scan the network for open TCP/UDP ports and services     |
| **Wireshark**  | (Optional) Capture and inspect network traffic           |
| **Kali Linux** | Penetration testing OS used for scanning and analysis    |

---

## IP Configuration

- **Local IP Address:** `192.168.2.153`  
- **Target Subnet:** `192.168.2.0/24`  
- **Interface Used:** `eth0`

### To find your IP and network interface:
```bash
ip a 
```
```
ifconfig
```
---


To run diffeerent nmap commands:
```bash
nmap 192.168.2.123
```
![output](C:\Users\SATVIK\Desktop\nmap\scan.png)
```
nmap -sS 192.168.2.123/24
```
![output](C:\Users\SATVIK\Desktop\nmap\subnet.png)
```
nmap -sT 192.168.2.123/24
```
```
nmap -A 192.168.2.123/24
```
![output]("C:\Users\SATVIK\Desktop\nmap\agg.png")
```
nmap -sV 192.168.2.123/24
```
---

To start Wireshark capture:
```
wireshark &
```
---


To save scan results as a Text file:
```bash
sudo nmap -sS 192.168.2.123 -oN nmap.txt
```
---
