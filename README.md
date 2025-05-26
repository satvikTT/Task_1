# NETWORK SCANNING & ANALYSIS PROJECT

Learn to discover open ports on devices in your local network using **Nmap** to understand network exposure. It also includes capturing network packets using **Wireshark** and improve network security awareness.

---
## Objective

Understand how to discover open ports on devices within your local network. This helps assess network exposure, identify potential vulnerabilities, and improve overall network security posture.

---

## Tools Used

| Tool          | Purpose                                                  |
|---------------|----------------------------------------------------------|
| **Nmap**      | Scan local network for open TCP/UDP ports and services   |
| **Wireshark** | (Optional) Analyze network traffic and packet details    |
| **Kali Linux**| Penetration testing OS used as the scanning environment  |

---

## IP Configuration

- **Local IP Address:** `192.168.2.153`
- **Target Subnet:** `192.168.2.153/24`
- **Interface Used:** `eth0`
  
---

To find IP and interface:
'''bash
ip a / ifconfig
'''
---

To save scan results as a Text file:
```bash
sudo nmap -sS 10.0.2.0/24 -oN nmap.txt
```
---
