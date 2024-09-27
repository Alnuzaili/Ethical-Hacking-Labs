# <u>Introduction to Information Security & Penetration Testing</u>

> ⚠️ This module is fully theoretical and was extracted from [CEH Study Guide](https://github.com/Samsar4/CEH-v10-Study-Guide/) repo. Here you'll find some basic terms in 'InfoSec world'.


## <u> Fundamental Security Concepts </u>
The whole principle is to avoid **Theft, Tampering and Disruption** of the systems through **CIA Triad** (Confidentiality, Integrity and Availability).

<p align="center">
<img width="50%" src="https://i.ytimg.com/vi/AJTJN4wDBM8/hqdefault.jpg">
</p>

- **Confidentiality**
Keeping systems and data from being accessed, seen, read to anyone who is not authorized to do so.

- **Integrity**
Protect the data from modification or deletion by unauthorized parties, and ensuring that when authorized people make changes that shouldn't have been made the damage can be undone.

- **Availability**
Systems, access channels, and authentication mechanisms must all be working properly for the information they provide and protect to be available when needed.

**Note:** *In addition, other properties, such as authenticity, accountability, non-repudiation and reliability can also be involved. (ISO/IEC 27000:2009)*

- **Auditing & Accountability**
Basically keep tracking of everthing, like, who's been logging in when are they loggin in whose access this data.

- **Non-Repudiation**
Non-repudiation is the assurance that someone cannot deny the validity of something. Non-repudiation is a legal concept that is widely used in information security and refers to a service, which provides proof of the origin of data and the integrity of the data.

### **Security, Functionality and Usability balance**

There is an inter dependency between these three attributes. When **security goes up, usability and functionality come down**. Any organization should balance between these three qualities to arrive at a balanced information system.

<p align="center">
<img width="50%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/f14455ed4def635e1bc93b85657f43dbbf4a3127/triad2.png">
</p>

## <u>Types of Hackers</u>

<p align="center">
<img width="50%" src="https://www.simplilearn.com/ice9/free_resources_article_thumb/types-hacker.JPG">
</p>

> - **Black Hat** - Hackers that seek to perform malicious activities.
> - **Gray Hat** - Hackers that perform good or bad activities but do not have the permission of the organization they are hacking against.
> - **White Hat** - Ethical hackers; They use their skills to improve security by exposing vulnerabilities before malicious hackers.

**Script Kiddie / Skiddies** - Unskilled individual who uses malicious scripts or programs, such as a web shell, developed by others to attack computer systems and networks and deface websites. 

**State-Sponsored Hacker** - Hacker that is hired by a government or entity related.

**Hacktivist** - Someone who hacks for a cause; political agenda.

**Suicide Hackers** - Are hackers that are not afraid of going jail or facing any sort of punishment; hack to get the job done.

**Cyberterrorist** - Motivated by religious or political beliefs to create fear or disruption.

## <u>Hacking Vocabulary</u>

- **Hack value** - Perceived value or worth of a target as seen by the attacker.
- **Vulnerability** - A system flaw, weakness on the system (on design, implementation etc).
- **Threat** - Exploits a vulnerability.
- **Exploit** - Exploits are a way of gaining access to a system through a security flaw and taking advantage of the flaw for their benefit.
- **Payload** - Component of an attack; is the part of the private user text which could also contain malware such as worms or viruses which performs the malicious action; deleting data, sending spam or encrypting data.
- **Zero-day attack** - Attack that occurs before a vendor knows or is able to patch a flaw.
- **Daisy Chaining / Pivotting** - It involves gaining access to a network and /or computer and then using the same information to gain access to multiple networks and computers that contains desirable information. 
- **Doxxing** - Publishing PII about an individual usually with a malicious intent.
- **Enterprise Information Security Architecture** (EISA) - determines the structure and behavior of organization's information systems through processes, requirements, principles and models.

## <u> Threat Categories </u>
* **Network Threats**
  - Information gathering
  - Sniffing and eavesdropping
  - DNS/ARP Poisoning
  - MITM (Man-in-the-Middle Attack)
  - DoS/DDoS
  - Password-based attacks
  - Firewall and IDS attack
  - Session Hijacking

* **Host Threats**
  - Password cracking
  - Malware attacks
  - Footprinting
  - Profiling
  - Arbitrary code execution
  - Backdoor access
  - Privilege Escalation
  - Code Execution

* **Application Threats**
  - Injection Attacks
  - Improper data/input validation
  - Improper error handling and exeception management
  - Hidden-field manipulation
  - Broken session management
  - Cryptography issues
  - SQL injection
  - Phishing
  - Buffer Overflow
  - Information disclosure
  - Security Misconfigurations
