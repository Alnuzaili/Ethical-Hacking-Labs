# <u>Introduction to Information Security & Penetration Testing</u>

> ⚠️ This module is fully theoretical and was extracted from [CEH Study Guide](https://github.com/Samsar4/CEH-v10-Study-Guide/) repo. Here you'll find some basic terms in 'InfoSec world'.


## Data Loss Prevention (DLP)
Data Loss Prevention (DLP) is the practice of **detecting and preventing data breaches, exfiltration, or unwanted destruction of sensitive data**. Organizations use DLP to protect and secure their data and comply with regulations.

* The DLP term refers to defending organizations against both data loss and data leakage prevention. 

#### Organizations typically use DLP to:

- Protect Personally Identifiable Information (PII) and comply with relevant regulations
- Protect Intellectual Property critical for the organization
- Achieve data visibility in large organizations
- Secure mobile workforce and enforce security in Bring Your Own Device (BYOD) environments
- Secure data on remote cloud systems

<p align="center">
<img width="90%" src="https://miro.medium.com/max/720/1*FG9LR51eySVRQJUjhVv-9A.png" />
</p>

## Data Backup
Data backup plays a crucial role in maintaining business continuity by helping org. recover from IT disasters, security breaches, application failures, human error, etc. 

All regulatory compliance such as COBIT, SSAE, SOCII, PCI-DSS, HIPPA, SOX, FINRA, FISMA, GDPR, etc. require business to maintain data backups of critical data for specified duration.

### Backup Strategies
1. Identifying the critical business data
2. Selecting the backup media
3. Selecting a backup technology
4. Selecting the appropriate RAID levels
5. Selecting an appropriate backup method

### 3 Backup methods
####  1. Cold backup 🔵

<img width="40%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/29c5e018095b135baec32aaece84a900a43b23ca/cc-cold.png"/>

- **Empty site, no hardware, no data, no people**
- **It takes weeks to bring online**
- Basic office spaces (e.g building, chairs, AC...)
- No operational equipment
- Cheapest recovery site

#### 2. Warm backup 🟡

<img width="40%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/29c5e018095b135baec32aaece84a900a43b23ca/cc-warm.png"/>

- **Somewhere between cold and hot - Just enough to get going (Big room with rack space, you bring the hardware)**
- Hardware is ready and waiting - you bring the software and data
- **It takes days to bring online**
- Operational equipment but little or no data

#### 3. Hot backup 🔴

<img width="40%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/29c5e018095b135baec32aaece84a900a43b23ca/cc-hot.png"/>

- **Exact replica of production systems**
- Applications and software are constantly updated
- Flip a switch and everyting moves
- **It take hours to bring online**
- Real-time synchronization
- Almost all data ready to go - often just a quick update
- Very expensive


## <u>Penetration Test - Basics</u>
> **This topic will be covered with details in [Chapter 14 - Pentesting](https://github.com/Samsar4/CEH-v10-Study-Guide/blob/master/modules/14-Pentesting.md).**

*A penetration test, colloquially known as a pen test, pentest or ethical hacking, is an authorized simulated cyberattack on a computer system, performed to evaluate the security of the system.*

> ⚠️ **Not to be confused with a vulnerability assessment.**

- Clearly defined, full scale test of security controls
- Phases
  - **Preparation** - Contracts and team determined
  - **Assessment** - All hacking phases (reconnaissance, scanning, attacks, etc.)
  - **Post-Assessment** - Reports & conclusions
- Types
  - **Black Box** - Done without any knowledge of the system or network.
  - **White Box** - When the attacker have complete knowledge of the system provided by the owner/target.
  - **Gray Box** - When the attacker has some knowledge of the system and/or network
