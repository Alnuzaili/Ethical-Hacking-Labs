# <u>Introduction to Information Security & Penetration Testing</u>

> ⚠️ This module is fully theoretical and was extracted from [CEH Study Guide](https://github.com/Samsar4/CEH-v10-Study-Guide/) repo. Here you'll find some basic terms in 'InfoSec world'.


## <u> Attack Vectors </u>
*Path by which a hacker can gain access to a host in order to deliver a payload or malicious outcome*

- **APT - Advanced Persistent Threats**
  - An advanced persistent threat is a stealthy threat actor, typically a nation state or state-sponsored group, which gains unauthorized access to a computer network and remains undetected for an extended period; Typically uses zero day attacks.
- **Cloud computing / Cloud based technologies**
  - Flaw in one client's application cloud allow attacker to access other client's data
- **Viruses, worms, and malware**
  - Viruses and worms are the most prevalent networking threat that are capable of infecting a network within seconds.
- **Ransomware**
  - Restricts access to the computer system's files and folders and demands an online ransom payment to the attacker in order to remove the restrictions.
- **Mobile Device threats**
- **Botnets**
  - Huge network of compromised systems used by an intruder to perform various network attacks
- **Insider attacks**
    - Disgruntled employee can damage assets from inside.
    - Huge network of compromised hosts. (used for DDoS).

- **Phishing attacks**
- **Web Application Threats**
  - Attacks like SQL injection, XSS (Cross-site scripting)...
- **IoT Threats**


## <u>Attack Types</u>
### 1. Operating System
*Attacks targeting OS flaws or security issues inside such as guest accounts or default passwords.*
>  - **Vectors**: Buffer overflows, Protocol Implementations, software defects, patch levels, authentication schemes

### 2. Application Level
*Attacks on programming code and software logic.*
>  - **Vectors**: Buffer overflows, Bugs, XSS, DoS, SQL Injection, MitM

### 3. Misconfiguration
*Attack takes advantage of systems that are misconfigured due to improper configuration or default configuration.*

>  - **Examples**: Improper permissions of SQL users; Access-list permit all

### 4. Shrink-Wrap Code
*Act of exploiting holes in unpatched or poorly-configured software.*
>  - **Examples**: Software defect in version 1.0; DEfect in example CGI scripts; Default passwords 

## <u>Vulnerabilities</u>

- **CVSS - Common Vulnerability Scoring System** [[+]](https://nvd.nist.gov/vuln-metrics/cvss)
  - Places numerical score based on severity
  - ![cvss](https://3.bp.blogspot.com/-5V1cb_wTvsk/Wl78iF4Sd8I/AAAAAAAAF7U/KmK4pMXi54YworDgh4uI8aZtHgy0bbznQCLcBGAs/s1600/CVSS.png
  )
- **CVE – Common Vulnerabilities and Exposures** [[+]](https://cve.mitre.org/)
  - Is a list of publicly disclosed vulnerabilities and exposures that is maintained by MITRE.
  - ![cve](https://i0.wp.com/gbhackers.com/wp-content/uploads/2016/10/cve.png?resize=486%2C408&ssl=1)
- **NVD - National Vulnerability Database**  [[+]](https://nvd.nist.gov/)
  -  is a database, maintained by NIST, that is fully synchronized with the MITRE CVE list; US Gov. vulnerabilities repository.

### Vulnerability Categories

- **Misconfiguration** - improperly configuring a service or application
- **Default installation** - failure to change settings in an application that come by default
- **Buffer overflow** - code execution flaw
- **Missing patches** -  systems that have not been patched
- **Design flaws** - flaws inherent to system design such as encryption and data validation
- **Operating System Flaws** - flaws specific to each OS
- **Default passwords** - leaving default passwords that come with system/application


## <u>Pen Test Phases (CEH method)</u>
1. **Pre-Attack Phase** - Reconnaissance and data-gathering.
2. **Attack Phase** - Attempts to penetrate the network and execute attacks.
3. **Post-Attack Phase** - Cleanup to return a system to the pre-attack condition and deliver reports.


## <u>The Five Stages of Ethical Hacking</u>

### 1. **Reconnaissance**
*Gathering evidence about targets*; There are two types of Recon:
- **Passive Reconnaissance**: Gain information about targeted computers and networks **without direct interaction with the systems**.
    - e.g: Google Search, Public records, New releases, Social Media, Wardrive scanning networks around.
- **Active Reconnaissance**: Envolves direct interaction with the target.
    - e.g: Make a phone call to the target, Job interview; tools like Nmap, Nessus, OpenVAS, Nikto and Metasploit can be considered as Active Recon.

### 2. **Scanning & Enumeration**
*Obtaining more in-depth information about targets.*
- e.g: Network Scanning, Port Scanning, Which versions of services are running.

### 3. **Gaining Access**
*Attacks are leveled in order to gain access to a system.*
- e.g: Can be done locally (offline), over a LAN or over the internet.
  - e.g(2): Spoofing to exploit the system by pretending to be a legitimate user or different systems, they can send a data packet containing a bug to the target system in order to exploit a vulnerability.
  - Can be done using many techniques like command injection, buffer overflow, DoS, brute forcing credentials, social engineering, misconfigurations etc.
  
### 4. **Maintaining Access**
*Items put in place to ensure future access.*
- e.g: Rookit, Trojan, Backdoor can be used.

### 5. **Covering Tracks**
*Steps taken to conceal success and intrusion; Not be noticed.*
  - e.g: Clear the logs; Obfuscate trojans or malicious backdoors programs.


## Three Types of Active Defense 
- **Annoyance**
  - Involves tracking a hacker and leading him into a fake server, wasting his time — and making him easy to detect.
- **Attribution**
  - Identify an attacker; Uses tools to trace the source of an attack back to a specific location, or even an individual hacker.
- **Attack**
  - That is most controversial. To “hack back,” a company accesses an alleged hacker’s computer to delete its data or even to take revenge. Both of these steps are considered illegal. 