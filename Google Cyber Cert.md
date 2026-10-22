# `Course 1: Foundations of Cybersecurity
# **Module 1**
- Personally identifiable information (PII) 
- (SPII) more important one
- SIEM information monitoring 
- transfer i.e communication
- technical i.e programming

## [Glossary](https://docs.google.com/document/d/1Feb8pHRY-blnpaLOohds2esd6IWdCIp-ikG7G_omSj4/template/preview?resourcekey=0-YHcAISkCiqGDq5KwO6yNeQ)

---

# **Module 2**

### Types of Attacks:
- brain virus - pirated copy of software (CD), any disk next put in will become infected
- Moore's worm - tally the internet, but instead kept loading itself onto computers thus frying them
- Love letter attack - email attack, sent itself to everyone and stole passwords (ILOVEYOU virus)
Social Engineering - manipulation of people via communication 
	- Social media: [[OpenSource Intelligence OSINT]] 
	- Watering Hole attack: a attack on a website used by employees
	- USB baiting: [[Rubber Ducky Hack]]
	- Physical Social Engineering: Impersonates employee
Phishing - social attack through emails to trick people
	- Business Email Compromise (BEC): email request for company info
	- Spear Phishing: "Trusted" email 
	- Whaling: "Trusted" email to a POI (person of interest)
	- Vishing: Fake phone call
	- Smishing: "Trusted" text message
Malware:
	- Virus: needs to be downloaded
	- worm: doesn't need to be downloaded, spreads automatically 
	- Ransomware: ransom
	- Spyware: spy
Cryptography:
	- Birthday: bruteforce attack

### CISSP Eight Domains
- **Security and Risk**: goals, mitigation and compliance
- **Asset Security**: Secure, store, maintain and destroy
- **Security architecture** and engineering: optimize data security and firewalls
- **Communications and network security**: secure physical and wired networks, network policy
- **Identity and Access management (IAM)**: police officer amongst employees
- **Security assessment and testing**: collect data and security audits
- **Security Operations**: conduct investigations
- **Software development security**: secure coding in the lifecycle

---

# **Module 3**
### Framework: 
- Security Frameworks
	- protecting PII
	- secure financials
	- identify weakness 
	- manage risk
	- align security with business
**Frameworks**
1. Identify security goals: be compliant with (GDPR) laws 
2. Setting Guidelines to achieve goal: develop new policies to be compliant 
3. Implementing process: procedure to apply to policies on by user and company
4. monitor and communicate results: report effectiveness

### CIA Triad (foundational):
(consider risk)
- Confidentiality: only authorized people have access/data
- Integrity: data is reliable/correct
- Availability: data can be accessed

---

# **Module 4**

**Tools** 
- SIEM tools (security management): collects and reviews logs (SPLUNK, Chronical)
- playbooks: manual that provides details about actions
- network protocol analyzers (packet sniffer): capture and analyze data traffic on a network (tcp dump, Wireshark)
- Linux operating system: 
- Programming Languages: automate tasks (Linux, SQL, and python)

**Create a [[Portfolio Ideas]]**
https://youtu.be/QsM6b5yix0U?si=iozrJfUgMTbfGe_n

---

# `Course 2: Manage Security Risks
# **Module 1**

### **[[NIST Risk Management Framework (RMF)]]:** 
- Prepare: activities necessary to manage security before a breach
- Categorize: develop risk manage tasks
- Select: choose customize and capture documentation
- Implement: implement security and privacy plans
- Assess: determine if controls are implemented correctly 
- Authorize: being accountable for risks (reports, plans of actions, goals)
- Monitor: be aware of how systems are operating

---

# **Module 2**

**Security Frameworks:** guidelines used to build plans to mitigate risk and and protect data/privacy

### Security Controls: (for specific)
- Encryption: convert data into encoded format
- Authentication: verify who someone is
- Biometrics: are unique physical attributes (Finger, voice and eye scan)
- Authorization: is proof someone has access to info

### **[[NIST Cybersecurity Framework (CSF)]]:** 
(voluntary framework)
- Identify: management of risk and its effect on an organization
- Protect: strategy used to implement procedures
- Detect: identify incidents and improve monitoring
- Respond: contain, neutralize and analyze security implements and then improve security.
- Recover: returning affected systems back to operation

### OWASP
Open
Web
Applications
Security 
Project
- Minimize attack surface area: phishing emails and weak passwords
- Principle of least privilege 
- Defense in Depth: multiple security controls (MFA, Firewalls, intrusion detection)
- Separation of duties: no one person should have too many privileges
- Keep security simple (simpler = better)
- Fix security issues correctly: identify the root cause and correct/test
Bonus:
- Establish secure defaults: its extra work to become insecure
- Fail securely: when controls fail it defaults to secure options
- Don't trust services: verify integrity of third-party-services data
- Avoid security by obscurity: dont rely on secret code, but rather defense in depth

### Security audit: 
A review of controls, policies, and procedures
- External: //not entry level//
- Internal: (identify risk, assess controls and correct compliance issues)
	- Establish Scope/Goals: do security audit ^, and to follow frameworks
	- Risk Assessment: identify risks, threats and vulnerabilities 
		- Risk: anything that can impact confidentially, integrity, or availability
		- Threat: any circumstance or event that can impact assets
		- Vulnerability: any weakness that can be exploited
	- Controls Assessment: 
		- **administrative:** people solutions
		- **technical:** software solutions
		- **physical:** physical solutions
	- Assessing Compliance: 
	- Communicating Results: 

Audit questions:
- what is the audit meant to achieve?
- which assets are most at risk?
- are current controls sufficient to protect those assets?
- what controls and compliance regulations need to be implemented?

`Security Audit: Complete

---

# **Module 3**

### Log Types:
- Firewall Log: records attempts or established connections to the internet
- Network Log: record of devices on the network and between themselves
- Server Log: service info such as websites, emails or file shares. also includes actions like login, password and username requests. 

### Types of SIEM Tools:
- Self-hosted: required to install, operate and maintain the tool using their own hardware. 
	- Pro's: for confidential data
- Cloud-hosted: maintained and hosted by the SIEM providers, using the internet. 
	- Pro's: don't have to invest in making your own, and use the cloud
- Hybrid: 
	- Pro's: Leverage the benefits of the cloud and maintain physical control of confidential data


[[Splunk]]: tool to retain, analyze and search a org's log data in real-time
- Splunk Enterprise (Self-hosted)
- Splunk Cloud (Cloud-hosted)

[[Chronicle]]: (Cloud-native) tool designed to retain, analyze, and search data

Indicators of Compromise (IOC)

---

# **Module 4**

### **Incident Response Playbook (6 phase):**
- **Preparation**: to mitigate the impact of a likelihood risk and impact (assign roles)
- **Detection** and Analysis: determine if a breach has occurred and determine its magnitude
- **Containment**: prevent further damage (high priority)
- **Eradication and Recovery**: complete removal of artifacts of the incident. Restore effected environment to a secure state,
- **Post-Incident Activity**: Documentation, Communication, and teaching lessons. Find root cause and improve posture
- **Coordination**: record and share info 


---


---
# `Course 3: Network Security

# **Module 1**
### Network Basics:

Local Area Network (LAN): local area
Local Area Network (WAN): wide area

**Hub**: device that broadcasts info to every device on the network
**Switch**: makes connections between specific devices, (more secure than hub)
**Router**: network device that connects multiple networks. 
**Modem**: device that connects a router to the internet

**Virtualization Tools**: software that performs the network operations 

**Cloud Computing**: using remote servers via the internet
**Cloud Network**: a collection of remote servers that store data via the internet

**Data Packet**: A piece of info with a
	- Header: IP / MAC / Protocol Number
	- Body: The message
	- Footer: Signature or ending
**Packet Sniffing**: Capturing and inspecting packets 

**Bandwidth**: amount of data received per second
**Speed**: rate at which packets are received or downloaded

### Transmission Control Protocol and Internet Protocol (TCP/IP Model):
- **TCP:** is a transmission control protocol to allow two devices to connect
- **IP:** is the internet protocol that is used for routing and addressing packets 
	- IPv4 Fields: Version (VER), IP Header Length (HLEN or IHL), Type of Service (ToS), Total Length, Identification, Flags, Fragmentation offset, Time to Live (TTL), Protocol, Header Checksum, Source IP Address, Destination IP Address, Options
	- IPv6
- **Port:** is a software based location that organizes the data sending
- **Port Numbers:**
	- 25 -- email
	- 443 -- secure internet communication
	- 20 -- large files
- MAC Address: alphanumerical tag assigned to each device

 **TCP/IP Model Layers:** 
- **Network Access Layer**: creating data packets and transmissions (ethernet cables and switches)
- **Internet Layer:** Data packets get IP addresses and delivered 
- **Transport Layer:** Protocols for the control of traffic through a network (TCP/UDP)
- **Application Layer:** organizes and tells how data packets will interact with devices (email services) (HTTP/TLS/DNS)

### Open Systems Interconnection (OSI) Model:
-  **Layer 7** (*Application layer*): Involves the everyday user, includes network protocols and software.
- **Layer 6** (*Presentation layer*): Data Translation and encryption (e.g. SSL)
-  **Layer 5** (*Session layer*): Is like a gate for connections that also authenticates and create checkpoints. When a open session is established data can pass then it closes them once its complete. 
-  **Layer 4** (*Transport layer*): Controls the speed of data and can break up data so it can be sent faster.
-  **Layer 3** (*Network layer*): Reads where data should be sent
-  **Layer 2** (*Data link layer*): Organizes sending and receiving data
-  **Layer 1** (*Physical layer*): Physical aspects of a network (hub, modem, wires)

---

# **Module 2**

**Network Protocols:** Rules used by a network to describe the order and structure of the data
### Protocols
Communication Protocols
- Transmission Control Protocol (TCP)
	- Connect devices with three-way handshake
	- *Transport Layer*
- User Datagram Protocol (UDP)
	- less reliable because it doesn't check connection (faster than TCP)
	- *Transport Layer*
- Hypertext Transfer Protocol (HTTP)
	- To be replaced with HTTPS (Insecure)
	- *Application Layer*
- Domain Name System (DNS)
	- Is a protocol that converts domain names into IP addresses
	- *Application Layer*

Management Protocols
- Simple Network Management Protocol (SNMP)
	- monitors and manages 
	- *Application Layer*
- Internet Control Message (ICMP)
	- reports on data transmission errors (e.g. /ping)
	- *Internet Layer*
- Dynamic Host Configuration Protocol (DHCP)
	- assigns a unique IP address and gateway to devices. 
	- DHCP *server* UDP port is 67 while DHCP *client* is port 68
	- *Application Layer* 

**Security Protocols**
- Hypertext Transfer Protocol Secure (HTTPS)
	- secure connection between client and server uses SSL/TLS
	- *Application Layer*
- Secure File Transfer Protocol (SFTP)
	- secure version of FTP, uses SSH to transfer files
	- *Application Layer*

### Ports for Stuff
DHCP
- UDP port 67 (servers)
- UDP Port 68 (clients)
Address Resolution Protocol (ADR)
- since MAC address stays the same per network interface card, it takes info sent to the IP and sends it to the correct MAC address
Telnet
- sends info in cleartext, like a unsecure SSH
- TCP Port 23
- *Application Layer* 
Post Office Protocol (POP)
- most likely POP3 and it manages and retrieves emails from mail server. 
- TCP/UDP Port 110 for unencrypted 
- TCP/UDP Port 995 for encrypted (SSL/TLS)
-  *Application Layer* 
Internet Message Access Protocol (IMAP)
- downloads eaaders of emails and message content
- TCP Port 143 for unencrypted 
- TCP Port 993 for encrypted (SSL/TLS)
Simple Mail Transfer Protocol (SMTP)
- Transmit and route emails using software Message Transfer Agent (MTA)
- TCP/UDP Port 25 for unencrypted 
- TCP/UDP Port 587 for encrypted (TLS)

### WiFi
- IEE 802.11 (WiFi)
- WiFi Protected Access (WPA): wireless security Protocol for devices
-  WEP
- WPA2
- WPA3

- **Firewall**: monitors to and from your network
	- Port Filtering: allows or blocks certain ports
	
	- Hardware Firewall: inspects all packets
	- Software Firewall: same as hardware but not a physical device (cheaper but process burden)
	- Cloud-Based Firewall: firewall as a service (FWAaS)
	
	- Stateful: tracks information passing through and filters threats 
	- Stateless: doesn't track and operates on predefined rules
	- Next Generation Firewall (NGFW): 
		- Deep packet inspection
		- Intrusion protection
		- Threat intelligence

- **Virtual Private Network (VPN):** network security service that's changes your public IP address, and keeps your data private
	- Encapsulation: protects your private data in other data
	- Connection Methods: Remote Vs. Site-to-Site
		- Remote Access: Connect device to VPN through internet (simple)
		- Site-to-Site: Used for enterprise to connect their network to other networks (difficult to configure)

 - **Security Zone**: segment of a network that protects internal from the internet
	- Controlled Zone: subnets 
		- Demilitarized Zone (DMZ): web, proxy, DNS, and Email Servers
		- Internal Network: 
		- Restricted Zone: only accessible with certain privileges 
	- Uncontrolled Zone: networks outside a organization control

- **Proxy Server**: Dedicated server that forwards information (uses temp data=more security)
	- Forward Proxy Server: regulates and restricts a persons access to the internet
	- Reverse Proxy Server: regulates and restricts a internet access to the internal server
	- Email Proxy Server: Filters spam email, checks if a email was forged 

---

# **Module 3**

### Network Intrusion Attacks: 
- **Malware:**
- **Spoofing:** pretend to be someone they are not
- **Packet sniffing:** capture and inspect network data or modify it
- **Packet flooding:** (SYN flood attack) pose as a TCP connection
- **Backdoors:** Intentional weakness left by administrators or attackers to have persistent access
- **DoS/DDoS attack:** An attack that floods a network with traffic

*Harm Effects: 
- *Leaking Data*
- *Damage Reputation*
- *Impact Customer Retention*
- *Loss Money/Time*
- *Public Safety*

TcpDump: used to capture network communications and collect statistics about a network and what ports are broken

### Packet Sniffing 
- Passive: Read only
- Active: Read/Write
- Counter: VPN, Dont use free Wifi
### IP spoofing 
- On-path attack: (MiTM) they are between two devices and steals/alters packets
- Replay attack: delays a packet or repeats it at another time.
- Smurf attack: sniffs the IP address and floods it with packets (DDOS + sniffing)

#### Brute Force Attack
- Simple: guessing credentials
- Dictionary: list of commonly used credentials
- Reverse: start with a single credential and try it in multiple systems
- Credential stuffing: which uses credentials from data breaches
### OS Security Hardening
- Salting/Hashing: Hashing is to convert information into a value to determine its integrity (impossible to decrypt) and salting is adding random characters.
- Multi-factor authentication (MFA) and two-factor authentication (2FA): Password + other factors
- CAPTCHA: Turing test
- Password Policies: standardize good password practices

### Network Hardening
- Port Filtering: only the ports needed should be allowed
- Subnets: so viruses cant spread across the network
- Encryption: Most up to date encryption
- Firewalls: set rules
- Intrusion Detection System (IDS): monitor and alerts possible intrusions
- Intrusion Prevention System (IPS): takes action to stop intrusive activity

### Network Security in The Cloud
- Identity Access Management (IAM): organize digital identities
- Hypervisor: (type 1) a virtual machine running on hardware
- Baselining: default configurations

---
# `Course 4: Linux and SQL

### OS: Linux
- A OS connects the user to the hardware
	1. Turn on computer
	2. Bios or UEFI run bootloader
	3. Bootloader boots OS
- GUI (Graphical User Interface)
	- Uses icons on the screen (Easier)
- CLI (Command Line Interface)
	- Text based user interface (More powerful)

### Linux Architecture
- User - chair warrior
- Applications/Program - program that does a specific task
- Shell - command line interpreter
- Filesystem Hierarchy Standard (FHS) - A way to store data
- Kernel - Manages and processes memory

### Distributions 
- Kali linux - many pre-installed tools
- Ubuntu - 
- Parrot
- Red Hat
- CentOS

### SQL (Structure Query Language)
: program language used to RWX ( Read Write eXecute )
- Log : records
- Query : request for data
- Filter : sort by a certain quality

SQL Commands: 
- Where
- From
- LIKE
- SELECT
- east% --> east-290

SQL Joins: 
- Inner Join: combines data, for matching data between
- Left/Right Join: full table, plus matching of the other side
- Full Outer Join: everything

Aggregate Functions: perform calculations over the data and return results.
- Count: returns number of rows 
	- e.g. SELECT COUNT(column)
- AVG: returns average of the data in a column
- SUM: returns the sum of a column

---
# `Course 5: Assets, Threats, and Vulnerabilities

# **Module 1**
- Asset: item that has value 
	- Asset Management: you can only protect things you take account for
	- Asset inventory: catalog of assets 
	- Asset Classification: classifying the importance of assets
		- public - anyone
		- internal - anyone in org
		- confidential - by people in specific project
		- restricted - highly sensitive and must be protected (need to know)

Data: translated, process or stored information
 - In use: being accessed 
 - In transit: moving
 - In rest: not being accessed 

Risk Categories
- damage
- disclosure
- Loss of information

1. Policy: set of rules that reduce risk and create a procedure
2. Procedure: step by step instructions for a plan
3. Standards: 

Compliance: is adherence to following rules

**[[NIST Cybersecurity Framework (CSF)]]:*
Levels (1-4)
1. bare-minimum
2. good
3. better
4. Exemplary
---
# **Module 2**
Security Controls: Safeguards to prevent risk
1. Technical - Encryption and  Authorization
2. Operations - day to day and incident response
3. Managerial - policies, standards and procedures

**Information Privacy**: protection of unauthorized access and distribution of data
**Information security** (InfoSec): refers to the practice of keeping data in all states away from unauthorized users.

**Data Owner**: person who decides who can access, edit, use or destroy data
**Data Custodian**: anyone or anything responsible for safe handling, transport and storage of info
**Data steward**: the person or group that maintains and implements data governance policies set by an organization

Data Lifecycle
- Collect
- Store
- Use
- Archive
- Destroy

**Cryptography**: transform data into something the user cannot understand
- Plain text: readable 
- Cypher text: un-readable
Algorithm: set of rules to solve a problem
Cipher: algorithm that encrypts info

Public Key Infrastructure (PKI): an encryption framework that secures the exchange of info online
1. Exchange of encrypted information
	- Asymmetric: use of public and private keys 
	- Symmetric (faster/less secure): use of a *single* key
2. Establish trust by using a system of digital certificates
	- Digital Certificate: a file that verifies the identity of a key holder

"Machines should never make the final decision, because they cannot be held accountable."\

Hash Files are used for integrity
Non-repudiation: the idea that authenticity of information cant be denied

AAA framework
- Authentication: 
	1. Knowledge: Something they know (password)
	2. Ownership: Something they possess (one time passcode (OTP))
	3. Characteristic: Something they are (biometrics)
- Authorization: privileges
	- Principle of least privilege
	- Separation of Duties: users shouldn't be given permissions to abuse a system
- Accounting: monitoring
	- Session: is a sequence of network HTTP basic auth requests and responses associated with the same user
		- Session ID: unique token to identify a user to a device
		- Session Cookie: a token to validate a session and how long it should last
		- Session Hijacking: when someone takes a ID

- Single Sign One (SSO): assigns all logins through one
	1. improves user experience
	2. lower costs (streamline)
	3. improves overall security
Multi-Factor Authentication (MFA): uses two or more techniques of authentication

Oauth: is an open-standard authorization protocol that shares designated access between applications
- API token: small block of information about a client
Basic Auth: the technology used to establish a user's request to access a server
- ID?
---
# **Module 3**

Vulnerability Management: stopping threats before they can become a problem
1. identify vulnerabilities
2. consider exploits
3. prepare defenses against threats
4. evaluate the defenses

0-day Exploit: a new exploit unseen before

Defense in Depth (castle approach): layered security
1. Perimeter Layer: user authentication layer
2. Network Layer: firewalls
3. Endpoint Layer: describes devices
4. Application Layer: MFA
5. Data Layer: info that is stored transferred or in use

Exposure: is a mistake that can be exploited
Common Vulnerability and Exposure List (CVE List): dictionary 
MITRE Corp: collection of non-profit research found in the 1999

CVE list criteria
1. Independent of other issues
2. Recognized as a potential risk
3. Submitted with support evidence
4. Only affect one code base

Common Vulnerability Scoring System (CVSS):
1-4 low risk
9+ should be addressed right away

Vulnerability Assessment: internal review process of a security system
1. Identification: find vuln / understand its state
2. Vulnerability Analysis: source of a problem
3. Risk Assessment: score is assigned
4. Remediation: address the vulnerabilities / patch

Attack Surface: all the potential vulnerabilities that a threat actor could exploit
Attack Vectors: specific parts a person may attack
Threat Actors:
- Competitors
- State Actors
- Criminal Syndicates
- Insider Threats
- Shadow IT
---
# **Module 4**

Social Engineering: uses human error and manipulation
1. prepare: gather intel
2. Establish trust: pre-texting
3. Persuasion: manipulation (they can use specific vocabulary)
4. Disconnect: disappear
Prevent Social
- Implement managerial controls
- Staying informed of trends
- Sharing what you know

Phishing Kit -
- malicious attachments
- Fake data-collection Forms
- Fraudulent web links

Smishing: use of a text message impersonating something/someone
Vishing: speak like someone they are not (could us AI voice)

Phishing security
- Anti-phishing policies
- Employee training
- Email Filters
- Intrusion prevention

Cryptojacking: installs software to illegally mine

Cross-site Scripting (XSS): injection attack that inserts code (HTML and javascript)
1. Reflected: script is sent to a server and activated during a server response (fake out link)
2. Stored: injected directly on a server (just visiting)
3. DOM-based: a script can be in the url

SQL Injection: attacks the part of a website that accepts user input
- In-band: uses a input channel to execute code
- Out-of-band: use a not direct channel to access information
- Inferential: cannot see the results, but analyze the behavior of a system
To Prevent:
- Prepared statement: executes user statement before passing it into a server, validating the input and stopping a injection.
- Input Sanitization: removes input that can be interpreted as code 
- Input Validation: user input meets expectations

Threat Modeling: process of identifying vulnerabilities and how they can be exploited
1. Define Scope: determine what your building by getting the inventory
2. Identify Threats: get all the threat actors
3. Characterize the Environment: consider how people interact with the assets 
4. Analyze Threats: examine existing protection and its gaps
5. Mitigate Risk: plan to defend against threats
6. Evaluate Findings: documentation and fixes are applied and recorded

Common Frameworks: 
- Stride
- Trike
- VAST
- P.A.S.T.A. (Process for Attack Simulation and Threat Analysis)
	1. define business and security objectives
	2. define technical scope
	3. decompose the application (data flow diagram)
	4. perform a threat analysis
	5. vulnerability analysis
	6. Conduct attack modeling


Attack Tree: diagram that maps threats to assets

---
# `Course 6: Sound the Alarm: Detection and Response

# **Module 1**

Event is a observable occurrence

NIST Incident Response Lifecycle (cyclical)
- Preparation
- Detection and Analysis
- Containment, Eradication. and Recovery
- Post-incident Activity
Computer security incident response teams (CSIRT)

The 5 W's of a incident
- Who triggered
- What happened
- When 
- Where it took place
- Why it occurred 

SIEM tool
1. Collect and aggregate Data
2. Normalize Data
3. Analyze Data

# **Module 2**
\
Network Traffic Flow
Packet Sniffer
Packet Analysis

network
- traffic = amount
- data = specific data

Indicators of Compromise (IOC): Observable evidence that suggests signs of a intrusion incident

Defensive Measures: 
1. Prevent Attacker Access (MFA)
2. Monitor Network Activity
3. Protect Assets
4. Detect and stop exfiltration

Components of a Packet
- header
- payload
- Footer

Network Protocol Analyzer(Packet Sniffer): capture and analyze data traffic
Packet Capture (p-cap): file containing data packets that are intercepted 

Packet Header (IPv4)
1. Header
	- Version: tells ipv version
	- IHL (Internet Header Length): length
	- TOS (Type of Service): how to handle a packet
	- Total Length: length of the *whole* packet 
2. Fragmentation
	- Identification
	- Flags
	- Fragment Offset
3. 
	- TTL (Time to Live) 


TcpDump is a cli network packet analyzer


# **Module 3**

Life-cycle of a Security Incident:
1. Preparation
2. Detection and Analysis: 
	- not all events are incidents but all incidents are events
	- investigation and validation of alerts
	- impossible to detect everything / high volume / false positive
3. Containment, Eradication, and Recovery
	- Contain: limit the malware's ability to spread
	- Eradicate: remove all dependencies of the malware and patching
	- Recovery: repair files
4. Post-Incident Activity
	- review areas for improvement 
	- Final Report: comprehensive review of the incident


Crowd-sourcing: if one company gets hacked they can alert everyone of the threat to stop others from being hacked.

Documentation:
- Transparent / evidence
- Standardization 
- Clarity

Chain of Custody: documenting evidence possession, and control
- validation and integrity ++

playbook types:
- Non automated: step by step actions
- Automated: SOAR and SEIM tools
- Semi automated: mixed

Triage: prioritize incidents based on their priority
1. Receive and assess
2. Assign priority
3. Collect and analyze

Business Continuity Plan (BCP): plans to keep going while experiencing a disruption 
- Hot Site: a site that is able to be used immediately when a main website goes down 
- Warm Site: like a hot site however may not be completely functional
- Cold Site: a backup facility that may have the capability to run a site but is not setup

# **Module 3**
- read and analyze logs
- interpret signatures
- search SIEM tools

Types of Logs: 
- Network Logs
- System Logs
- Application Logs
- Security Logs
- Authentication Logs

log:
- time stamps (date and time)
- system characteristics (IP and hardware)
- description of even (event and reaction)

Types of Logs:
- Syslog: protocol and log format
	- Protocol: log server port 514 for plain-text and port 6514 for encrypted.
	- Service: log forwards multiple logs into one remote server
	- Log Format: Header -> structured Data -> message
- JavaScript Object Notation (JSON): easy to read
- Extensible Markup Language (XML): uses commas to separate info
	- Tags: you add a start and end tag (<tag*> *Enter Data* </tag*>) used to identify
	- Elements: Data and the tag 
	- Attributes: extra data or second part of a tag
- CSV (Comma Separated Value): separated by commas 
- CEF (Common Event Format): separated by pipes

Intrusion Detection Systems (IDS): 
- Host-Based (HIDS): a IDS that monitors its host / endpoint
- Network-Based (NIDS): monitors network traffic 
	- Action: Determines if rule criteria is met
		- Alert
		- Pass 
		- Reject
		- Drop
	- Header:
		- Source and IP
		- Source and Destination
		- Protocols
		- Traffic Destination
	- Rule options:

**Signature Analysis:** detection method used to find events of interest
- Advantage: 
	- low false-positives
- Disadvantages:
	- has to be updated
	- can be evaded 
	- inability to detect unique CVE
**Anomaly-based Analysis**: detects strange behaviour, it has to be trained before detecting
- Advantage: 
	- ability to detect new threats
- Disadvantage: 
	- high rate of false-positives
	- if there's a preexisting compromise it wont be able to detect

IDS <-> Signature analysis
IDS monitors then checks by the signature analysis, if its bad then it will be logged

Splunk: Search P Language (SPL)

Chronicle: (Yala-L)

---
# `Course 7: Automate Cybersecurity Tasks with Python

# Module 1

Python advantages: 
- Resembles human language
- Standard Guidelines
- Online Support
- Built-in code

Integrate Development Environment (IDE)
Command Line Interpreter (CLI)

Data type: 
- String: `"This is a string" or 'This string'
- Float: `11.00
- Integer: `10
- Boolean: True or False
- List: `["this", "is", "a", "list"]
- Tuple (memory efficient): `("this", "is", "a", "tuple")
- Dictionary: `{1: "East", 2: "West", 3: "North", 4: "South"}
- Set: same as a list but no two values can be the same

If/Else statements
- If
	checks if a condiition is true
- elif
	else if checks another condition, and gives a new output
- else
	backup if the function is false

*Type Error: occurs when two different types are added*

**Iterative Statements:**
- **For Loops**: repeat code for specified sequence
- **While Loops**: they loop *while* a statement is true

	There is two parts of a loop
	- **Header**
		- loop variable: Controls the iteration of a loop (`for i in length)
		- Range(): `range(start, stop, increment)` or `range(length)
	- **Body**
		- break: stops the loop
		- continue: starts the loop again, ignoring the rest

# Module 2

**Functions**: A section of code that can be reused.
`def` is placed behind a function name
`def doFunction():
     `print("Function Complete!)`
 *but nothing happens, you still have to call it*

**Parameters**: a object that included as a object which is used in a function
`range(start, stop)`
*the start and stop are the parameters*

**Argument**: the data brought into a function when it's called
`range(1,7)
*the 1 and 7 are arguments*

**Return**: executes inside a function and sends information back to its call
`return variable`

**Library**: is a collection of modules
**Modules**: run-able code, functions and other things
*Python Standard Library: common module pre-loaded with python*
**Python Enhancements Proposals** (PEP 8 Guidelines): guidelines on how code should be written to keep readability 

# Module 3

Strings are immutable, once they are set they can't be changed

List Methods:
- `.insert(where, variable)` finds the index and places a variable
- `.remove(variable)` removes instance
- `.append(variable)` adds instance to the end of a list
- `.index(variable)` outputs the index of variable

- "`\w`" is any alphanumerical value
Import re or regular expressions are used to search for patterns
`re.findall("ts", "tss", "aaaa", "tsa)`

# Module 4

**Parsing**: converting data into a readable format

Working With Files:
- **open**: command to open and read ("r") or write ("w") to a file in python
`with open("file", "r") as file:
	`var = file.read()`

- `.read()` converts files into strings
- `.split(p)` turns string into a list, p tells where to be split
- `"p".join(list)` turns a list into a string, p tells what to join with

Types of Errors:
- **Syntax Errors**: Invalid usage
- **Logic Errors**: Produce unintended results
- **Exceptions**: Mathematically impossible / can't grab proper information

---
# `Course 8: Put It to Work: Prepare for Cybersecurity Jobs`


# Module 1

**Security Mindset**: the ability to assess risk and identify breaches

Data Types:
- **Public Data**: Accessible to the public, but still needs to be protected
- **Private Data**: Kept away from the public
- **Sensitive Data**: Only people authorized can view
- **Confidential Data**: PII

# Module 2

**Incident Escalation**: identify a incident, triaging it, then handing it to the proper team

Skill to Escalate Security Incidents:
- Attention to Detail
- Following Escalation Guidelines

Reasons to Escalate:
- **Malware**
- **Unauthorized Access**
- **Improper Usage**

Types of Data Privilege: 
- **Data Owners**: Admin
- **Data Controller**: Determines how data is used, stored and processed
- **Data Processors**: Third party processor for the controller
- **Data Custodian**: Grant and Revoke access to data
- **Data Protection Officer (DPOs)**: Monitor internal compliance, assess security measures.

**Escalation Policy**: a set of guidelines and actions on who should be notified and how the incident should be handled.

# Module 3 

**Stakeholders**: a individual or group who has interest in the actions and activities of a organization
- **Risk manager**: identify risks, manage security incidents, notify legal, and inform public relations
- **Chief Executive Officer (CEO)**: Financial decisions, report to shareholders, and manage operations
- **Chief Financial Officer (CFO)**: Financial operations, and costs tools
- **Chief Information Security Officer (CISO)**: develop security architecture, risk analysis and system audits, and create business continuity plans (BCP)
- **Operation Managers**: oversee pro's, work with analysts, and daily maintenance of security operations

Communicate Concisly: be aware of who and what you tell people about
- Be precise
- Avoid unnecessary technical terms
- Clear Purpose 

Security Story Details: 
- What the challenge is 
- How it impacts
- Possible Solutions

# Module 4 

Tools:
- **OWASP top 10**
- **CSO Online**: News and analysis
- **Krebs Security**: Security Blog
- **Dark Reading**: News

Use social media, join associations.
# Module 5

Jobs:
- **Security Analysis**: monitor data, develop strategies, and research IT trends
- **Information Security Analyst**: creating plans, and implementing security measures 
- **Security Operations Center Analyst (SOC)**: handling incidents rapidly and efficiently, by following playbooks

Jobsites:
- ZipRecruiter
- Indeed
- Monster Jobs
- LinkedIn

Prepare For a Interview:
- Review the Job description
	- Mission
	- Vision
	- Core values
	- Company Culture
- Mock Interview
- Dress like a Pro
- Remind yourself of all the preparation you've done

How to Build Rapport:
- Be formal and professional 
- Be polite / Friendly
- Show appreciation
- Keep tone friendly (if you smile while you talk you will sound friendlier)
- Eye Contact
- Follow up
- Confidence

Have Questions
- **If you were to hire me right now, how would you use my skillset**
- What will be my biggest challenge / and how will i be expected to handle it
- Best part about the company
- What's the typical day like
- What is the growth like

Interview (2 part)
- **Background interview**: education, experience, skills, ability : you should ask questions too, and how they will use your skills
- **Technical interview**: to explain a skill on your resume or answer a question

Final Offer:
- Negotiate for a higher salary
- Ask for other benefits (vacation days)

STAR Method (helps open ended questions)
- **Situation**: create / remember a scenario
- **Task**: the problem
- **Action**: how i handled the problem
- **Results**: how the action went and benefits

Elevator Pitch (short summary):
- short
- persuasive
- who you are
- why you care
- qualifications / skills
- find examples online
Avoid
- rambling
- don't sound ingenuine / conversation
- don't speak to fast