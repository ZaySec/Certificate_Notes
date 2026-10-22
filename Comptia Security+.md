
---
# 1: Security Controls

*Used to prevent, minimize and limit damage*

- **Technical Controls**: (Computer Tech)
	- Encryption
	- Intrusion Detection System (IDS)
	- Firewalls & Antivirus (AV)
	- Least Privilege 
-  **Managerial Controls**: (Written Policies)
	- Risk Assessment 
	- Vulnerability assessment
- **Operational Controls:** (People)
	- Awareness / Training
	- Configuration Management
	- Media Protection
- **Physical Controls**: (Physical)
	- Fences / Locks
	- Badge Readers


**Control Types:**
- **Preventive:** Limits access to a resource 
	- *e.g. Firewall, On-boarding, Guard, Lock*
- **Deterrent:** Discourage a intrusion attempt 
	- *e.g. Splash Screen, Demotion, Reception Desk, Warning Signs*
- **Detective:** Identify and log intrusion attempt
	- *e.g. System Logs, Review Login Reports, Patrol an area, Motion Detector*
- **Corrective:** Used to reverse a event or to continue operating
	- *e.g. Restoring Backups, Create Policies, Contact Police, Fire Extinguisher*
- **Compensating:** Using other means to control a unknown attack type until it is known
	- *e.g. Firewall Rule, Separation of Duties, Require Simultaneous Guards, Generator*
- **Directive:** Direct a subject towards security compliance
	- *e.g. Encryption for Sensitive Files, Compliance policy, Security Policy Training, Sign for Personnel*


--- 


# 2: The CIA Triad

*Confidentiality, Integrity, and Availability (CIA)* 

- **Confidentiality:** Prevent unauthorized access
	- Encryption
	- Access Controls
	- Multi Factor Authentication (MFA)
- **Integrity:** Info cant be modified without logs
	- Hashing
	- Digital Signatures
	- Certificates
	- Non-repudiation
- **Availability:** System and info is accessible
	- Redundancy
	- Fault Tolerance
	- Patching


**Proof of Origin**
1. Prove the message wasn't change (Integrity)
2. Prove the source of the message (Authenticate)
3. Make sure the signature isn't fake (non-repudiation)
4. Sign with the private key
5. Verify with the public key


---


# 3: AAA Framework

*Identify... 
Authentication: You are you.
Authorization: What access do you have?
Accounting: Logging of events...*

(Authenticate) *with Certificate Authority (CA) *
- Digitally sign certificates with the CA
- You can use the signature to verify
(Authorize) *with Authorization Model (Abstraction)*
- Make a role / group which a user will need depending on what they need to access


---


# 4: Gap Analysis

*Where you are, and where you want to be*

1. **Choosing the Framework**
	- Baseline like these can be pre-created by organizations
		- NIST
		- ISO/IEC 27001
2. **Evaluate People & Processes**
	- Experience 
	- Current training
	- Know their knowledge of policies and procedures
	- Research existing IT systems / Policies 
3. **Compare and Contrast** 
	- Evaluate existing systems weaknesses
		- Next find the best process
	- Examine broad categories 
		- Break them down and apply or fix
4. **Analysis Report**
	- Detailed baseline objectives
	- Clear view of the current state
	- Create a path
		- Time
		- Money
		- Change Control
	- Create a final report and formal description


---


# 5: Zero Trust

*Authenticate yourself each time you want access to a resource*

**Planes of operation:**
- **Data Plane:** Sending the data and security actions
- **Control Plane:** Manages actions and policies of the data plane


**Controlling Trust:**
- **Adaptive identity**
	- consider the source
	- relationship to the organization
	- physical location
	- type of connection
	- ip address
- **Threat Scope Reduction**
	- decrease the number of possible entry points
- **Policy-driven Access Control**
	- combine the adaptive identity with pre-defined rules to decide access level
- **Security Zones**
	- Where we connect *from*
	- Where we connect *to*
	- you can create vpns for specific groups (untrusted / trusted)
- **Policy Enforcement Point (PEP)** 
	- Collects info
		- End users
		- applications
		- non-human entities
	- **Policy Decision Point**
		*Decides if connection are allowed or disallowed*
		- **Policy Engine**
			- Checks all the decisions and compares them to rules
			- Grant, deny or Revoke
		- **Policy Administrator** 
			- Take the decision and give it the the policy enforcement point (PEP)


---


# 6: Physical Security

*You need to know how to protect a physical space*

- **Barricade**
	- Prevent Access
	- Channel people through a point
	- Identify safety concerns
	- Can be used to a extreme
		- concrete
		- moats
		- barbed wire
- **Access Control Vestibule (air gap)**
	- A room to pass through to get more access
	- Control access through a area
		- *e.g. if one door unlocks the other locks*
- **Fence**
	- Build a perimeter
	- Transparent or Opaque
	- Robust / Sturdy
	- Prevent Climbing (height or razors)
- **Video Surveillance**
	- Close Circuit Television (CCTV)
	- Object or Motion Detection
	- Network of cameras send video to a storage point
- **Security Guard**
	- Physical protection and reception
	- Validate info
	- Two person integrity
	- Access bade
		- Picture
		- Name
		- Must be worn at all times
		- Electronically logged
- **Lighting**
	- Attackers avoid the light
	- Easier to see when lit
	- Non IR cameras can see better
	- Consider light level and angles
	- Avoid Shadows and Glare
- **Sensors**
	- Motion Detector
		- Infrared (limited in distance)
		- Pressure (weight)
		- Microwave (long distance)
		- Ultrasonic (detect motion and collision detection)


---

# 7: Deception and Disruption

*Discombobulate the bad guys*

- **Honey Pot**
	- Trap the attacker
	- Check what systems they are attacking
	- Create a fake world to waste attackers time
- **Honeynets**
	- Build multiple honey pots
	- Keep attackers very busy
- Honeyfiles
	- Bait the attacker (*e.g. passwords.txt*)
	- add many honeyfiles to file shares
	- Set a alert or bear trap around these files
- Honeytokens
	- Add traceable data to the honeynet
	- Add fake API credentials
	- Add fake emails and monitor them


---


# 8: Change Management

*One change could effect everything*

Clear Change Policies
- Frequency
- Duration
- Installation process
- Rollback procedures


**Change Process**
1. Fill out a change form
2. Have a reason
3. Identify the scope
4. Schedule for the date/time
5. What and who it will effect
6. Analyze the risk associated
7. Get approval
8. Get end-user acceptance


**Ownership**
- Don't make the change
- Owner manages the process
- Ensures the process is followed and acceptable
**Stakeholders**
- They will want to have input
- Be aware of who changes can effect
	- e.g. Changing shipping labels
		- Shipping / Receiving
		- Account reports
		- Product delivery time
		- Revenue
**Impact Analysis**
- Determine the risk (high, medium, low)
- A fix can actually break something
- Data corruption
- What can happen if there is NO change?


- **Test Results:** Use a sandbox or a safe space
- **Backup plan:** Make sure you can revert your changes
- **Maintenance Window:** Find the best time to make the change
	- Holidays
	- Weekends
	- Non work days
	- Time of year


---


# 9: Technical Change Management

*How to perform a change*

- **Scope of Change:** 
	- Only change what is in scope
	- Some liberties are allowed if the are under the scope (*e.g. dependencies*)
- **Downtime:** 
	- Services can be unavailable
	- Have two systems so you can switch to a different
	- Make sure the backups are effective
	- Everyone should be aware of the downtime
- **Restarts:** 
	- Rebooting the OS
	- Physically power off then on
	- Can the system recover from a power outage
	- Services are normally quicker 
	- Launch a new instance
- **Legacy Applications:** 
	 - More complex since they aren't supported
	 - Document the system
	 - Become the expert
- **Dependencies:**
	- Make a change to one service to be able to change another
	- Makes the change process more complex
	- Sometimes it may be on another system
- **Documentation:**
	- The only constant is change
	- Documents can be outdated quickly
	- REQUIRE document updates with the change
- **Version Control:** 
	- Be able to choose a version
	- Easy revert to older systems
	- Know what changes have been made


--- 


# 10: Public Key Infrastructure (PKI)

*Dealing with digital certificates*

- **Symmetric Encryption:** 
	- Encrypt and de-crypt with the same key
	- Shared secret
	- Scalability problem
	- Very Fast!!!
- **Asymmetric Encryption:** 
	- Different keys for encryption and decryption
	- Private and public key
		- Public key is the lock
		- Private key is the unlock
- **Key Escrow:** 
	- The keys are in the hands of a third party


---


# 11: Encrypting Data

*Protect data that is stored*

- **Transparent Encryption:** 
	- Encrypt *ALL* data 
	- Symmetric key
	- Decrypt every time you need it
- **Record-level Encryption:**
	- Encrypt *only* what necessary
	- Less overhead
- **Transport Encryption:**
	- Make sure info being sent is protected
	- Encrypt in the application (*e.g. HTTPS*)
	- Virtual Private Network (VPN)
- **Encrypting Algorithms:**
	- Many different types
	- Requires both sides to use the same one(s)
	- Advantages and Disadvantages of different algorithms
		- Security Level
		- Speed
		- Complexity
- **Cryptographic Keys:** 
	- Open knowledge of how they work
	- Knowing doesn't help
	- The key is the only thing that is effective
- **Key Lengths:**
	- Larger keys tend to be more effective
	- A weak key is a weak key
- **Key Stretching:**
	- Hash a hash of a hash...


---


# 12: Key Exchange

*How do you share a key if the transport is insecure*

- Share a *symmetric key* with *asymmetric encryption*


---


# 13: Encryption Technologies


- **Trusted Platform Module (TPM):**
	- Designed to give cryptographic functions
	- Persistent memory
	- Password protected
- **Hardware Security Module (HSM):**
	- For servers and a lot of keys
	- Large scale
	- Securely stores keys
	- Offload CPU's overhead to this device
- **Key Management System:**
	- On base or cloud based
	- Manage all keys from one console
	- Keeps the keys away from the data
	- Rotate keys
	- Logging and reporting of keys
- **Secure Enclave:**
	- A protected part of hardware isolated (processor)
	- Has its own boot ROM
	- Monitors system boot
	- Has a true RNG
	- Root cryptographic keys
	- AES encryption


---


# 14: Obfuscation 

*Hiding information in plain site, only knowing how its hidden will reveal it*

- **Steganography:**
	- Root in Greek "Concealed Writing"
	- Security through obscurity
	- *e.g. hiding information in a image or embed messages in TCP packets*
	- Audio and video can also be used
- Printers use yellow dots to create watermarks
- **Tokenization:**
	- replace sensitive information with a non-sensitive placeholder
	- Temporary tokens are used on credit card processing
	- We wont have to encrypt data now!
- **Data Masking:**
	- Hide the original data 
	- Protects PII
	- The data may still be intact in storage
	- Techniques
		- *substituting, shuffling, encrypting, masking out...*


---

# 15: Hashing and Digital Signatures

*Represent data as a short string of text*

- **Hashing:**
	- SHA256
- **Collision:**
	- Hashes should be unique 
	- MD5 had a collision making it bad...
- **Practical Hashing:**
	- Comparing downloads 
	- Store passwords
	- Don't store passwords in plain text, provide a hash
- **Salting:** 
	- Extra random info added to the has to randomize the hash
	- Everyone can use the same password and they will still have different hashes
	- Stops rainbow tables
- **Digital Signature:** 
	- *sign with the private key, verify with the public*
	- Non-repudiation
	- Integrity
	- Authentication


How to create a Digital Signature
1. Plain text 
2. Hash it
3. Encrypt hash with private key
4. Done!
Verify
1. Decrypts the signature with public key
2. Hash the plain text to verify


---


# 16: Blockchain Technology

*everyone can maintain the ledger, and everyone has a copy*

- **Open & Practical for**
	- Payment Processing
	- Digital Identification
	- Supply Chain Monitoring
	- Digital Voting


---

# 17: Certificates

*More than just a identification card...*

- **X.509 (Standard format):**
	- Serial number
	- Version
	- Signature algorithm
	- Issuer
	- Name of the cert holder
	- Public Key
	- Extensions
- **Root of Trust:**
	- How can we trust someone we don't know yet?
	- Third party voucher
	- Hardware Security Module (HSM)
	- Security Enclave
- **Certificate Authorities (CA):**
	- Trusted third party
	- An authority
	- *If you trust a CA you trust its signatures*
	- Real time verification
- **Third Party Certificate Authorities (CA):**
	- Built into your browser (hundreds of authorities)
	- Responsible for signing digital certificates
	- You are not purchasing just the signature but the authority / trust
- **Private Certificate Authority:**
	- Every machine has to trust the internal network CA
	- *e.g. Microsoft Certificate Services, OpenCA...*
- **Key Revocation:**
	- If you need to revoke a digital signature
	- Create a Certificate Revocation List (CRL)
	- Heartbleed effected private keys causing companies to need to revoke signatures / certificates
- **Online Certificate Status Protocol (OCSP):**
	- Certificate holders verify their status
	- The status is connected to the handshake
	- Some may say they support but don't check



---


# 18: Threat Actors

*Entity responsible for a attack*

- **Attributes:**
	- Internal / External
	- Resources / Funding
	- Level of sophistication
- **Motivations:**
	- Data
	- Espionage
	- Disrupt the Service
	- Blackmail
	- Financial Gain
	- Political
	- Ethical 

Types of Threats
- **Nation State (APT):**
	- External Entity
	- Government
	- data, revenge, disruption, war...
	- Constant attacks, lots of funding, and even multiple attacks at once
	- Also known as a Advanced Persistent Threat (APT)
	- Highest Sophistication
- **Unskilled Attacker (script kiddie):**
	- External or internal
	- Anyone can do this
	- Disruption, data, philosophical, money...
	- Not a lot of resources
- **Hacktivist:**
	- External
	- Hacker with a activism purpose
	- Philosophy, revenge, disruption
	- Low resources
- **Insider Threat:**
	- Internal
	- Revenge or financial gain
	- Medium level of sophistication since they know the land
- **Organized Crime:**
	- External
	- Sophisticated and funded
	- Could be a group or a individual
	- Motivated by Money
- **Shadow IT:**
	- Internal 
	- Going rouge by building their own infrastructure
	- Don't have to deal with company stuff, instead make their own
	- Limited by budget

| Threat Actor    | Location | Resources       | Sophistication | Motivation                      |
| --------------- | -------- | --------------- | -------------- | ------------------------------- |
| Nation State    | External | Extensive       | Very High      | Data, Revenge, Disruption War   |
| Unskilled       | External | Limited         | Very Low       | Data, Disruption, Philosophy    |
| Hacktivist      | External | Some Funding    | Can be High    | Revenge, Disruption, Philosophy |
| Insider Threat  | Internal | Many Resources  | Medium         | Revenge, Financial Gain         |
| Organized Crime | External | Often Extensive | Very High      | Financial                       |
| Shadow IT       | Internal | Many Resources  | Limited        | Revenge, Philosophy             |


---


# 19: Common Threat Vectors

*Methods of attack*

- **Message Based Vector:**
	- One of the biggest and most successful
		- Email
		- SMS
	- Phishing attacks use malicious links
	- Social engineering techniques
		- invoice scan
		- cryptocurrency scam
- **Image Based Vector:**
	- Scalable Vector Graphic (SVG)
		- XML file that holds more than a image
		- Could put a java injection
- **File Based Vector:**
	- Malicious Code can hide in many places
	- Compression type
		- contains malicious info inside
	- Microsoft Office, Adobe, Zip, RAR
- Voice Call Vectors: 
	- Vishing is phishing over the phone
	- Spam over IP to large scale IP
	- War Dialing is trying to find unpublished phone numbers that can give access
	- Call Tampering is disrupting voice calls
- **Removable Device Vectors:**
	- Useful for air gapped networks
	- USB drive that can act as something else
- **Vulnerable Software Vectors:**
	- Client Based
		- Infected executable
		- May require updates
	- Agent less
		- Separate system
		- Compromised server would affect all users
- **Unsupported Systems Vectors:**
	- Not having the ability to patch a vulnerability
	- Make sure all of these systems are identified
- **Unsecured Network Vectors:**
	- Ease of access for attackers
	- make sure to use proper protocols (*e.g. WPA2*)
	- No open access points
	- Enable 802.1X
	- Bluetooth could also be used for recon
- **Open Service Ports:**
	- Every open port is a opportunity
	- Every application has their own open port
	- Firewalls help control traffic through these ports
- *Make sure to change default credentials *
- **Supply Chain Vector:**
	- tampered during or after the manufacturing process
	- Managed Service Providers (MSPs) are targets for hackers, and they can manage PII


---

# 20: Phishing

*Trying to get your to click the link*

- **Business Email Compromise:**
	- Don't trust emails
	- Spoofed email addresses to look legit
- **Tricks and Misdirection:**
	- Typosquatting (*e.g. go0gle.com*)
	- Pretexting (a well made lie / story)


---

# 21: Impersonation

*Pretending to be someone they are not to gain trust*

- **Eliciting Information:**
	- Gaining info they would not have access too
	- Not as simple asking for bank account number
- **Identity Fraud:**
	- A attacker using someone else's information to gain 
	- credit, bank, loan fraud and more
	- Can be used with government employees
- Protection
	- Never volunteer info
	- Never give personal info across the internet
	- Always verify who they are



---


# 22: Watering Hole Attack

*Instead of accessing your network, they wait for you to visit a site they hacked*

- **Executing a Watering Hole Attack:**
	- Determine the sites the victim uses
	- Infect one of the third party sites
	- Infect all the visitors 
- **Defense in Depth:**
	- Layered Defense (*e.g. Firewall and IPS*)
	- AV or Anti-malware signature updates



---


# 23: Other Social Engineering Attacks

*Injecting false info*

- **Misinformation / Disinformation:**
	- Spread incorrect information
	- Create confusion and division
	- Divide, Distract, persuade
	- Advertising can take a part
	- Enabled through social media
- **The Misinformation Process**
	1. Create fake users (sock puppets)
	2. Create Content
	3. Post on Social Media 
	4. Amplify Message
	5. Real Users share the info
	6. Mass media will pick up the story
- **Brand Impersonation:**
	- Pretend to be a known / trusted brand
	- Create tens of thousands impersonated sites
	- Visitors can be given malware and pop ups


---


# 24: Memory Injections

*Malware running in memory*

- **Memory Injection:** 
	- Hide malware inside of a process 
	- Get access to that data and privileges
- **DLL Injection:**
	- Many applications use this DLL 


---


# 25: Buffer Overflows

*Spilling over into other memory areas*

- Honestly too technical
- Adding extra memories to packets


---


# 26: Race Conditions

*Things happening at the same time*

- **Time of Check to Time of Use Attack (TOCTOU)**
	- If you are planning on using a variable you will check it
	- Now if the variable changed by the time it is used, this is a race condition
- **Race Condition Example:**
	- *If not all users of a bank are updated with a ledger, more withdrawls than allowed may be made*


---


# 27: Malicious Updates

*Not every update is more secure than the last*

- **Updates can appear when you open a application**
	- Certain malware may appear to be a update
- **Downloading and Updating**
	- Every installation may be malicious 
	- Confirm the source
	- Visit the developers site directly
	- Many OS's will only allow signed apps
- **Automatic Updates**
	- Often includes security checks / digital signatures
	- Relatively trustworthy


---


# 28: # Operating System Vulnerabilities

*Everyone has a OS*

- **Windows receive a OS update every second tuesday of the month**
	- *Elevation of Privilege Vulnerabilities, Security Feature Bypass Vulnerabilities, Remote Code Execution Vulnerabilities, Denial of Service Vulnerabilities, Updating Vulnerabilities*
- **OS Best Practices**
	- Always update ASAP
	- May require testing before deployment
	- May require a reboot
	- Have a fallback plan


--- 


# 29: SQL Injection 

*Running code that shouldn't be ran*

- Any input from the user is vulnerable


---


# 30: Cross Site Scripting (XSS)

*Having someone else run the malicious code, to retrieve info*

- **Normal Attack**
	- Sending a malicious link that also have the exe (most commonly java) 
	- The victim opens the link and runs the java
	- The attacked can hijack thier account
- A persistent attacks works the same, but instead they post the link somewhere that works persistently 
- **Protecting from XSS attack**
	- Don't click third party links
	- Disable or limit javascript
	- Keep your browser and applications up to date


---


# 31: Hardware Vulnerabilites

*The S in IOT stands for security*

- Anything connected to a network can be attacked
- **Firmware is the OS on the device**
	- Many times people don't know what it is
	- Only the vendors can fix it
- **End of Life (EOL)**
	- manufacturer stopped selling the product
	- may continue support
	- important for security patches and updates
- **End of Service Life (EOSL)**
	- Support is no longer available 
	- No ongoing patches or updates
	- May have premium-cost support option
	- SIGNIFICANT CONCERN
- **Legacy Platform**
	- Older hardware, software, firmware
	- Compare risks to reward if its a EOSL
	- May require extra firewall rules 


---


# 32: Virtualization Vulnerabilities

*escaping a vm, is hard but worth it*

- Many similar vulnerabilities and opportunities
- VM escape would mean full control over the vm


--- 


# 33: Cloud-specific Vulnerabilities

*With embracing the cloud, we take in their vulnerabilities*

- **Attack the service**
	- Denial of Service (DOS)
	- Take advantage of weak or faulty authentication
	- Directory Traversal
	- Remote Code Execution (run anything they like on your server)
	- Web application attacks have increased
	- Cross site scripting (XSS)
	- Out of bounds write (crash or run remote exe)
	- SQL Injection


---


# 34: Supply Chain Vulnerabilities

*Every step along the way can be attacked*

- One exploit added somewhere on the attack chain can be abused down the road
- **Service Providers**
	- Can't control a service provider
	- They have access to internal services (useful for a hacker)
	- Many different types of service providers
	- Add security audits into the contract
- **Hardware Providers**
	- Can you trust the system? (How can you verify)
	- Have a list of trusted vendors
	- Strict Controls over policies and procedures
	- Principle of least permission
	- There's a limit to trust
- **Software Providers**
	- Look at the digital signature at the installation
	- Software auto updates requires a lot of trust
	- Open Source?
		- Pros: being able to see the code
		- Cons: Malicious changes


---

# 35: Misconfiguration Vulnerabilities

*They will find your mistakes*

- Its easy to leave a door unlocked
- **Unsecured Admin Accounts**
	- Make sure to have a strong password
	- Disable the ability to direct login to the root account
		- *You have to login through a normal account, and then sudo that account*
	- Protect these important accounts
- **Insecure Protocols**
	- Some protocols aren't encrypted (*Telnet, FTP, SMTP, IMAP*)
	- Verify with a packet capture
	- Change to the encrypted version (HTTP -> HTTPS)
- **Default Settings**
	- Every application has default logins
	- Mirai Botnet
		- Takes over IOT devices automatically
		- Open source and available to run
- **Open Ports and Services**
	- Services can open ports 
	- Manage with a firewall
	- Firewall rule sets can be complex, and it's easy to mess up
	- Always test and audit


---


# 36: Mobile Device Security

*Difficult to secure and more*

- **Jailbreaking / Rooting**
	- Install custom firmware
	- Used to gain more access to the device
	- Uncontrolled access
- Side loading
	- Malicious apps
	- Manage installation sources 


---


# 37: Zero-Day Vulnerabilities

*There is vulnerabilities, we just don't know them yet. Zero is in reference to the first day they are found*

- Search for unknown vulnerabilities, so they cant fix / notice it
- If a zero day vulnerability is used against a machine then it is a zero day attack
- Since vendors don't know yet, there isn't a patch


---


# 38: Malware

*Malicious software*

- **Types:**
	- Viruses
	- Worms
	- Ransomware
		- Encrypts all of your data, they want you to pay to decrypt
		- Always has backups
	- Trojan Horse
	- Rootkit
	- Keylogger
	- Spyware
	- Bloatware
	- Logic Bomb
- Multiple types of malware can work together 
- **Data is valuable**
	- Family pictures
	- Important documents
	- Personal Identifiable Information (PII)
	- Company Private Data


---


# 39: Viruses and Worms

*Malicious software*

- **Virus**
	- Can reproduce itself
	- Can be invisible 
	- Thousands of new Viruses each week
	- **Types:**
		- Program Virus: part of a application
		- Boot Sector Virus: at boot the virus runs
		- Script Virus: runs a script
		- Macro Virus: there can be a virus in a application
		- **Fileless Virus:**
			- Stealthy, it can avoid AV
			- Operates in memory
- **Worms**
	- Automatically reproduce and spread across a network
	- Can over many systems quickly
	- Firewall and IDS and IPS 


---


# 40: Spyware and Bloatware

*Watching and making you slow*

- **Spyware**
	- Maintain AV
	- Always know what you are installing 
	- Where's your backup...
	- Run some scans
- **Bloatware**
	- Applications you didn't expect
	- You don't get a choice
	- Waste of storage
	- Slows down the system
	- More Vulnerabilities
	- Challenge to uninstall


---


# 41: Other Malware Types

*More types of malware*

- **Keyloggers**
	- Capture typing data (*e.g. websites. credit cards, password, messages*)
	- Circumvents E2E
- **Logic Bomb**
	- Waits for predefined event
	- Time Bomb
	- User Event
	- Difficult to Identify
	- Prevention
		- No predefined Signatures...
		- Change Control
		- Monitor when files have been changed
		- Constant Auditing
- **Rootkit**
	- Modifies core system files
	- Can be invisible to the OS and AV
	- Use a rootkit removal tool (reactive not preventive)
	- Secure boot with UEFI


---


# 42: Physical Attacks

*Locks only keep out honest people*

- **Brute force (the physical version)**
	- push through obstacles
	- Break windows / doors
	- pick locks
- **RFID Cloning**
	- Stealing a access badge and key fobs
	- Duplicators are cheap
	- Can take a matter of seconds
	- Use MFA to prevent
- **Environmental Attacks**
	- Attack everything supporting the technology
	- Power monitoring (destroy their power)
	- HVAC (systems need to be properly secured)
	- Fire suppression


--- 


# 43: Denial of Service (DoS)

*Stop the services from running*

- **Friendly DS**
	- Unintentionally DoSing yourself
	- Looping a switch
	- Bandwidth DoS
	- Any environmental mistake (*e.g. fire, water, temperature, humidity*)
- **Distributed Denial of Service (DDoS)**
	- Botnets set to attack (or send a lot of data too)
	- Can be above 3 million devices
	- Asymmetric Threat (the attacker can have a small amount of resources, but are still effective against a org with a lot of resources)
- **DDoS Reflection and Amplification**
	- Turn your small attack into a big attack
	- Protocol Abuse (*e.g. NTP, DNS, ICMP*) requesting information


---


# 44: DNS Attacks 

*Tricking where a computer requests info from*

- **DNS Poisoning Attack**
	- Modifying the DNS server
	- Modify the host files 
	- MiTM attack to DNS spoof
- **Domain Hijacking**
	- Instead of spoofing the DNS packet, just take the domain name
	- Hackers are now the IP address, being able to steal any info sent
- **URL Hijacking** (*typosquatting / brandjacking*)
	- *e.g. g0ogle.com*
	- Sell a bad url to the LEGITIMATE site
	- Phishing Site
	- Infect your device
	- Different top level domain (google.com vs. google.net)


---


# 45: Wireless Attacks

*Attacking or jamming frequencies*

- Deauth attack
- **Protecting against deauth attack**
	- Some of the important management frames are encrypted
- **Radio Frequency (RF) Jamming**
	- DoS to prevent wireless access
	- Non-intentional (*e.g. microwave, Fluorescent light bulbs*)
- Wireless Jamming
	- Constant random bits 
	- Data sent at random times to be harder to diagnose
	- Reactive jamming (only when someone tries to communicate)
	- Fox hunter (find who is jamming)
		- Directional Antenna 
		- Attenuator 


---


# 46: On-path Attack (or MiTM)

*Someone in the network is watching*

- MiTM sits between two devices collecting all the information
- ARP Poisoning 
	- requires the attacker to be on the subnet
	- the attacker will redirect the traffic
- On-path browser attack ()
	- acts as a proxy 
	- redirects traffic


---


# 47: Replay Attacks

*Capturing sent info to appear as the client*

- **Pass the hash**
	- Client sends info to server
	- Attacker intercepts the hash
	- The password is in the hash, but they don't need to encrypt (unless they encrypt it)
- **Cookies**
	- Stores valuable info (*e.g. user, session ID, details about session*)
- **Session Hijacking**
	- With a session ID, you wont need to authenticate
	- Session ID can be intercepted
- **Header Manipulation**
	- Info Gathering (wireshark, kismet)
	- Expliot (XSS)
	- Modify Headers (tamper, firesheep, scapy)
	- Modify Cookies (Add ons)
- **Prevention**
	- ENCRYPT EVERYTHING


---


# 48: Malicious Code

*Any executable code*

- **Forms**
	- exe, scripts, macro viruses, worms, trojans horses, etc... 
- **Protection**
	- Anti-malware
	- Firewall
	- Continous updates and patches
	- Secure Computing habits


---


# 49: Application Attack

*Just more attacks*

- **Injection attack**
	- Adding your own info to data
	- Code should always check inputs
	- SQL Injection
- **Buffer Overflow**
	- Adding extra data into a memory slot, overflowing into a new memory slot
	- Not simple / very powerful
- **Replay attack**
	- Using sent info from client, to appear as the client
	- Might first use a MiTM
- **Privilege Escalation** 
	- Gain higher level access to a system
	- Principle of Least Privilege 
	- Mitigation
		- Patch the application
		- Update AV
		- Data Execution Prevention
- **Cross Site Requests**
	- It looks like its receiving info from one server, but it can be the wrong one
	- Intercepting can be prone to forgery, changing your request and making the server do something else
- **Directory Traversal**
	- Read or write files that are outside the scope of a servers directory
	- Request info from other directory paths can show vulnerabilities


---


# 50: Cryptographic Attacks

*Instead of finding the key, they attack the safe*

- **Birthday Attack**
	- what are the chances two students share a birthday? 50%
	- Hash Collision: two different plain texts that have the same hash
- **Collisions**
	- Two hashes are similar enough they produce the same hash
- **Downgrade Attack**
	- Force a system to use a weaker encryption / no encryption
	- SSL Stripping, 
		- Works as a MiTM, 
		- Strips the S from HTTPS
		- The page is now in the clear


---


# 51: Password Attacks

*guessing passwords*

- Don't store passwords in plain text
- Hash all passwords
	- hash represents data as a fixed-length string
	- No way to reverse engineer from just the hash
- **Spraying Attack**
	- Incorrect password guessing can get a lock out
	- Attackers use top passwords
- **Brute Force Attack**
	- Tries every possible combo of letters to guess a password
	- It is very slow
- 


---


# 52: Indicators of Compromise (IOC)

*finding out if you have a compromised system*

- **Indicators**
	- Unusual amount of traffic
	- Hash values have changed
	- Uptick in traffic from somewhere new
	- Change to DNS data
	- Uncommon login patterns
	- Certain files are being read more often
- **Account Lockout**
	- Credentials are not working
	- OR a admin could have locked out a account, which in itself is a indicator (but worse)
- **Concurrent Session Usage**
	- One account is logged in from different places
	- Difficult to tell, maybe a phone and a pc
- **Blocked Content**
	- Attacker wants to stay in, so they stop updates and patches
	- Removal Tools or AV might not be able to run / be downloaded
- **Impossible Travel**
	- Authentication logs can be telling
	- You can't have a user logon in two different continents minutes apart
- **Resource Consumption**
	- Watch for file transfers (Bandwidth might increase at strange times *3am*)
	- Could be your first notification that there is a current breach
- **Resource Inaccessibility**
	- Server is down
	- Network Disruption
	- Encrypted data (ransomware)
	- Locked (Brute force attack)
- **Out-of-cycle Logging**
	- Info in log should not be happening 
	- Firewall log activity
- **Missing Logs**
	- A attacker deletes logs / evidence
	- Setup notification if logs go missing
- **Published / Documented**
	- If your data has been published online
	- Raw data may be released without context


---


# 53: Segmentation and Access Control

*Isolating devices can keep them from getting infected*

- Segmenting
	- Isolating devices can keep them from getting infected
	- Can increase performance (*e.g. bandwidth*)
	- Security
	- Payment Card Industry (PCI) compliance
- Access Control List (ACL)
	- Allow or disallow traffic
	- Restrict access to IP, port, time of day, application, etc
- Application Allow / Deny List
	- Any application can be dangerous 
	- Allow List
		- Nothing runs unless its approved 
	- Deny List
		- Nothing on the "deny" list can run


---


# 54: Mitigation Techniques 

**

- **Patching:** system stability and security
	- Can be automated or monthly
	- Auto-update may not always be the best option
	- Certain systems may require testing before usage
- **Encryption:** 
	- Prevent access
	- File or Disk encryption
- **Monitoring:** 
	- Aggregate info from devices
	- Sensors info
	- Collectors
- **Least Privilege:**
	- Rights and permissions should be the bare minimum
	- All user accounts must be limited (*e.g. roles, admin, guest*)
	- Guest can't run admin privilege
- **Configuration Enforcement:**
	- Perform a posture assessment 
	- Extensive check:
		- OS patch version
		- EDR (end point detection and response) version
		- Status of firewall
		- Certificate status
	- System not to standard can be quarantined
- **Decommissioning:**
	- Data in the trash can be found
	- Most storage devices will still have storage, terminate accordingly 
	- Recycle or Destroy the drive


---


# 55: Hardening Techniques 

*Take devices, add things and configure them to be harder*

- **Endpoint Detection and Response (EDR)**
	- Detect a threat
		- Signatures
		- behavioral analysis, machine learning, process monitoring
	- Investigate the threat 
	- Respond to a threat
		- isolate system, quarantine threat, rollback to a previous config, api driven, no input required
- **Host-based Firewall**
	- software based: runs on every endpoint
	- allow / disallow traffic
	- Identify and block unknown processes 
	- Manage Centrally
- **Host-based Intrusion Prevention System (HIPS)**
	- *Basically a IPS on every device*
- Change Default Configs (*e.g. passwords, ports, names*)
- Remove unnecessary software (less software = less vulnerabilities)


---


# 56: Cloud Infrastructure

*off premise servers that run a service*

- A responsibility matrix will show who is responsible for data
- **Hybrid Consideration:**
	- More than one cloud can be in use (this adds complexity)
	- Network protection mismatch
	- Hard to manage security logs
	- Data Leakage
- **Third Party vendors in the cloud**
	- Vendor Risk assessment
	- Incident Response
	- Monitor
- **Infrastructure as Code**
	- defining the infrastructure as code instead of hardware
	- Code can be reusable to rebuild a instance on another cloud provider
- **Server-less Architecture** 
	- Function as a Service (FaaS)
	- May only run for one event
- **Micro services and API**
	- **Monolithic application** 
		- big application that does everything
	- **Micro service** 
		- Application Programming Interfaces (API)
		- API is the glue for the micro services
		- Scalable
		- Resilient 
		- Better security


---


# 57: Network Infrastructure Concept

**

- **Physical Isolation**
	- Keep certain bandwidths physically apart (air gapped)
	- Web servers and database can be kept separate 
	- Can keep customer data apart
- Virtual Local Area Network (VLAN): separate logically instead of physically
- Software Defined Networking (SDN)
	- Infrastructure plane / Data plane
		- Process network frames and packets
		- Forwarding, trunking, encrypting, NAT
	- Control Layer / Control plane
		- Manages the actions of the data plane
		- Routing tables, session tables, NAT tables
		- Dynamic routing protocol updates
	- Application layer / Management plane
		- configure and manage the device
		- SSH, browser, API


---


# 58: Other Infrastructure Concepts

*centralized vs. decentralized, 
virtualization vs. containers
IoT
SCADA
RTOS
HA*

- **On-premises Security**
	- Customize and full control
	- On-site IT team can mange better, but can be expensive
	- Local team maintains up time and availability
	- Security changes can take time and money
- **Centralized vs. Decentralized**
	- Most organizations are physically decentralized
	- Difficult to manage diverse systems
	- A centralized approach can be better
		- Correlated alerts
		- consolidated file analysis
		- global process for everything
- **Virtualization**
	- Run many different systems
	- Each virtual machine requires a OS and resources
- **Container**
	- Contains everything you need expect a OS
	- Use a docker to run all of the containers
	- Each container is isolated
	- Container image is lightweight
- **Internet of Things (IoT)**
	- Sensors, smart devices, wearable tech, facility automation
	- Weak defaults
	- The S in IoT stands for security
- **SCADA / ICS**
	- Supervisory Control and Data Acquisition System
		- large scale, multi-site Industrial Control Systems (ICS)
	- One control room can monitor and control all the systems
	- Requires extensive segmentation (Isolation for security)
- **Real-time Operating System (RTOS)**
	- A deterministic operating system
		- A car's brake pads are the override control
	- Extremely sensitive to security issues
- **Embedded System**
	- Hardware and software designed for a specific function
- High Availability (HA)
	- Redundancy doesn't always mean available
	- Always on, always available
	- HA also means more expensive


---


# 59: Infrastructure Considerations

*Overview of Infrastructure*

- **Availability**
	- System Up-time
	- Balancing act with security
- **Resilience**
	- Eventually something will happen
		- How fast to fix
	- Mean Time to Repair (MTTR)
- **Cost**
	- Costs a lot of money to keep systems running
	- Initial installation and maintenance costs
	- Consider deprecation, capital expense, taxes
- **Responsiveness**
	- Request info time
	- Important for interactive applications
	- Speed is a important metric 
- **Scalability**
	- Usage can change throughout the day 
	- Elasticity: the ability to expand and retract a applications resource
- **Ease of deployment**
	- An application has many moving parts
	- you must consider how hard or easy it is to install and configure each part
- **Risk Transference**
	- Transfer risk to a third party
	- Cyber security Insurance
- **Ease of Recovery**
	- Time is money
	- Malware infection = Reload a image (10 minutes)
- **Patch Availability**
	- Software isn't static
	- First task after installation
- **Inability to Patch**
	- Patching isnt a option (more often than you think)
	- Common targets are embedded systems
	- May need extra security around this hardware or software
- **Power**
	- Foundational / Overlooked
	- Power requirements 
	- Primary provider
	- Backup services (*e.g. Uninterruptible Power Supply (UPS), Generator*)
- **Compute**
	- Applications heavy lifting
	- More options in the cloud
	- Amount depends on complexity


---


# 60: Secure Infrastructures

*Making sure the pieces of infrastructure can all be protected from each other*

- **Device Placement**
	- Firewalls between untrusted and trusted devices
	- Services may require their own software / defense
- **Security Zone**
	- Separate devices by their use or access type
	- One zone might be able to contact the outside, while another cannot access the outside
		- Trusted / Untrusted (*Trusted -> untrusted only*)
		- Internal / External (*External -> internal*)
- **Attack Surface**
	- How many vectors in
	- Everything can be a vulnerability, all they need is one
	- Minimize the attack surface
		- Audit code
		- Block ports
		- monitor traffic
- **Connectivity**
	- Everything attributes to security
	- Secure the cables, protect the physical from taps
	- Application level encryption
	- Network level encryption


---


# 61: Intrusion Prevention System (IPS)

*Watch traffic and decide if it needs to be stopped*

- Intrusion Detection System (IDS): *ONLY* monitors but doesnt stop
- **Failure Modes**
	- We need IPS to have a 100% uptime
	- Fail-open: data will flow with no IPS
	- Fail-close: data will stop
- **Device Connections**
	- Active monitoring: A IPS can be inline, like a firewall
		- A outage can cause downtime
		- The IPS could block legitimate traffic
		- Fail-close
	- Passive Monitoring: Its not inline, receives a copy instead
		- Cannot block traffic in real time
		- Fail-open


---


# 62: Network Appliances

*Network devices*

- **Jump Server**
	- A server that can be accessed from the outside
	- SSH / Tunnel / VPN
	- Significant Concern
- **Proxy Server**
	- Makes requests on behalf of a user
	- Can act as a middle man and IPS / IDS
	- Can be used for caching
	- Explicit Proxy: needs to be configured 
	- Transparent Proxy: will act as a proxy without the person knowing
- **Application Proxy**
	- NAT (network address translation): converts internal to external IP addresses
	- Some proxies can work with multiple protocols, while others can do only one
- **Forward Proxy**
	- Or internal proxy
	- This proxy sends traffic to the external then replies to the internal
	- Is used for security
- **Reverse Proxy**
	- Inbound traffic from the external to the internal
	- Can act as a Cache for the internet
- **Open Proxy**
	- SIGNIFICANT CONCERN FOR SECURITY
	- Is controlled by a third party, who we can not trust
	- Third party could add information as a MiTM
- **Balancing The Load**
	- Distribute the load
	- Large scale implementation
	- Fault tolerance: if a server fails, the other servers will take the load
	- Active / Active load balancing
		- All the servers are in use and being used
		- SSL offload (decrypt and encrypt the info, saving resources for the servers)
		- Prioritization
		- Content Switching
	- Active / Passive load balancing
		- Some server are active
		- Fault tolerant in practice
- **Sensors and Collectors**
	- Aggregate info from network devices
	- Collect logs on almost everything
	- Collector
		- Could be a SIEM
		- A centralized console for the info


---


# 63: Port Security

*Protect the entry points of traffic*

- Passwords and usernames count as a part of this security
- **Extensible Authentication Protocol (EAP)**
	- Many different ways to authenticate
	- integrates with 802.1x
- **IEEE 802.1x**
	- Port based Network Access Control (NAC)
	- Wont be able to use network until authenticated
- **EAP and 802.1x**
	- Supplicant - the client
	- Authenticator - the device that provides access
	- Authentication Server - Validates the client credentials 
	1. Initialize = supplicant talks to authenticator
	2. EAP Request = authenticator asks for supplicant credentials
	3. EAP Response = supplicant gives credentials to authenticator
	4. Pass = authenticator informs the Authentication Server
	5. Question = Authentication Server asks the authenticator for more details
	6. Requests details = authenticator asks supplicant for more details
	7. Answers = supplicant gives credentials 
	8. Confirm = Authentication Server chooses if the credentials are good


---


# 64: Firewall Types

*Control the traffic between points*

- **Universal Security Control**
	- Parental Controls
	- Controls web requests and content
	- Acts as a IDS / AV
- Network Based Firewall
	- Filter traffic by port of application
	- Encrypt traffic
	- Firewalls can be a level 3 device (router)
- UTM
	- Unified Threat Management Device
	- Can handle multiple things at once
	- URL filter / Content inspection
	- Malware inspection
	- Spam filter
	- CSU / DSU
	- Router, switch
	- Firewall
	- IDS / IPS
	- Bandwidth shaper
	- VPN endpoint
	- Can only turn on a few services before losing performance
- Next-Generation Firewalls (NGFW)
	- *e.g. application layer gateway, stateful multi layer inspection, deep packet inspection*
	- Operate at OSI level 7
	- Can analyze all packets of a network...
		- Can determine what applications are used and decide if certain packets are needed
		- Can act as a IPS 
		- Content filtering
- Web Application Firewall (WAF)
	- Analyze input in web based applications
	- Acts as a IPS 
		- e.g. stopping SQL injection
	- Can work with a NGFW
	- It may be required for PCI DSS (Payment Card Industry Data Security Standard)


---


# 65: Secure Communication

*If you need to access a network from the outside*

- **Virtual Private Network (VPN)**
	- Encrypted Tunnel
		- Encrypt your data which will mean you need new headers
		- Once the packet is received decrypt
- **SSL / TLS VPN (Secure Socket Layer VPN)**
	- Uses common SSL / TLS protocol (No firewall issues)
	- Remote access for a single device (client)
	- Use normal login, or have digital certificates for SSL 
	- Can be ran from application or browser
- **Site to Site IPsec VPN**
	- Always on
	- Remote site can connect to corporate network
- **SD - WAN**
	- Software Define Networking in WAN
	- Built for the cloud
- **Secure Access Service Edge (SASE)**
	- "Next Gen" VPN
	- Security technology is next to the cloud


---


# 66: Data Types and Classifications

*Not all data is the same*

- Data Types
	- **Regulated Data** (*e.g. managed by third party, laws and statues*)
	- Trade Secret (*e.g.a organization secret formulas*)
	- **Intellectual Property** (*e.g. Copyright and trademark*)
	- **Legal Info** (*e.g. sensitive aspects of legal matters need to be kept a secret*)
	- **Financial Details** (*e.g. bank details, payment info*)
	- **Proprietary** (*e.g. data only to be found in a org*)
	- **Personally Identifiable Information (PII)** (*e.g. anything to identify a person*)
	- **Protected Health Information (PHI)** (*e.g. health info*)

	- Human - Readable
	- Non-human readable
	- Hybrid
- **Classifying Sensitive Data**
	- Not all data has the same level
	- Different levels require different clearance
	- Or data may require a different process to be able to view
	- Create a private sector network to view data
- **Data Classifications** 
	- Sensitive data
	- Confidential
	- Public / Unclassified
	- Private / Classified / Restricted 
	- Critical (always available)


---


# 67: States of Data

*Data in different states*

- **Data At Rest**
	- If data is on a storage device then data is at rest
	- Encrypt Data
	- Apply permissions
- **Data In Transmit / Motion**
	- Data being moved in a network
	- Not much protection as it travels
	- Protection: Use a Firewall or IPS
	- Transportation Encryption: TLS or IPsec
- **Data in Use**
	- Data actively in use
	- Normally not encrypted
	- Attackers like to target this
- **Data Sovereignty**
	- Data in a country is applied to its laws
	- Legal monitoring, court orders, etc
	- Laws may prohibit where data can be stored
		- *e.g. EU citizen data must be stored in the EU*
	- Learn the compliance laws
	- **Geolocation**
		- Location details
		- 802.11, mobile provider, GPS
		- Use location data to determine what type of access a person has
		- If someone is inside a corporate building then they can get more access


---


# 68: Protecting Data

*Ways to protect data*

- **Geographic Restrictions**
	- Depending on where a person is ; control their access
	- Identify IP subnet, though it can be hard
	- Geolocation data
	- IP address is not very accurate
- **Geofencing**
	- Determining the access to someone depending on where they are
- **Protecting Data**
	- Security jobs primary task
	- Be aware of where data is
	- **Permissions Restrictions**
		- Control access to data
		- Have a authentication process
	- **Encryption**
		- Plain text -> Cipher text
		- Confusion: when encrypted data looks completely different from its plain text
		- Hashing (can approve of data, but a finger print cant recreate a person)
	- Obfuscation: make something harder to read
	- Masking: Hide some data (*e.g. show just on part of PII*)
	- Tokenization: replace sensitive info with a placeholder
	- Segmentation: Separate data into different locations, divide and store


---


# 69: Resiliency

*Be hard to kill*

- **High Availability (HA)**
	- Always on, always available
	- If one machine goes down another can pick up the pace
	- Additional costs (*e.g. more systems, more power*)
- **Server Clustering**
	- Combining servers
	- Easy to increase or decrease capacity
	- Interoperability
- **Load Balancing**
	- Load is distributed amongst the servers
	- Load balancer  
- **Site Resiliency**
	- Moving a data center to another location
	- Could be used for natural disasters 
	- Could go back to original center
- **Hot Site**
	- A exact replica of everything 
	- Another cloned server center
- **Warm Site**
	- Some hardware
	- Some data
- **Cold Site**
	- No hardware
	- Empty building
	- People to run the site
- **Geographic Dispersion**
	- A backup site within the same proximity of a storm is no use
	- Hard to transport equipment / people
- **Platform Diversity**
	- Different platforms can create a challenge for hackers
	- Used so one vulnerability can't take down a whole server
- **Multi-cloud System**
	- Many different cloud services
	- A breach would not effect the entire server
	- Geographic Dispersion
- **Continuity of operations planning**
	- Backup plan
	- Have alternatives to server


---


# 70: Capacity Planning

*Supply the demand (in balance)*

- **People**
	- Some services require human intervention
	- Too few can be bad
	- Too many can be expensive
- **Technology**
	- Pick technology that can expand
	- Web severs = load balancer
	- Database servers = clusters sql
	- Cloud servers = cost depends on size
- **Infrastructure**
	- Underlying framework
	- Physical Devices (purchase, configure, install)
	- Cloud-based Devices (Easily deployed, can expand)


---


# 71: Recovery Testing

*Make sure your recovery plan works*

- **Tabletop Exercises**
	- Performing a full scale recovery can be costly
	- Many logistics and problems can be analyzed
- **Fail Over**
	- Need redudant systems
	- Test to see if redundant configurations work
	- The less you notice the better 
- **Simulation**
	- Try anything (*e.g. phishing attack, password reset, data breaches*)
	- Phishing attack
		- see who clicks and provide more training
- Parallel Processing
	- Improve performance
	- split complex task among processors


---


# 72: Backups

*Storing your storage but more safe*

- **Backup Details**
	- How much data?
	- What type of backup?
	- What media will you store on?
	- Where will said media be stored?
	- What software will be used to backup and restore?
	- How is the schedule?
- **Onsite Backup**
	- No internet link is required
	- Data is immediately available 
	- Generally less expensive
- **Offsite Backup**
	- Transfer over the internet
	- Data is available after a disaster 
	- Restoration can be performed anywhere
- **Frequency of Backups**
	- How often, every day, month, year
	- This can be different on each device
	- This requires significant planning
- **Encryption**
	- Data may need to be protected
	- Recovery key is required
	- Useful for cloud storage (there is no cloud just someone else's server)
- **Snapshots**
	- Useful for cloud environments
	- An instant backup of a entire system
	- Contains only the changes of a system
	- Could be used everyday
	- Fast recovery
- **Recovery Testing**
	- It's not enough to preform a backup
	- Disaster recovery testing (simulation)
	- Confirm restoration, make sure its correct
	- Perform periodic audits
- **Replication**
	- Take one data and clone it to multiple places
	- Data is available somewhere else 
- **Journaling**
	- Corrupted data cannot be read
	- Restore data for a backup
	- Instead do journaling
		- Write to a journal first
		- Then copy it to the dataset
		- Wont get corrupted data


---


# 73: Power Resiliency 

*Power is the foundation of our technology*

- **Uninterruptible Power Supply (UPS)**
	- Short Term backup
	- Blackouts (no power), brownout (drop in voltage), surges (excess voltage)
- **UPS Types:**
	- Offline / standby 
	- Line-interactive (increase volts if needed)
	- On-line / Double conversion 
- **Generator**
	- Long term (with fuel)
	- Power a entire building
	- It may take a few minutes for the generator to kick in
	- Use both


---


# 74: Secure Baselines

*Use the best practices for applications*

- **Establish Baseline**
	- Some organizations already have foundational baselines
	- Often available by manufacturer
		- application developer
		- operating manufacturer
		- Appliance manufacturer
	- *Security Compliance tool kit*
- **Deploy Baseline**
	- Managed through administered controls
	- May require multiple deployment
	- Make it automatic
- **Maintain Baseline**
	- Many practices rarely change
	- Some baselines might require ongoing updates
	- Test and measure conflict


---


# 75: Hardening Targets

*System defaults are rarely secure, use a hardening guide, check online, reach out to manufacturer*

- **Mobile Devices Hardening**
	- Always connected devices need to stay secure
	- Updates are crucial (bug fixes and security patches)
	- Segment the data 
	- Control with a Mobile Device Manger (MDM)
- **Workstations Hardening**
	- User desktops and laptops
	- Constant monitoring and updates
	- Automate the monthly patches
	- Connect to a policy management system
	- Remove unnecessary software
- **Network Infrastructure Devices Hardening**
	- Switch, routers, modems, etc...
	- Purpose built devices
	- Configure the authentication
	- Check with the manufacturer (security updates, not usually updated frequently, but very important)
- **Cloud Infrastructure Hardening**
	- Secure the cloud management
	- Principle of Least Privilege
	- Configure Endpoint Detection and Response (EDR)
	- Always have backups (Cloud to Cloud C2C)
- **Server Hardening**
	- Varied operating systems
	- Updates and service packs (multiple updates)
	- User accounts (proper user and password creation)
	- Network access and security 
	- Monitor and secure (AV, IPS, IDS)
- **SCADA / ICS Hardening**
	- *control, manage, monitor multi scale industrial control systems (ICS)*
	- Distributed system controls 
	- Requires extensive segmentation (no access to the internet)
- **Embedded System Hardening**
	- Hardware and software created for a specific purpose
	- Can be difficult to update
	- Segment and Firewall
- **RTOS (Real Time Operating System) Hardening**
	- Operating system with a deterministic processing schedule 
	- Isolate the system
	- Run with minimum services
	- Use secure communication
- **IoT Devices Hardening**
	- Heating, cooling, lighting, etc.. control
	- Weak defaults
	- Deploy updates quickly
	- Segmentation (access to a IoT device should not be able to escalate)


---


# 76: Securing Wireless and Mobile 

*Not just security, but also signal strength*

- **Site Survey**
	- Determine existing wireless landscape
	- Identify existing access point 
	- Work around existing frequencies
	- Plan for ongoing site surveys
	- Heat maps (show signal strength)
- **Wireless Survey Tools**
	- Signal Coverage
	- Potential Interference 
	- Built-in Tools
	- 3rd Party Tools
	- Spectrum Analyzer
- **Mobile Device Manager (MDM)**
	- Manage company owned and user owned devices (BYOD, bring your own device)
	- Centralized management of the mobile device
	- Set policies on apps, data, camera, etc...
	- Manage access control (have screen locks, passwords, biometrics)
- **Bring Your Own Device (BYOD)**
	- Employee owns the device
	- Difficult to secure 
		- Its both a home and work device
		- how is data protected
		- what happens to the data when a device is sold or traded in
- Corporate Owned, Personally Enabled (COPE)
	- Company owns the device, and can permit personal use
	- Organization keeps full control of the device
	- Information is protected
	- Choose Your Own Device (CYOD)
- **Cellular Network**
	- Separate land into "cells"
	- Security Concerns
		- Traffic monitoring
		- Location monitoring
		- Worldwide access to a mobile device
- **Wi-Fi**
	- Local network access
	- Same security concerns as other devices
	- Data capture (hopefully everything is encrypted)
	- On-path attack
- **Bluetooth**
	- Personal Area Network (PAN)
	- Connects our mobile devices
	- Do not connect to unknown bluetooth devices


---


# 77: Wireless Security Settings

*Anything sent in a radio frequency can be picked up by anyone*

- **WPA2 PSK Problem**
	- Listen to a four way handshake and hash
	- Attackers can capture the hash and brute force it
	- Anyone with the key can connect to the network
- **WPA3 GCMP**
	- Stronger encryption
	- Message Integrity Check (MIS)
- **SAE**
	- Mutual authentication process
	- no more four way handshake, so no hash to capture
	- SAE = Simultaneous Authentication of Equals 
	- *Dragonfly handshake*
- **Wireless Authentication Model**
	- Shared password / pre-shared key
- **Wireless Security Modes**
	- Open system (no password)
	- WPA3 personal / WPA3 PSK (pre shared key = shared password)
	- WPA3 Enterprise (Authenticate each use)
- **AAA Server**
	- *Identification*
	- AAA Framework
		- Authenticate: prove who you are (password)
		- Authorization: based on your identity what access do you have
		- Accounting: log time, data sent and received, logout time
- RADIUS (Remote Authentication Dial in Service)
	- Type of AAA server
	- Centralize authentication for users
		- connect to router / switch, login to server, access a vpn
- IEEE 802.1x
	- *Network Access Control (NAC)*
	- Don't get access to the service without a password
	- used in conjunction with RADIUS, LDAP, TACACS+
- Extensible Authentication Protocol (EAP)
	- Many ways to authenticate
	- integrates with IEEE 802.1x
- IEEE 802.1x & EAP
	- Supplicant - the client
	- Authenticator - the device that provides access 
	- AAA server - Validates the clients credentials


---


# 78: Application Security

*Secure coding concepts are often secondary*

- **Input validation**
	- Stop unexpected data
	- Document all methods: forms, fields, type
	- Check and correct input (normalization)
	- The *fuzzers* will put random data to see what happens to the app
- **Secure Cookies**
	- Cookies are info to keep data on you for a website
	- Secure cookies (only send through https)
	- Sensitive info should not be saved in a cookie
- **Static Code Analyzers**
	- Static Application Security Testing (SACT)
	- Many vulnerabilities can be found
	- Not everything can be found 
	- Still have to verify findings
- **Code Signing**
	- Potential malware is in the app...
	- Check to see if the code is sent by the manufacturer
	- Checks if the app has been changed
	- Application can be digitally signed with (Digital Certification or Certificate Authority (CA))
- **Sandboxing**
	- Only has access to data that is necessary
	- Used in development
- **Application Security Monitoring**
	- Real-time info
	- View blocked attacks 
	- Audit the logs
	- Anomaly Detection


---


# 79: Asset Management

*Be aware of what you own, how to store, use and destroy it*

- **Acquisition / Procurement Process**
	- Purchasing
	- Start from request from the user
	- Negotiate with suppliers
	- Purchase, invoice, payment
- **Assignment / Accounting**
	- Central asset tracking system
	- Ownership (associate a person with a asset, used for tracking)
	- Classification (type, hardware, software)
- **Monitoring / Asset Tracking**
	- Inventory every asset
	- Associate a support ticket with a device make and model
	- Enumeration (list parts of a asset)
	- Add a asset tag
- **Media Sanitation**
	- System disposal or decommissioning
	- Different use cases 
		- Clean hard drive for future
		- Permanently delete all data
	- One way trip
	- Reuse the storage media
- **Physical Destruction**
	- Shredder / Pulverizer
	- Drill / Hammer
	- Electromagnetic (degauss)
	- Incineration
- **Certificate of Destruction**
	- Destruction is often done by a 3rd party
	- Confirmation the drives are destroyed
	- Paper trail of broken data
- **Data Retention**
	- Backup data
	- Regulatory Compliance
	- Different data needs 


---

# 80: Vulnerability Scanning

*Test to see if a system is able to be attacked*

- **Vulnerability Scanning**
	- Minimally invasive
	- Port Scan
	- Identify System
	- Gather as much info as possible
- **Static Code Analyzer**
	- Static Application Security Testing (SAST)
	- Many vulnerabilities can be found
	- But Not everything
	- Still have to verify each finding
- **Dynamic Analysis (Fuzzing)**
	- Send random info into a application
	- Look for something out of the ordinary
	- **Fuzzing Engine and Frameworks**
		- Different options
		- Almost always a automated process
		- CERT Basic Funding Framework (BFF)
- **Package Monitoring**
	- Confirm the package is legitimate
	- Confirm a safe package


---


# 81: Threat Intelligence

*Understand threats and the people who use them*

- **Open Source Intelligence (OSINT)**
	- public sources
	- Discussion groups, social media
	- Government Data
	- Commercial Data
- **Proprietary / Third-party Intelligence**
	- Third party complies them
	- Threat intelligence services
	- Constant Threat Monitoring
- **Information-Sharing Organization**
	- Public threat intelligence
	- Private threat intelligence
	- Allows for a community to work together
	- Cyber Threat Alliance (CTA)
- **Dark Web Intelligence**
	- Dark web (TOR)
	- Find hacking groups, stores and services
	- Monitor Forums for Activity


---


# 82: Penetration Testing

*Hacking*

- NIST Technical Guide to Info and Testing Assessment
- **Rules of Engagement (RoE)**
	- Define the purpose and scope
	- Know the test parameters
	- Testing type and schedule
		- Physical
		- Online
		- 6pm
	- Rules
		- IP address range
		- Emergency Contacts
		- How to hand sensitive info
		- in-scope and out-of-scope devices and applications
- **Exploiting Vulnerabilities**
	- Try to exploit the system
	- Be careful certain attacks can cause DoS
	- You may need to try different types of attacks
	- If you can get through so can hackers
- **The Process**
	- Initial Exploitation
	- Lateral Movement
	- Persistence
	- The Pivot
- **Responsible Disclosure Program**
	- Takes time to fix a vulnerability
	- Bug Bounty Programs
	- A controlled info release


---


# 83: Analyzing Vulnerabilities

*Determining the threats*

- **Dealing with False Information**
	- False Positives / False Negative
	- Update to the latest signatures
- **Prioritizing Vulnerabilities**
	- Determine how crucial a vulnerability is 
	- Refer to public data (nvd.nist.gov)
- **Common Vulnerability Scoring System (CVSS)**
	- Quantitative scoring sheet (1-10)
	- Scoring standard can change
	- Enhanced feed sharing and collaboration
- **Common Vulnerability and Exposure (CVE)**
	- Vulnerabilities can be cross referenced
	- Some vulnerabilities are hard to determine
- **Vulnerability Classification**
	- The scanner looks for everything
	- Application Scans
		- Desktop, mobile apps
	- Web Application Scans
		- Software on a web server
	- Network Scans
		- misconfigured firewalls, open ports, vulnerable devices
- **Exposure Factor**
	- Determine the percentage of how bad a vulnerability is 
	- Difference between taking down a server (100%) and slowing its down (25%)
- **Environmental Variables**
	- What environment is the vulnerability existing in
	- Can help prioritize and patch frequency
	- Every Environment is different
		- Number and type of users
		- Revenue generating application
		- Ease to exploit will increase its priority
- **Industry / Organizational Impact**
	- Some exploits have significant consequences
		- Hospital, power plants, etc
- **Risk Tolerance**
	- The amount of risk acceptable to a organization
	- The timing for security patches
	- Testing takes time (while testing you are vulnerable)


---


# 84: Vulnerability Remediation

**

- **Patching**
	- Most common mitigation technique 
	- Schedule vulnerability / patch notices
	- Unscheduled patches (most urgent)
	- This is a ongoing process
- **Insurance**
	- Cybersecurity insurance coverage
		- Lost Revenue
		- Data recovery cost
		- Money to lost phishing
		- Privacy lawsuit costs
	- Doesn't cover everything
	- Ransomware has increased in popularity
- **Segmentation**
	- Separate devices onto their own networks / VLANs
	- A breach would have a limited scope
	- Can't patch (Disconnect it from the internet)
	- Use internal NGFWs
- **Physical Segmentation**
	- Use separate devices
	- Or do it digitally with Virtual Local Area Networks (VLAN)
- **Compensating Controls**
	- Optimal Security methods
	- Compensate in other ways
		- Disable problematic services
		- Revoke Access to the application
		- Limit external access
		- Modify internal security controls and software firewalls 
	- Provide coverage until a application is deployed
- **Exceptions and Exemptions**
	- Removing the vulnerability is optimal (but not everything can be removed)
	- A balancing act
	- Not all vulnerabilities are the same severity
	- An exemption may be an option
- **Validation of Remediation**
	- The vulnerability is now patched
		- Did it stop the vulnerability
		- Did you patch all the systems
	- Rescanning (Preform a vulnerability scan)
	- Audit
	- Verification
- **Reporting** 
	- Ongoing Checks are Required
	- Difficult or impossible to do without automation
	- Continuous reporting
		- number of identified vulnerabilities
		- Systems patched vs unpatched
		- New threat notifications
		- Errors, exceptions, and exemptions


---


# 85: Security Monitoring

*Constantly monitor, the vast amount of entry points that also keep increasing*

- **Monitoring Computing Resources**
	- **System Monitoring**
		- Authentication - logins from strage places
		- Server monitoring - Service activity, backups, software versions
	- **Application Monitoring**
		- Availability - uptime and response times
		- Data transfers - increases or decreases in rate
		- Security notifications - from the developer / manufacturer
	- **Infrastructure**
		- Remote access systems - employees, vendors, guests
		- Firewall and IPS reports - increase or type of attack
- **Log Aggregation**
	- Security Information and Event Manager (SIEM)
	- Centralized Reporting
	- Correlation between diverse systems
- **Scanning**
	- Constantly changing threat landscape
		- *e.g. new vulnerabilities, apps, services*
	- Actively check systems and devices
	- Gather the raw details
- **Reporting**
	- Analyze the collected data
	- Status information
	- Determine best next steps
	- Ad hoc information summaries (e.g. prepare for the unknown)
- **Archiving**
	- IBM 2022 - Takes about 9 months to identify and contain a breach
	- Access to (old & new) data is critical
	- May have a mandate to collect data over a certain amount of time
- **Alerting**
	- Real-time notification of security events
		- *e.g. large amount of authentication failures, large file transfers, remote access*
	- Actionable data
	- Notification methods
- **Alert Response and Remediation**
	- Quarantine
	- Alert tuning (prevent false positives)
	- An alert should be accurate


---


# 86: Security Tools

*Tools to measure security effectiveness*

- **Security Content Automation Protocol (SCAP)**
	- Many tools to evaluate a threat in different ways...
	- Allows tools to identify and act on the same criteria
- **Using SCAP**
	- SCAP content can be shared between tools
	- Especially useful in large environments
	- This specification standard enables automation
	- Automation types
		- *e.g. ongoing monitoring, notification alerts, remediation of non compliant systems*
- **Benchmarks**
	- Apply security best-practices to everything
	- Example: mobile device
		- Disable screenshots, disable voice calls when locked, force encryption
		- Popular benchmark is Center for Information Security (CIS)
- **Agents / Agent-less**
	- Check to see if the device is in compliance
	- Agents can usually provide more detail
- **SIEM**
	- Security Information and event Managment
	- Log collection of security alerts
	- Data correlation
	- Forensic analysis
- **Anti-virus and Anti-malware**
	- Malware refers to a broad category
	- Terms are effectively the same
- **Data Loss Prevention (DLP)**
	- Know where your data is stored
	- Stop the data leakage
- **Simple Network Management Protocol (SNMP)**
	- Database of data (MIB) - Management Information Base
	- Database containing OIDs - Object Identifiers
	- Request statistics from a device (poll devices over udp/161)
- **SNMP Traps**
	- SNMP Traps can be configured on the monitored device
	- Set a threshold for alerts
- **Netflow**
	- Gather traffic statistics from all traffic flows
	- Probe and collector
	- Usually a separate app
- **Vulnerability Scanner**
	- Minimally invasive
	- Port scan
	- Identify systems
	- Test from the outside and the inside
	- Gather as much info as possible


---


# 87: Firewalls

*Internet traffic rules to stop certain types of data from entering or leaving*

- **Network-based Firewalls**
	- Filter traffic by port number or application
	- Encrypt traffic
	- Most firewalls can be layer 3 devices (router)
- **Next-Gen Firewall (NGFW)**
	- The OSI application layer (layer 7)
	- *Also called application layer gateway, state full multi layer inspection, deep packet inspection*
	- Requires some advanced decodes
- **Ports and Protocols**
	- Make forwarding decisions based on protocol (TCP or UDP) and port number
	- Based on destination
- **Firewall Rules**
	- A logical path
	- Specific rules at the top
	- Implicit deny 
		- *e.g. step through each rule, but if no rule passes just deny*
	- Access Control Lists (ACLs)
- **Screened Subnet**
	- An additional layer of security
	- Internet traffic can be routed to a subnet that doesn't hold sensitive info within the internal network
- **IPS Rules integrated with NGFW**
	- Different ways to find malicious traffic
	- Signature-based
	- Anomaly-based 
		- After building a normal, unusual patters can be flagged
	- You determine what happens when unwanted traffic appears
	- Thousands of rules
	- Rules can be customized by group


---


# 88: Web Filtering

*Parental controls*

- **Content filtering**
	- Control traffic based on data within the content
	- Corporate control of outbound and inbound data
	- Control of inappropriate content (parental controls)
	- Protection against "evil" sites
- **URL Scanning**
	- Allow or restrict based on Uniform Resource Locator (URI)
	- Managed by category
		- *e.g. Auction, Hacking, Malware, Travel, Recreation, etc*
	- Can be limited
	- Often integrated into an NGFW
- **Agent Based**
	- Install client software on the user's device
	- Users can be located anywhere (and filter still works)
	- Updates must be distributed to all agents
- **Proxies**
	- Sits between the users and the external network
	- Receives the user request and sends the request on their behalf (The proxy)
	- Useful for caching information, access control, URL filtering, content scaninng
	- Applications may need to know how to use the proxy (explicit)
	- Some proxies are invisible (transparent)
- **Forward Proxy**
	- A centralized "internal proxy"
	- Used to protect and control user access to the internet
- **Block Rules**
	- Based on specific URL
	- Category of site content
	- Different dispositions
- **Reputation**
	- Filter URLs based on perceived risk
		- Good reputation is allowed
		- Bad can be blocked
	-  Risk: trustworthy, low risk, medium risk, suspicious, high risk
	- Automated reputation
	- Manual Reputation
	- Add these dispositions to the URL filter
- **DNS Filtering**
	- Before connecting to a website, get the IP address
	- DNS is updated with real-time threat intelligence
	- Harmful sites are not resolved
	- This works for any DNS lookup


---


# 89: Operating System Security

*Use Linux*

- **Active Directory**
	- Database containing everything on the network
	- Manage authentication
	- Centralized access control
	- Commonly used by the help desk
- **Group Policy**
	- Manage the computers or users with group policies
	- A central console
	- Comprehensive control
- **Security-Enhanced Linux (SELinux)**
	- Security patches for the Linux kernel
	- Limits application access
	- Open source


---


# 90: Secure Protocols

*Encrypt your traffic, aka make them use secure protocols*

- **Unencrypted Network Data**
	- Network traffic is important data
	- Some protocols aren't encrypted
	- Verify with a packet capture
- **Protocol Selection**
	- Use a secure application protocol 
	- A secure protocol may not be available
- **Port selection**
	- Secure and insecure applications use different ports for encrypted and unencrypted
	- HTTP = 80 and HTTPS = 443
	- The port number does not guarantee 
- **Transport Method**
	- Don't rely on the application
	- 802.11 Wireless
		- Open access point: no transport-level encryption
		- WPA3: all user data is encrypted
	- Virtual Private Network (VPN)
- **VPN Tunnel**
	- May need a concentrator
	- More software
	- Paid Service


---


# 91: Email Security

*Emails are a door into your computer...*

- **Mail Gateway**
	- *The gatekeeper*
	- Evaluates the source
	- Blocks bad content
	- On-site or cloud based
- **Sender Policy Framework (SPF)**
	- SPF protocol (configures a list of servers who are authorized to send emails for a domain)
	- Check DNS TXT record to see if it came from the right place
- **Domain Keys Identified Mail (DKIM)**
	- A mail server signs all outgoing mail (public key is in the DKIM TXT record)
	- Signature is validated by the receiving mail servers
- Domain-based Message Authentication Reporting, and Conformance (DMARC)
	- Extension SPF
	- Decide what to do with spoofed emails
		- Accept all, send to spam, or reject the email
	- Compliance reports are sent to the email administrator


---


# 92: Monitoring Data

*Watch inbound and outbound data to identify problems*

- **File Integrity Monitoring (FIM)**
	- Some files change all the time while others never change
	- Monitor important operating system and application files
	- Windows - SFC (System File Checker)
	- Linux - Tripwire
	- Many host-based IPS options
- **Data Loss Protection (DLP)**
	- Data in use 
		- Monitoring data in the active memory
		- Endpoint DLP
	- Data in motion
		- Monitoring packets in real time
	- Data at rest
		- On server
		- In storage
- **USB Blocking**
	- 2008 US D.O.D worm "agent.btz" replicates using usb storage
		- Banned removable flash media and storage device
	- All devices had to be blocked 
	- Ban was lifted in 2010
- **Cloud-based DLP**
	- Located between users and the internet
	- Block custom defined data strings
	- Manage access to URLs
	- Block viruses and malware
- **DLP and Email**
	- Check every email inbound and outbound
		- Inbound: Find keywords, identify impostors, quarantine emails
		- Outbound: Fake wire transfers, W-2 Transmissions, employee information


---

# 93: Endpoint Security

*Securing the device used by the user*

- **Edge Control**
	- Where the inside of the network meets the outside
	- Firewall to monitor all traffic
	- Managed through static firewall security rules
- **Access Control**
	- Ability to limit a devices access to a certain type of data
	- Create policies, like groups, where the device is, and where the data is
- **Posture Assessment**
	- Can't trust everyone's computer
	- Malware infection / Lack of Anti-virus
	- Unauthorized apps
	- Check *before* a device connects to a network
- **Health Checks**
	- Persistent Agents
		- Permanently installed on system that performs checks
	- Dissolvable Agents
		- Performs checks then terminates itself after its done
	- Agentless Network Access Control (NAC)
		- Integrated with active directory
		- Checks are made during login and logoff
- **Failing Your Assessment**
	- What happens if it fails
	- Quarantine network, notify admins
	- Once resolved try again
- **Endpoint Detection and Response (EDR)**
	- Detect a threat with more than just signatures
	- Behavioral and Root Cause Analysis
	- Respond to the threat
- **Extended Detection and Response (XDR)**
	- A improvement on EDR
- **User Behavior Analytics**
	- Extends a scope to anomaly detection
	- Watch user, hosts, network traffic, data repositories 
	- Watch for anything unusual


---


# 94: Identity and Access Management (IAM)

*Give the right permissions to the right people*

- **Provisioning / de-provisioning User Accounts**
	- User account creation
	- Occurs for certain events
		- *e.g. hiring, firing, promotions*
	- Account details
	- Important part of IAM
- **Permission Assignment**
	- Each entity gets limited permissions
		- *Just enough to do their job*
	- Storage and files can be private to that user
	- NO privileged access to the OS
- **Identity Proofing**
	- IAM should confirm who you are
	- Resolution (Who the system thinks you are)
	- Validation (password, security questions)
	- Verification / Attestation (passport, in person meeting)
- **Single Sign-on (SSO)**
	- Provide credentials once
	- Usually limited by time
- **Lightweight Directory Access Protocol (LDAP)**
	- Protocol for read/write directories over IP network
- **X.500**
	- Distinguished names
	- Directory Information Tree
- **Security Assertion Markup Language (SAML)**
	- Open standard for authentication and authorization
	- Not originally made for devices
- **OAuth**
	- Authorization framework
	- Created by Twitter, Google, and many others
	- Not a authentication protocol 
- **Federation**
	- Instead of creating a new account, use a account that is already approved
		- *"Login with Google"*
	- Third parties must have a trusting relationship
- **Interoperability**
	- Many different ways to communicate with an authentication server
	- Often determined by what is at hand
	- A new app uses OAuth (now you have to provide a way to be interoperable)


---


# 95: Access Controls

*Who gets access and how*

- **Least Privilge**
	- Give accounts least amount of permission
	- This can lower a hacked accounts scope
- **Mandatory Access Control (MAC)**
	- Operating system may limit a operation 
	- Every object gets a label
		- *e.g. Confidential, Secret, Top Secret, etc.*
- **Discretionary Access Control (DAC)**
	- Used in most operating systems
	- Very flexible access control
- **Role-Based Access Control (RBAC)**
	- You have a role in your organization (Windows = groups)
	- Administrator provide access based on the role of the user
- **Rule-Based Access Control**
	- Generic term for following rules
	- Access is determined through system-enforced rules
	- The rule is associated with the object
- **Access-Based Access Control (ABAC)**
	- Users have complex relationships to applications and data
	- ABAC can consider many parameters
- **Time-of-day Restrictions**
	- Restrict access during certain times
	- Can be difficult to implement in a world wide organization


---


# 96: Multifactor Authentication

*Something you know, have, are, or location*

- **Something You Know**
	- Password
	- PIN (Personal Identification Number)
	- Pattern
- **Something You Have**
	- Smart Card
	- USB Security Key
	- Hardware or software token
	- Your phone (SMS)
- **Something You Are**
	- Biometrics
		- Fingerprint, iris scan, voice print
	- Difficult to change
	- Not foolproof
- **Somewhere You Are**
	- Login from the wrong country
	- IP address
	- Mobile Device Location Services


---


# 97: Password Security

*Create strong passwords, use a manager*

- **Password** 
	- Age and expiration
	- Length
	- Complexity
	- Non common phrases
	- No repeating passwords
- **Password Manager**
	- Reminders to reset password
	- Check password strength
	- Store many passwords in one place
- **Password less authentication**
	- Many breaches are due to weak passwords
	- Authenticate without a password
		- *Facial recognition, security key, etc*
	- Used with more factors
- **Just-in-time permissions**
	- Grant admin access for a limited amount of time
	- Narrow the scope of privilege for a attacker
	- Request access from a clearing house
	- Password vaulting
	- Accounts are temporary


---


# 98: Scripting and Automation

*A script can complete tasks for you*

- **Automation Benefits**
	- Save time
	- Enforce baselines
	- Standard infrastructure and configurations
	- Secure scaling
	- Employee Retention
	- Reaction time
	- Workforce multiplier
- **Cases for Automation**
	- User and resource provisioning (hiring / firing)
	- Guard rails 
	- Security groups (constantly changing)
	- Ticket creation
	- Escalation 
	- Controlling services and access
- **Scripting Considerations**
	- Has to interact with other systems
	- Cost of creating the code (time / money)
	- Single point of failure
	- Technical debt
		- *e.g. solving symptoms instead of the core problem*


---


# 99: Incident Response

*Handling a hack or problem*

- NIST SP800-61
- **Preparing for a Incident**
	- Contact list
	- "Go bag" 
		- *e.g. hardware and software designed for handling a incident*
	- Incident analysis resources
		- *e.g. documentation, pictures, etc*
	- Incident mitigation software
	- Policies needed to handle a incident
- **Detecting a Incident**
	- Many different detection sources
	- A large amount of volume
	- Incidents are almost always complex
- **Analysis**
	- Web server log
	- Exploit announcements 
	- Direct threats (someone claims to attack you)
	- IPS or IDS usage and logs
- **Isolation and Containment**
	- Stop them immediately
	- Sandbox attacks and red team practice
	- Isolation can be problematic
		- e.g. services can get effected, malware may self destruct if it knows its in a sandbox
- **Recovery After an Incident**
	- Get things back to normal
	- Eradicate bug
	- Recover the system
		- *e.g. restore backups, rebuild from scratch, replace compromised files, tighten down perimeter*
- **Incident Lessons**
	- ASAP Do meeting that discuss the incident
	- Create better plans
	- Ask questions
		- *e.g. what happened, what was the timeline, how was our documentation and how did we do, what were the indicators*
- **Training for a Incident**
	- Train before a incident
	- What to do
		- Initial response
		- Investigation plan
		- Incident reporting
	- Training may be costly but a incident could cost more


---


# 100: Incident Planning

*Prepare and plan for a incident to have a better response*

- **Exercising**
	- Test yourself before a event
	- Define rules of engagement
	- Verify specific scenario
	- Make it timed based
	- Evaluate response
- **Tabletop Exercises**
	- Cheaper than a real attack
	- Many logistics can be determined
	- Get key players together for a table top exercise
- **Simulation**
	- Test with a simulated event
		- *e.g. Sending phishing emails*
	- Test internal security
	- Test the users
- **Root Cause Analysis**
	- Determine the ultimate cause of an incident
	- Create a set of conclusions regarding the incident
	- Don't get tunnel vision
	- Mistakes happen
- **Threat Hunting**
	- Find a vulnerability before a attacker does
	- Intelligence data is reactive
	- Speed up the reaction time


---


# 101: Digital Forensics

*Collect data relating to intrusions, and be as detailed as possible*

- **Legal Hold**
	- Legal technique used to reserve relevant information
	- Separate repository stored as Electronically Stored Information (ESI)
	- Ongoing obligation to preserve data
- **Chain of Custody**
	- Maintain integrity
	- Chain of custody logs everyone who had the data
	- Avoids tampering
	- Label and catalog everything
- **Acquisition**
	- How to obtain the data
	- Some data may be on other systems
	- You can get a snapshot of a VM
	- Look for any left behind digital items like artifacts
- **Reporting**
	- Document the findings
	- Summarize information
	- Detailed explanation
	- Create a conclusion
- **Preservation**
	- Handling the evidence
	- Manage the collection process
	- Work with copies and not the real data
	- Live collection has become an important skill
	- Follow best practices 
- **E-discovery**
	- Collect, prepare, review, interpret, and produce electronic documents
	- Works together with digital forensics


---


# 102: Log Data

*The files that hold the actions of computers*

- **Security Log Files**
	- Detailed security-related information
		- Blocked traffic
		- Exploit attempts
		- Blocked URL categories
		- DNS sinkhole traffic
	- Critical security information
- **Firewall Logs**
	- Traffic flows through the firewall
	- Check the source / destination IP, ports, and disposition
	- Next gen firewall (NGFW)
- **Application Logs**
	- Specific applications have logs
- **Endpoint Logs**
	- Attackers often gain access through endpoints
	- There's a lot of data at endpoints
	- Use with correlation with other logs
- **OS-Specific Security Logs**
	- OS security events
	- Find problems before they happen
		- *e.g. a certain service is disabled or enabled*
	- May require filtering
- **IPS / IDS Logs**
	- Logs contain info about predefined vulnerabilities
- **Network Logs**
	- Switches, routers, access points, VPN concentrators 
	- Network changes
- **Metadata**
	- Data that describes other data sources
	- You often don't see this data
	- Pictures have a lot of metadata
		- *e.g. time, place, size, owner, phone*
- **Vulnerability Scans**
	- Find lack of security controls
	- Find misconfigurations
	- Real vulnerabilities
- **Automated Reports**
	- SIEM may include a report generator
	- Requires human intervention
	- Requires data storage and processing power
- **Dashboards**
	- Real-time status info
	- Add or remove info
	- Shows the most important data
- **Pocket Captures**
	- Solve complex application issues
	- Gathers packets on the network (third party app like wireshark)
	- View detailed info about traffic flow


---


# 103: Security Policies

*Rules that everyone needs to follow to stay safe*

- **Acceptable Use Policies (AUP)**
	- How devices and the internet can be and can't be used
	- Limit legal liability
- **Business Continuity Policy**
	- Have alternatives
	- Plan before the issue arrives
- **Disaster Recovery Plan**
	- Ready for a disaster
	- Be prepared for every type of disaster
	- Have a comprehensive plan
		- Recovery location
		- Data recovery
		- Application restoration
		- IT team and employee availability 
- **Security Incident Policy**
	- Have a way to stop incidents
		- Phishing
		- DDoS
		- Confidential info stolen
- **Incident Response Team Policy**
	- A team dedicated to incidents
	- Trained and tested
	- Compliance officers
	- Technical Staff
	- User community
- **NIST SP800-61 Revision 2**
	- A guide for the response life cycle
		- Preparation
		- Detection and Analysis
		- Containment, Eradication, and Recovery
		- Post-incident Activity
- **Software Development Lifecycle (SDLC)**
	- Get a idea into a app
	- There's no best way, but there is frameworks
		- Waterfall: goes through all the steps linearly 
		- Agile: A circular development
- **Change Management Policy**
	- One of the most common risks
	- How to make a change
		- Upgrade software, change firewall configuration, modify switch ports
	- Have clear policies
	- Sometimes difficult to implement


---


# 104: Security Standards

*Create storage standards and minimums to be followed*

- **Password Standards**
	- Create a formal password complexity policy
	- Define acceptable authentication methods
	- Policy for a password reset
- **Access Control Standard**
	- Determine what information is used, and what time and circumstances
	- Define access control types (*e.g. No discretionary, mandatory only, etc.*)
	- Determine how a user gets access
	- Document how access may be removed
- **Physical Security Standard**
	- Regard physical Security controls
	- Grant physical access (*e.g. employee vs visitor*)
	- Define specific security systems
- **Encryption Standard **
	- Define the type of encryption that should be used
	- Also have the implementation of the use of encryption
	- Data encryption minimums


---


# 105: Security Procedures

*Procedures meant to be followed for maximum security*

- **Change Management**
	- Formal process of managing change
		- Determine the scope
		- Analyze the risks
		- Create a plan
		- Get user-end approval
		- Present the proposal
		- Backup plan
		- Document changed
- **On-boarding**
	- Bring a new person into the org
	- IT agreements need to be signed
	- Create accounts
- **Off-boarding**
	- What happens to their hardware and data
	- Disable their account once they are gone
		- Don't delete this could be problematic
- **Playbooks**
	- Conditional steps for every type of attack
	- Step by step process or guide
	- Can be automated
	- Integrated with a SOAR platform
- **Monitoring and Revision**
	- Security must change with real world
	- Update security postures
	- Change steps in playbooks
	- Understand new security threats
- **Governance Structures**
	- Board
		- A panel of specialist 
		- Set tasks and requirements for the committees
	- Committees
		- Subject-matter experts
		- Considers input from the board
		- Determines next step for a topic at hand
		- Presents the results to the board
	- 
	- Government Entities
		- Legal concerns
		- Admin requirements
		- Political issues
	- 
	- Centralized / Decentralized
		- Centralized - one location that makes the decisions
		- Decentralized - spreads the vote 

---


# 106: Security Considerations

*Understanding when and how to implement security*

- **Regulations**
	- Regulations are foundational
	- Sarbanes-Oxley Act (SOX)
		- The Public Company Accounting reform and investor Protection act of 2002
	- Health Insurance Portability and Accountability (HIPAA)
		- How personal medical info is handled, disclosed and transferred
- **Legal**
	- Formal set of procedures to report illegal activities
	- Responsible for holding evidence
	- Disclosure of security breach
	- Cloud computing creates a lot of challenges
- **Industry**
	- Differences for security in environments
		- e.g. Electrical utility vs Medical
-  **Geographical Security**
	- Local / Regional laws are different
	- City may collect certain data
	- National level data, will need more security
	- Global will have the most concerns, with legal, regulations and security


---


# 107: Data Roles and Responsibility

*Broad term of roles of control*

- **Data Responsibilities**
	- The data owner is responsible
	- They have to keep it safe
- **Data Roles**
	- Data controller - how it will be used
	- Data processor -  using the data
		- e.g. payroll department (controller) and payroll company (processor)
	- Data custodian - security, accurate, private
		- Makes sure org is in compliance 
		- Applies sensitivity labels to data
		- Controls what user can access what data


---


# 108: Risk Management

*Finding and documenting risks*

- **Risk Identification** 
	- Identify and address risks
	- Larger organization, the more risks
- **Performing a Risk Assessment**
	- Not all risks require constant evaluation
	-  One-time vs Continuous Assessment
- **Ad Hoc (for this purpose only)**
	- Performing something for one thing only
	- Learning about a threat then checking for it
	- Create a committee that will test then document 
- **Recurring Assessment**
	- Scheduled tests every 3-6-12 months
	- Internal team may request updates
	- Mandated risk assessment depending on what is stored


---


# 109: Risk Analysis

*Determining if its worth it*

- **Qualitative Risk Assessment**
	1. Risk Factor - *Legacy windows client*
	2. Impact - *medium*
	3. Annualized rate of Occurrence - *high*
	4. Cost of Controls - *medium*
	5. Overall Risk - *high*
- **Quantitative Risk Assessment**
	- ARO (Annualized Rate of Occurrence): How likely it will hit
		- = ARO * EF
		- e.g. 12 (ARO) x 1.0 (EF) = $12,000 (SLE)
	- Asset Value (AV): Value to the organization (not the price to purchase)
	- Exposure Factor (EF): percentage lost to a risk
		- e.g. losing a entire asset 1.0 and quarter is .25
	- SLE (Single Loss Expectantancy): loss of money one event
		- = AV * EF
		- e.g. $1,000 (AV) x 1.0 (EF) = $1,000 (SLE)
	- ALE (Annualized Loss of Expectancy)
		- = ARO * EF
		- e.g. 12 (ARO) x 1.0 (EF) = $12,000 (SLE)
	- **Impact**
		- Life is the most important consideration
		- Property or the risk to buildings and assets
		- Safety, risk of injury
		- Finance, resulting cost 
	- **Likelihood and Probability**
		- Likelihood - qualitative
		- Probability - quantitative
	- **Risk Appetite and Tolerance**
		- Risk appetite posture is readiness to take risk
			- Conservative, neutral, and expansionary
		- Risk tolerance is the amount they can risk
	- **Risk Register**
		- Each risk is detailed
		- Offers solutions to avoid risk
		- Monitor the results


---


# 110: Risk Management Strategies

*Avoid, Mitigate or accept it*

- **Risk Transfer:** Accepting the risk or purchasing cyber security insurance
	- Exemptions will need approval
- **Avoid and Mitigate**
- **Risk Reporting:** A list of risks and how to manage them

---


# 111: Business Impact Analysis

*Time is money!*

- **Recovery Time Objective (RTO):** how quickly it takes to get a system running
- **Recovery Point Objective (RPO):** At what point are we recovered
	- e.g. we need at least 50% processing power
- **Mean Time to Repair(MTTR):** Average time required to fix something
- **Mean Time Between Failures (MTBF):** How risky it is to use a piece of equipment
	- Up-time / failures = MTBF


---


# 112: Third-Party Risk Assessment

*Can you trust your partners?*

- **Third-party Risk:** the people you are working with are given trust, so know who they are and put them under contracts
- **Penetration Testing Risk:** 
- **Rules of Engagement:** Determine what devices, time, and areas are allowed to be attacked
- **Right-to-Audit Clauses:** Business partners may be holding your companies info, add this clause to be able to audit the partner
- **Evidence of Internal Audit:** 
	- May be required, 
	- Have a third-party perform a audit and check their security controls
	- Perform at a reasonable frequency
- **Supply Chain Analysis:** Check the process of creating a product, and where security concerns may lie
- **Independent Assessments:** Bring a outside firm to determine security concerns
- **Vendor Selection Process:** 
	- Due Diligence: investigating and verifying information provided
	- Conflicts of interest: when a company may be a competitor or friend of one
- **Vendor Monitoring:** Review the vendor and outside sources of the vendor such as the news. 
	- **Questionnaires:** Ask about security controls, devices, and processes


---


# 113: Agreement Types

*Legal bindings and contracts*

- **Service Level Agreement (SLA):** Minimum terms of service
- **Memorandum of Understanding (MOU):** broad goals of what they will accomplish together, very informal. 
- **Memorandum of Agreement (MOA):** In detail description of partnership, more formal
- **Master Service Agreement (MSA):** Legal contract that sets the terms and can cover future transactions
	- Work Order (WO) / Statement of Work (SOW)
		- Describes the expectations and answer questions
- **Non-Disclosure Agreement (NDA):** Keep confidentiality between two parties, protects user confidential info
	- One or both parties have to keep confidentiality
- **Business Partners Agreements (BPA):** who makes the decisions, detailing the contingencies, and more


---


# 114: Compliance

*Series of standards to follow*

- **Lots of legal stuff**
- Monitor your own compliance so you don't break rules
	- Internal or External
- You can lose selling license
- Can get felonies for breaching privacy such as HIPAA or GLBA


---


# 115: Privacy

*How to handle sensitive personal info*

- **General Data Protection Regulation (GDPR):** In the EU its a privacy law, and users can request to remove their info. Giving the user the right to be forgotten
- **Data Subject:** is everyone with PII
- **Data Responsibility**
	- Data owner: accountable for specific data
- **Data inventory and Retention:** A list of all the data they collect, the owner, how often its updated, and the format
	- Internal Use: Projects, it security, quality checks
	- External Use: Select data to share publicly and follow existing laws and regulations


---


# 116: Audits and Assessments

*Running audits lets us examine all our tech*

- **Internal Audits:**
	- Check for compliance
	- Have a audit committee who starts and stops the audit
- **External Audits:**
	- May be required by regulation
	- Let a third party gather and compile info


---


# 117: Penetration Tests

*Test the companies security*

- **Physical Penetration Tests:** Test the effectiveness of physical security
- **Pentesting Perspectives:**
	- Red team - Offensive
	- Blue team - Defensive
	- Integrated (Purple Team) - combine the two
- **Working Knowledge:** How much do you know about the test 
	-  Known Environment: Full disclosure
	- Partially Known: a mix focused on certain applications
	- Unknown Environment: The pentester knows nothing about the systems
- **Reconnaissance:** 
	- Need info before the attack 
	- Collect the digital footprint 
	- Minimize the attack area
	- Create a network map
- **Passive Reconnaissance:**
	- Learn as much from open sources
	- Social media, web site, online forums, reddit, social engineering, dumpster diving, 
- **Active Reconnaissance:** 
	- Trying the doors 
	- ping, port, OS scans


---


# 118: Security Awareness

*Check how well employees do*

- **Phishing Campaigns:** 
	- Test the people
	- Automate the process
	- Be able to recognize
	- Asking for personal info?
	- Check if email filtering is working
- **Anomalous Behavior Recognition:** 
	- Check risky behavior
	- Check unexpected behavior
	- Check unintentional behavior
- **Reporting and Monitoring:**
	- Automate alerts
	- Log the data and make it readable
	- Check if something is a one time thing or reoccurring
- Create a Security Awareness Team
	- Establish minimum awareness level
	- Integrate compliance mandates
	- Define metrics
- **Execution**
	- Create training material
	- Document the metrics
	- Identify the stakeholders
	- Deploy training materials


---


# 119: User Training

**

- **Security Awareness Training:**
	- Before giving access
	- Specialized training for roles
	- Also applies to third parties
	- Document who has been trained, and who hasn't
- **User Guidance and Training:**
	- Provide Policies / Handbooks
	- Situational Awareness
	- Insider Threats
	- Password Management
	- Be aware of media and cables
	- Social Engineering Awareness
	- Operational Security
	- Security measures for hybrid or remote work1