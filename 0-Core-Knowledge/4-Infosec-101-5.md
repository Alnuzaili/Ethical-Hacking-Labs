# <u>Introduction to Information Security & Penetration Testing</u>

> ⚠️ This module is fully theoretical and was extracted from [CEH Study Guide](https://github.com/Samsar4/CEH-v10-Study-Guide/) repo. Here you'll find some basic terms in 'InfoSec world'.


## <u>Incident Management Process</u>
*An incident is an event that could lead to loss of, or disruption to, an organization's operations, services or functions.*

***Incident management** is a term describing the activities of an organization to identify, analyze, and correct hazards to prevent a future re-occurrence.*

1. **Preparation:** Select people, assign rules, define tools to handle the incident.
2. **Detection & Analysis:** Determine an incident has ocurred (IDS, SIEM, AV, Someone reporting, etc).
3. **Classification and Prioritization:**
4. **Notification:** Identify minor and major incident; who and how to notify an incident.
5. **Containment:** Limit the damage; Isolate hosts; Contact system owners.
6. **Forensic Investigation:** Investigate the root cause of the incident using forensic tools; System logs, real-time memory, network device logs, application logs, etc;
7. **Eradicate & Recovery:** Remove the cause of incident; Patch if needed. Recovery: get back into production; Monitor affected systems.
8. **Post-incident Activities:** Document what happened and why; Transfer knowledge.

### Incident Response Team Duties

1. Managing security issues by taking a proactive approach towards the customer's security vulnerabilities 
2. Developing or reviewing processes and procedures that must be followed 
3. Managing the response to an incident and ensuring that all procedures are followed correctly in order to minimize and control the damage
4. Identifying and analyzing what has happened during an incident, including impact and threat
5. Providing a single point of contact for reporting seucirty incidents and issues
6. Reviewing changes in legal and regulatory requirements to ensure that all processes and procedures are valid
7. Reviewing existing controls and recommending steps and technologies to prevent future incidents
8. Establishing relationship with local law enforcement agency, gov. agencies, key partners and suppliers

### SIEM -  Security Information and Event Management
<p align="center">
<img width="90%" src="https://secureops.com/wp-content/uploads/2020/01/components-of-siem.jpg" />
</p>

*Collects data points from network, including log files, traffic captures, SNMP messages, and so on, from every host on the network. SIEM can collect all this data into one centralized location and correlate it for analysis to look for security and performance issues, as well negative trends all in real time.*

* **Aggregation**: Collecting data from disparate sources and organizing the data into a single format. Any device within a SIEM system that collects data is called collector or an aggregator.

* **Correlation**: Is the logic that looks at data from disparate sources and can make determinations about events taking place on your network. (Could be in-band or out-of-band, depending on the placement of the NIDS/NIPS).
	* **Alerts** - For notification if something goes bad.
	* **Triggering** - Exceeding thresholds.

* **Normalization**: Will actually create multiple tables / organize in such a way that the data can become more efficient and allows our analysis and reports tools to work better.

* **WORM - Write Once Read Many**: The concept being is that log files are precious, and a lot of times you might want to look at them in an archival way, so that we can use optical media like WORM drives to store them.

#### Most Popular SIEM Tools:

* **[Splunk](https://www.splunk.com/)**
	![splunk](https://www.splunk.com/content/dam/splunk2/images/screenshots/platform-journey/conflaunch/SS-UI-Light-Mode-frame.png)

<br>

* **[ArcSight](https://www.microfocus.com/en-us/products/siem-security-information-event-management/overview)**
	![arcsight](https://i.ytimg.com/vi/N7J0EwdbKF0/maxresdefault.jpg)

<br>

* **[ELK - Elastic Search, Log Stash and Kibana](https://www.elastic.co/what-is/elk-stack) (Open Source)**
	![elk](https://i.imgur.com/lydtCwn.png)

## <u>Identity and Access Management</u>
> **Identification, Authentication, Authorization**, and **Accounting** work together to manage assets securely.

### 1. **Identification**
*The information on credentials identifies the user.*

- **Example**: 
  - Your name, username, ID number, employee number, SSN etc.

### 2. **Authentication**
*“Prove you are the legitimate User". – Should always be done with Multifactor Authentication!*

* **Authentication Factors:**
	* Something you **know** (e.g. - password)
	* Something you **have** (e.g. - smart card)
	* Something you **are** (e.g. - fingerprint)
	* Something you **do** (e.g. - android pattern; manual signature)
	* **Somewhere** you are (e.g. - geolocation)
> 🛑 **Multi-factor authentication** *generally uses two of this examples (e.g. - Something you **Know(1)** and Something you **Have(2)**, never on same category*

### 3. Authorization concepts
*What are you allowed to access – We use Access Control models, what and how we implement depends on the organization and what our security goals are.*

* **Permissions**:
	* Applied to resources
* **Rights** / **Privileges**:
	* Assign at system level 
* **Authorization strategies**:
	* Least privileged
	* Separation of Duties

### 4. Accouting
*Trace an Action to a Subjects Identity:*
- Prove who/what a given action was performed by (non-repudiation); Logging

### Access Controls Models

<p align="center">
<img width="80%" src="https://security-architect.com/wp-content/uploads/FGA.png" />
</p>

* **Mandatory Access Control (MAC)**:
	* Every object gets a **label**
		- Confidential, secret, top secret, etc
	* The administrator decides who gets access to what security level; Users cannot change these settings
	* Used on old systems (e.g. Top Secret Gov. information)
* **Discretionary Access Control (DAC)**:
	* Used in most OS
	* Owner of the data defines access
	* Very flexible access control; Very weak security
* **Role-based Access Control (RBAC)**:
	* Access to resources is defines by a set of rules defined by a role in your organization/job function (Manager, Director etc)
	* Administrators provide access based on the role of the user
		- Rights are gained implicity instead of explicity
	* In Windows, use **Groups** to provide role-based access control
		- e.g. Admin Groups --> Rights and Perms,
		- Sales Group --> Rights and Perms


> ⚠️ **Access is defined by ACL, Access Control List**.
> ⚠️ **Implicity deny** prevents access unless specifically permitted. 

