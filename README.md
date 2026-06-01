# Active Directory Attack Lab

## Overview

This project demonstrates a complete Active Directory attack chain in a controlled lab environment. The objective was to understand how common misconfigurations and weak security controls can be exploited to achieve full domain compromise.

The lab simulates real-world attack scenarios, covering credential theft, lateral movement, privilege escalation, persistence, and post-exploitation techniques.

---

## Lab Environment

| Component         | Details             |
| ----------------- | ------------------- |
| Domain Controller | Windows Server 2019 |
| Client Machines   | Windows 10          |
| Attacker Machine  | Kali Linux          |
| Domain            | `marvel.local`      |

---

## Attack Path

```text
Initial Access
      ↓
Credential Capture
      ↓
Lateral Movement
      ↓
Privilege Escalation
      ↓
Domain Compromise
      ↓
Persistence
```

---

## Techniques Demonstrated

### Credential Capture

* LLMNR/NBT-NS Poisoning
* SMB Relay Attacks
* URL File Attacks

### Lateral Movement

* Remote Shell Access
* Pass-the-Password
* Pass-the-Hash

### Privilege Escalation

* IPv6 MITM & LDAP Relay
* Token Impersonation
* Kerberoasting

### Credential Access

* Credential Dumping using Mimikatz

### Persistence

* Golden Ticket Attack

---

## Tools Used

* Nmap
* Responder
* Impacket
* Mimikatz
* Hashcat
* Metasploit Framework
* CrackMapExec

---

## Key Learning Outcomes

* Understanding Active Directory attack paths.
* Capturing and abusing credentials.
* Performing lateral movement across domain systems.
* Escalating privileges to Domain Administrator.
* Maintaining persistence through Kerberos ticket manipulation.
* Identifying common Active Directory security weaknesses.

---

## Report

📄 **Full Lab Report:** [Download PDF](./Active%20Directory%20Attack.pdf)

---

## Disclaimer

This project was conducted in a private laboratory environment for educational and defensive security research purposes only.

The techniques demonstrated are intended to help security professionals understand attack methodologies and improve the security posture of Active Directory environments. Unauthorized use of these techniques against systems without explicit permission is illegal and unethical.
