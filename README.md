# CompTia-Security-SY0-701-notes

Hi All, I completed my exam on the 16th of August 2024 after roughly a month of self study. I used a range of resources found on [O'Reilly](https://www.oreilly.com/), ranging from the [certification guide](https://www.oreilly.com/library/view/comptia-security-sy0-701/9781835461532/), a video course by [Sari Green](https://www.oreilly.com/library/view/comptia-security-sy0-701/9780138251062/) and [practice exams.](https://www.oreilly.com/library/view/comptia-security-sy0-701/9780138225568/) 

ProfesserMesser's [YouTube Playlist, CompTIA SY0-701 Security+ Training Course ](https://www.youtube.com/playlist?list=PLG49S3nxzAnl4QDVqK-hOnoqcSKEIDDuv) was my main study resource where most of my notes were derived from, I used other tools to help me better understand concepts I was struggling with. 

I used [Free labs](https://www.101labs.net/comptia-security/) for hands on practical experience a day before taking my exam.**(Note that you will need your own VM with a Linux distro installed to complete these.)**

I made flash cards to help me memorise the most common TCP/UDP and their uses: 

TCP Ports: 20/21, 22, 23, 63, 80,110, 143, 443, 445, 3389.

UDP Ports: 53, 67/68, 69, 88, 636 89/990, 993, 995, 6154.

My final and one of the more useful resources was this [Reddit post].(https://www.reddit.com/r/CompTIA/comments/zkjs1d/how_a_dumdum_like_me_passed_sec/?utm_source=share&utm_medium=ios_app&utm_name=iossmf)

I am a full time student in Australia and was able to get a **50% voucher** after emailing CompTia and verifying my student status.

<img src="https://github.com/Feshovski/CompTia-Security-SY0-701-notes/blob/main/CompTIA%20Certificate.png?raw=true" width="600"/>

**Please note that for a lot of these concepts I went into a lot more detail that is required to better prepare myself for the future.**

<details>
<summary>Key Information Security+ Exam</summary>

# How to pass your SY0-701 Security+ Exam

## Pre-text

The most popular technology certification in the world

### Career Growth
- Security+ builds a great foundation

### Professional prerequisite
- Personal knowledge and satisfaction.

### Computing Technology Industry Association (CompTIA)
- The largest provider of vendor-neutral IT certifications
- Members include IT resellers, IT distributors, IT manufacturers, and IT training centers.

---

## Exam Specifications:

- **90-minute exam**, maximum of **90 questions**
- **Passing score**: 750 on a scale of 100-900

| Domain | % of Exam |
|--------|-----------|
| 1.0 - General Security Concepts | 12% |
| 2.0 - Threats, Vulnerabilities, and Mitigations | 22% |
| 3.0 - Security Architecture | 18% |
| 4.0 - Security Operations | 28% |
| 5.0 - Security Program Management and Oversight | 20% |

---

## Exam Types:

- **Multiple Choice**
  - Single, multiple answers

- **Performance-based**
  - Complete a task
  - Matching, sorting, drag-and-drop, etc.

---

## CompTIA Certification Objectives

- [Exam objectives](https://www.comptia.org/training/resources/exam-objectives/comptia-security-701-exam-objectives)
- Get as much hands-on as possible
- CompTIA Security+ labs


</details>

<details>
<summary>1.0 General Security Concepts</summary>
  
# 1.1 Security Controls
  
Security controls help prevent security events to help minimize impact and limit damage done by threat actors. Assets to consider are data, physical property, computer systems, and more.

### Technical Controls: Controls implemented using systems
- Operating system control
- Firewalls, anti-virus, etc.

### Managerial Controls: Administrative controls associated with security design and implementation
- Security policies, standard operating procedures
- Governance, policies, procedures, and strategies for managing risk within an organization
- Typically associated with legal

### Operational Controls: Controls implemented by people instead of systems
- Security guards, awareness programs
- Guard Shack

### Physical Controls: Limits physical access
- Guard shack can be physical or operational
- Fences, locks
- Badge readers

### Security Controls Categories
| Categories   | Preventive           | Deterrent            | Detective            | Corrective         | Compensating        | Directive                     |
|--------------|----------------------|----------------------|----------------------|--------------------|---------------------|------------------------------|
| Technical    | Firewall             | Splash Screen        | System logs          | Backup recovery    | Block instead of patch | File Storage policies        |
| Managerial   | On-boarding policy   | Threat of demotion   | Review login reports | Policies for reporting issues | Separation of duties | Compliance policies          |
| Operational  | Guard shack          | Front Reception Desk | Property patrols     | Contacting law enforcement | Guard duties        | Security Policy Training     |
| Physical     | Door lock            | Posted Warning Sign  | Motion detectors     | Fire Extinguisher  | Backup generator    | Signs: Authorised personnel only |

These are not inclusive lists: There are many categories of controls, and some organizations will combine types. There are multiple security controls for each category and type. Some security controls may exist in multiple types or categories. New security controls are created as systems and processes evolve. Your organization may use very different controls.

### Types of Security Controls

### Preventive: Blocks access to a resource
**Prevent access:**
- Firewall rules
- Follow security policy
- Guard shack checks all identification
- Enable door locks

### Deterrent: Discourages an intrusion attempt, does not directly prevent access
**Makes an attacker think twice:**
- Application splash screens
- Threat of demotion
- Front reception desk
- Posted warning signs

### Detective: Identify and log an intrusion attempt, may not prevent access
**Find the issue:**
- Collect and review system logs
- Review login reports
- Regularly patrol the property
- Enable motion detectors

### Corrective: Apply a control after an event has been detected, reverse the impact of an event, and continue operating with minimal downtime
**Correct the problem:**
- Restoring from backups can mitigate a ransomware infection
- Create policies for reporting security issues
- Contact law enforcement to manage criminal activity
- Use a fire extinguisher

### Compensating: Control using other means, existing controls aren't sufficient, may be temporary
**Prevent the exploitation of a weakness:**
- Firewall blocks a specific application instead of patching the app
- Implement a separation of duties
- Require simultaneous guard duties
- Generator used after power outage

### Directive: Direct a subject towards security compliance, a relatively weak security control
**Do this, please:**
- Store all sensitive files in a protected folder
- Create compliance policies and procedures
- Train users on proper security policy
- Post a sign for "Authorised Personnel Only"

# 1.2 The CIA Triad

The CIA Triad is an easy way to remember the fundamentals of I.T Security.

![image](https://github.com/user-attachments/assets/85255377-34d1-4bb9-98c7-9d9479815c8f)


### Confidentiality:
- Prevent disclosure of information to unauthorized individuals or systems.

### Integrity:
- Ensure data is stored and transferred as intended.

### Availability:
- Systems and networks must be up and running.

## Diving deeper into the above:

### Confidentiality: Certain information should only be known to certain people.
- Prevent unauthorized information disclosure.
- Encrypt messages so only certain people can read them.
- Selectively restrict access to a resource using access controls.
- Two-factor authentication.

### Integrity: Data is stored and transferred as intended.
- Any modification to the data would be identified.
- Hashing ensures integrity by producing a unique hash value for data; the value will change if the data is altered in any way.
- Digital signatures take a hash and encrypt it with an asymmetric encryption algorithm to further verify the integrity of the data.
- Certificates combined with digital signatures will further ensure verification.
- Non-repudiation provides proof of integrity, and can be asserted to be genuine.

### Availability: Information is accessible to authorized users.
- **Redundancy**: Build services that will always be available.
- **Fault tolerance**: Ensure that a system will continue to run even when a failure occurs.
- **Patching**: Ensure the systems are always as stable as possible and up to date with security patches to reduce the chances of an exploit.

# 1.2 Non-repudiation

You can't deny what you've said. It can be compared to signing a contract, your signature adds non-repudiation, and others can verify your signature.

### Proof of integrity:
Verify data does not change. The data remains accurate and consistent.

In Cryptography, we can use a hash:
- Represents data as a short string of text
- A message digest, a fingerprint
- If the data changes, the hash changes
- Doesn't necessarily associate data with an individual, it will only tell you if the data has changed

### Proof of origin:
- **Integrity**: Prove the message was not changed
- **Authentication**: Prove the source of the message
- **Non-repudiation**: Make sure the signature isn't fake

### Asymmetric Encryption:
- Sign with the private key and an associated public key.

### Creating a digital signature:
1. The sender uses their private key to encrypt (sign) a hash of the message, creating a digital signature.
2. The recipient uses the sender's public key to decrypt the digital signature. If the decrypted hash matches the hash of the received message, it verifies that the message was sent by the holder of the private key and that it has not been altered.

This method is used to ensure authenticity and integrity of the message, but not confidentiality.

# 1.2 AAA Framework: Authentication, Authorisation and Accounting

A security model used to control access to compute resources, ensure secure communication, and manage user identities.

### Identification:
This is who you claim to be, usually your username.

### Authentication:
To verify the identity of a user or system. It requires users to provide credentials to confirm their identity.
- Password login
- Biometric scanning
- Multi-factor authentication

### Authorisation:
Based on your identification and authentication, what access do you have?
- Access Control Lists (ACL)
- Role-based access controls (RBAC)
- Attribute-based access control (ABAC)

### Accounting:
To track user activities and resource usage. It involves logging and monitoring user actions to create an audit trail.
- Logging access attempts
- Tracking user actions
- Usage reports

An organisation has a trusted Certificate Authority (CA). Most organisations maintain their own CAs.

The organisation will create a certificate for a device, and it is further used as an authentication factor to verify that it really was digitally signed by the CA.

### Authorisation Models:

The user or device has now authenticated, and we need to apply an authorisation model. Associating individual users' access rights does not scale well. Using an authorisation model to define roles, organisations, attributes, and other types of characteristics is more effective.

The use of an authorisation model will help reduce complexity and create a clear relationship between the user and the resource. Instead of mapping every individual user to an abstraction (group), it is easier to allocate permissions to them all.

# 1.2 Gap Analysis

Where you are compared to where you want to be.  
The "gap" between the two.

A baseline will give you something to work towards, and an idea on where the goal should be. Also categorised as an internal set of goals.

### Compare and Contrast:
- Examine the current processes
- Research existing IT systems
- Evaluate existing security policies
- Identify weaknesses, along with the most effective processes

A detailed analysis can help examine broad security categories and break those into smaller, more manageable segments.

### The analysis report: The final comparison.
- Detailed baseline objectives
- A clear view of the current state

"How to get from where you are, to where you want to be"
![image](https://github.com/user-attachments/assets/7572ca03-6048-4740-9144-f44249b43186)

# 1.2 Zero Trust Security Model

Many networks are relatively open on the inside.

Zero Trust is a holistic approach to network security, covering every device, every process, and every user on the network.
- Never trust, always verify - Micro segmentation and least privilege access principles 
- Everything must be verified
- Nothing is inherently trusted
- Multi-factor authentication, encryption, system permissions, additional firewalls, monitoring and analytics, etc.

### Planes of operation: Split the network into functional planes
- Applies to physical, virtual, and cloud components.

### Data plane: 
The part of the device performing the security process, a switch, router, or firewall. Tools that help move data from one part of the network to another.
- Process the frames, packets, and network data
- Processing, forwarding, trunking, encrypting, NAT
![image](https://github.com/user-attachments/assets/30172513-a9c1-4362-aeb7-cac486dd2e49)


### Control plane: 
This is where we manage all of the actions occurring in the data plane.
- Define policies and rules
- Determine how packets should be forwarded
- Routing tables, session tables, NAT tables

### Adaptive Identity: 
A dynamic approach to managing user identities and access privileges within an IT environment.
- **Behavioural Analysis**: Monitoring and analysing user behaviour to detect anomalies that may indicate potential security risk.
- **Risk-Based Authentication**: Adjusting authentication requirements based on the assessed risk level, such as requiring multi-factor authentication for high-risk activities.
- **Contextual Awareness**: Considering various factors such as the user's location, device, and time of access to make real-time access decisions.
- **Continuous Monitoring**: Continuously assessing user activities to update risk profiles and dynamically adjust access controls.

### Threat Scope Reduction:
- Decrease the number of possible entry points.

### Policy-Driven Access Control:
- Combine the adaptive identity with a predefined set of rules.

### Security Zones: 
Security is more than a one-to-one relationship.

Where are you coming from and where are you going:
- Trusted, untrusted
- Internal network, external network
- VPN 1, VPN 5, VPN 11
- Marketing, IT, accounting, human resources.

Using Zones may be enough by itself to deny access:
- For example, Untrusted to Trusted zone traffic.
Some zones are implicitly trusted:
- For example, Trusted to Internal zone traffic.

### Policy Enforcement Point (PEP): 
Subjects and systems, end-users, applications, and non-human entities.
- A gatekeeper, all traffic must pass through this point to decide if the traffic is allowed through the PEP or not.
- Allow, monitor, and terminate connections.

### Applying Trust in the Planes:

### Policy Decision Point (PDP):
- There's a process for making an authentication decision.

### Policy Engine:
- Evaluates each access decision based on policy and other information sources.
- Grant, deny, or revoke access.

### Policy Administrator:
- Communicates with the policy enforcement point.
- Generates access tokens or credentials.
- Tells the PEP to allow or disallow access.
  
### Zero Trust Across Planes
![image](https://github.com/user-attachments/assets/8aac0e3d-50c0-4e1e-a5eb-98653bd7b0e2)

# 1.2 Physical Security

### Barricades / Bollards: Prevent access
- Channel people through a specific access point
- Keeps other things out
- Allow people, prevent cars and trucks
- Identify safety concerns and prevent injury
- Can be used to an extreme: concrete barriers/bollards, moats.

### Access Control Vestibules: 
A room you must pass through to gain access to the rest of the building.
- All doors are normally unlocked, opening one door causes others to lock.
- Or all doors are normally locked, unlocking one door prevents others from being unlocked.
- One door open/other locked. When one is open, the other cannot be unlocked.
- One at a time, controlled groups, managed through an area.
- They are designed to allow or control access through a particular area.

### Fencing: 
Builds a perimeter, usually very obvious.
- Transparent or opaque, see through the fence (or not)
- Robust
- Prevent climbing, razor wire or built high.

### Video Surveillance: 
CCTV, can be used to replace physical guards.
- Camera features are important, motion recognition to alarm and alert when something moves.
- Object detection can identify a license plate or person's face.
- Networked together and recorded over time.

### Guards and Access Badges:
- Physical protection at the reception area of a facility.
- Validates identification of existing employee.
- Two-person integrity/control to minimize exposure to an attack, no single person has access to a physical asset.
- Access badge to provide a picture, name, or other details, it must be worn at all times and is electronically logged.

### Lighting: 
More light means more security.
- Attackers avoid the light, Non-IR cameras can see better.
- Specialized design for better overall light, lighting angles may be important for facial recognition.

### Sensors: 
Infrared, detects infrared radiation in both light and dark areas, common in motion detectors.
- Pressure, detects a change in force, floor, and window sensors.
- Microwave detects movement across a large area.
- Ultrasonic signals receive reflected sound waves, it will detect motion and collision detection, etc.

# 1.2 Deception and Disruption

### Honeypots: Attracts the bad guys and trap them there.
- Helps you see what type of attacks are being used and what type of systems they are trying to attack.
- Virtual world that attracts automated systems/attackers.

### Honeynets: 
A real network including more than a single device.
- Servers, workstations, routers, switches, firewalls, etc.
- A larger deception network with one or more honeypots in hopes to keep attackers interested.

### Honeyfiles: 
Attract attackers with fake files/information.
- Something bright and shiny
- Bait for the honeynet (e.g., `passwords.txt`)
- Add many honeyfiles to file shares.
- An alert is sent if the file is accessed, a virtual bear trap.

### Honeytokens: 
Traceable data to track the malicious actors.
- Adds traceable data to the honeynet.
- If the data is stolen, you'll know where it came from.
- API credentials that do not actually provide access but a notification is sent to you when they're used.
- Fake email addresses, constantly monitor the internet to see who posts it.
- Honeytokens can be any type of data, database records, browser cookies, web page pixels, etc.

# 1.3 Change Management

### How to make a change: 
You need to go through a formal process to make sure the change will work properly.
- Upgrade software
- Patch an application
- Change firewall configuration
- Modify switch ports

One of the most common risks in the enterprise:
- Occurs very frequently
- A system that is less updated is probably less secure
- Often overlooked or ignored

### Have clear policies:
- Frequency, duration, installation process, rollback procedures.

Sometimes extremely difficult to implement:
- It's hard to change corporate culture.

### Change Approval Process:
A formal process for managing change to maintain the uptime and availability of our systems and ensure everyone is informed.
- Avoid downtime, confusion, and mistakes.

A typical approval process:
1. Complete the request forms
2. Determine the purpose of the change
3. Identify the scope of the change
4. Schedule a date and time for the change
5. Determine affected systems and the impact
6. Analyze the risk associated with the change
7. Get approval from the change control board
8. Get end-user acceptance after the change is complete.

### Ownership:
Involves assigning responsibility for managing and overseeing the change process to specific individuals or groups.
- Clear accountability
- Decision-making authority
- Leadership and guidance

### Stakeholders:
- Individuals or groups affected by or having an interest in the change
- Support and buy-in
- Providing input and feedback
- Managing resistance, addressing concerns early
- Maintaining communication

### Impact Analysis:
- Assess how the change will affect various aspects of the organization
- Identify risk
- Evaluating effects on business processes
- Planning resource allocation
- Setting expectations

### Determine a risk value:
- High, medium, or low.

The risks can be minor or far-reaching:
- The "fix" doesn't really fix anything
- The fix breaks something else
- Operating system failures
- Data corruption

### What's the risk with not making the change?
- Security vulnerability
- Application unavailability
- Unexpected downtime to other services

### Test results: Sandbox Testing Environment
- You can perform as many tests as you'd like and you'd have no effect on production systems.
- A technological safe space where you can make mistakes, try different techniques and perform extensive testing after the fact to see if the update worked correctly.
- Try the upgrade and apply the patch.
- Test and confirm before deployment.
- Confirm the backout plan, move everything back to the original. A sandbox can't consider every possibility.

### Backout Plan:
You should always have a way to revert your changes, prepare for the worst, hope for the best.
- Always create backups before making any changes to a system.

### Maintenance window: 
Finding time to implement a change.
- When is the change happening? 
- During the workday may not be the best option. Potential downtime would affect a large part of production.
- Overnights are often a better choice. (Especially challenging for 24-hour production schedules)
- The time of the year may be a consideration, retail networks are frozen during the holiday season.

### Standard Operating Procedure:
Change management is critical; it affects everyone in the organization.
- The process must be well documented
- Should be available on the intranet with all standard processes and procedures
- Changes to the process are reflected in the standard.


# 1.3 Technical Change Management

### Put the change management process into action: 
Execute the plan.
- There's no such thing as a simple upgrade, it can have many moving parts.
- Separate events may be required.
- Change management is often concerned with "what" needs to change.
- The technical team is concerned with "how" to change it.

### Allow/Deny list: 
Any application can be dangerous.
- Vulnerabilities
- Trojan Horses
- Malware
- Security Policy can control app execution, allow/deny list.

### Allow List:
- Nothing runs unless it's approved.
- Very restrictive.

### Deny List:
- Nothing on the "bad list" can be executed.
- Antivirus, anti-malware.

### Restricted Activities:
- The scope of a change is important, defines exactly which components are covered.
- A change approval isn't permission to make any change, the change control approval is very specific.
- The scope may need to be expanded during the change window, it's impossible to prepare for all possible outcomes.
- The change management process determines the next steps, there are processes in place to make sure the change is successful.

### Downtime:
Services will eventually be unavailable.
- The change process can be disruptive.
- Usually scheduled during non-productive hours.
- For systems working 24/7, try to prevent any downtime by switching to a secondary system, upgrade the primary, then switch back.
- Minimize any downtime events, the process should be as automated as possible, switch back to secondary system if issues appear, should be part of the backout plan.
- Send emails and calendar updates.

### Restarts: 
It's common to require a restart.
- Implement the new configuration.
- Reboot the OS, power cycle the switch, bounce the service.
- Can the system recover from a power outage?

### Legacy Applications:
Some applications were here before you arrived.
- They'll be here when you leave.
- Often no longer supported by the developer, you're not the support team.
- Fear of the unknown, face your fears and document the system. It may not be as bad as you think!
- May be quirky, create specific processes and procedures. You'll become the expert!!

### Dependencies: 
To complete A, you must complete B.
- A service will not start without other active services.
- An application requires a specific library version.
- Modifying one component may require changing or restarting other components, this can be challenging to manage.
- Dependencies may occur across systems, upgrade the firewall code first, then upgrade the firewall management software.

### Documentation: 
It can be challenging to keep up with changes.
- Documentation can become outdated very quickly.
- Required with the change management process.
- Updating diagrams, modifications to network configurations, address updates.
- Updating policies/procedures, adding new systems may require new procedures.

### Version Control: 
Track changes to a file or configuration data over time.
- Easily revert to a previous setting.
Many opportunities to manage versions, router configurations, Windows OS patches, application registry entries.


# 1.4 Public Key Infrastructure (PKI) and Cryptography

### Policies, procedures, hardware, software, people:
- Responsible for creating, distributing, managing, storing, and revoking digital certificates.
- This is a big endeavor and requires a lot of planning.
- PKI is also referred to as the binding of public keys to people or devices, the certificate authority. It's all about trust.

### Symmetric Encryption: A single, shared key
- Encrypt with the key.
- Decrypt with the same key.
- If it gets out, you'll need a new key.
- Secret key algorithm, a shared secret.
- Doesn't scale very well, challenging to distribute.
- Difficult above 10 or more members.
- Very fast to use, less overhead than asymmetric encryption, often combined with asymmetric encryption.


### Asymmetric Encryption: Two or more mathematically related keys
- Private key, kept private.
- Public key, anyone can see this key.
- The private key is the only key that can decrypt data encrypted with the public key. You can't derive the private key from the public key.

### The Key Pair: Asymmetric encryption, Public Key Cryptography
- Everyone can have the public key, only Alice has access to the private key.
![image](https://github.com/user-attachments/assets/68ce42cf-884b-4377-bb29-33a9b31ad101)


### Key Generation:
- Build both the public and private key at the same time.
- Lots of randomization.
- Large prime numbers.
- Lots and lots of maths.

### Key Escrow: Someone else holds your decryption keys
- Your private keys are in the hands of a third party.
- This may be within your own organization.
- This can be a legitimate business arrangement, a business might need access to employee information.
- Government agencies may need to decrypt partner data.
- Handing your private key to someone else may seem controversial; however, it is sometimes necessary.


# 1.4 Encrypting Data

### Encrypting stored data, protecting data on storage devices:
- SSH, hard drive, USB drive, cloud storage, etc.
- This is data at rest.

### Full-disk and partition/volume encryption:
- BitLocker, FileVault, etc.

### File Encryption:
- EFS (Encrypting File System).
- Many third-party utilities perform the same result.

### Database Encryption: Protecting stored data, and the transmission of that data:
- Transparent encryption: Encrypts all database information with a symmetric key.
- Record-level encryption: Encrypt individual columns, use separate symmetric keys for each column.
- Transport encryption: Protect data traversing the network. Browsers communicate using HTTPS.
- VPN (Virtual Private Network): Encrypts all data transmitted over the network, regardless of the application. Client-based VPN using SSL/TLS, site-to-site VPN using IPsec.

### Encryption Algorithms: There are many different ways to encrypt data, the same formula must be used during encryption and decryption:
- Both sides decide on the algorithm before encrypting data, the details are often hidden from the end-user.
- There are advantages and disadvantages between algorithms: Security level, speed, complexity of implementation.

### Cryptographic Keys: There is very little that isn't known about the cryptographic process:
- The algorithm is usually a known entity.
- The only thing you don't know is the key.
- The key determines the output, encrypted data, hash value, digital signature.
- Similar to a door lock.

### Key Lengths: Larger keys tend to be more secure:
- Prevent brute-force attacks.
- Attackers can try every possible key combination.

### Symmetric Encryption:
- 128-bit or larger symmetric keys are common.
- These numbers get larger and larger as time goes on.

### Asymmetric Encryption:
- Complex calculations of prime numbers.
- Larger keys than symmetric encryption.
- Common to see key lengths of 3072 bits or larger.

### Key Stretching: Make a weak key stronger by performing multiple processes:
- Hash a password, hash the hash of the password, and continue.
- Brute-force attacks would require reversing each of those hashes, they'd have to spend much more time to decrypt.


# 1.4 Key Exchange

### A logistical challenge: How do you share an encryption key across an insecure medium without physically transferring the key?

### Out-of-band key exchange: Don't send the symmetric key over the net:
- Telephone
- Courier
- In-person, etc.

### In-band key exchange: On the network:
- Protect the key with additional encryption.
- Use asymmetric encryption to deliver a symmetric key.

### Real-time encryption/decryption: Share a symmetric session key using asymmetric encryption:
- Client encrypts a random (symmetric) key with a server's public key.
- The server decrypts this shared key and uses it to encrypt data.
- This is the session key.

### Symmetric key from asymmetric keys:
- Use public and private key cryptography to create a symmetric key.


# 1.4 Encryption Technologies

### Trusted Platform Module (TPM)
- A specification for cryptographic functions.
- Cryptography hardware on a device.
- Cryptographic processor, random number generator, key generators.
- Persistent memory, unique keys burned in during manufacturing.
- Versatile memory, stores keys, hardware configuration information, securely stores BitLocker keys.
- Password protected, no dictionary attacks.

### Hardware Security Module (HSM)
- Securely stores thousands of cryptographic keys.
- Used in large environments.
- Clusters, redundant power.
- High-end cryptographic hardware, plug-in card or separate hardware device.
- Key backup, secure storage in hardware.
- Cryptographic accelerators, offload CPU overhead from other devices.

### Key Management System
- On-premises, cloud-based, many different keys for many different services.
- Manage all keys from a centralized manager, separate the encryption keys from the data.
- Create keys for specific services or cloud providers (SSL/TLS, SSH, etc.).
- Associate keys with specific users, rotate keys on regular intervals.
- Log key use and important events.

### Keeping Data Private
- Our data is located in many different places: mobile phones, cloud, laptops, etc.
- The most private data is often physically closest to us.
- Attackers are always finding new techniques, it's a race to stay one step ahead.
- Data is changing constantly, we need to keep the data protected.

### Secure Enclave
- A protected area for our secrets.
- Often implemented as a hardware processor.
- Isolated from the main processor.
- Many different technologies and names.
- Provides extensive security features.
- Has its own boot ROM.
- Monitors the system boot process.
- True random number generator.
- Real-time memory encryption.
- Root cryptographic keys.
- Performs AES encryption in the hardware device AND MORE.


# 1.4 Data Obfuscation

### The Process of Making Something Easy to Understand to Making It Unclear
- It's now much more difficult to understand.
- If you know how the obfuscation is done, you'll be able to gain access to the data.
- The idea is you're hiding information in plain sight. Only if you know how it's hidden, you'll recognize there's data hidden within that object.
- Hiding information inside an image is known as Steganography.

### Steganography
- Greek for "Concealed writing."
- Security through obscurity.
- The message is invisible, but it's stored within the data contained within the image.
- The covertext, the container document or file.

### Common Steganography Techniques:
- **Network-based**: Embed message in TCP packets.
- **Image-based**: Embed the message in the image itself.
- **Invisible Watermarks**: Yellow dots on printers (machine identification code).
- **Audio Steganography**: Modify the digital video file, interlace a secret message within the audio. Similar technique to image steganography.
- **Video Steganography**: A sequence of images, use image steganography on a larger scale, manage the signal-to-noise ratio, potentially transfer much more information.

### Tokenization
- Replace sensitive data with a non-sensitive placeholder.
- Example: SSH 266-12-1112 becomes 691-61-8539. We are able to match the two together behind the scenes and transfer it across the network. On the other side, it will make that switch to what the actual number might be.
- An attacker capturing the card numbers can't use them later.
- This isn't encryption or hashing, as the original data and token aren't mathematically related.
![image](https://github.com/user-attachments/assets/18a49b79-71e7-48ca-864a-f8b45fcc924d)


### Data Masking
- Data obfuscation, hide some of the original data.
- Protects PII (Personally Identifiable Information) and other sensitive data.
- May only be hidden from view, the data may still be intact in storage. Control the view based on permissions.
- Many different techniques: substituting, shuffling, encrypting, masking out, etc.

# 1.4 Hashes

### The Process That Transforms Input Data of Any Size into a Fixed-Length String of Characters
- Represent data as a short string of text.
  - A message digest.
  - Fingerprint.

### One-Way Trip
- Impossible to recover the original message from the digest.
- Used to store passwords, ensuring confidentiality.

### Verify a Downloaded Document is the Same as the Original
- Ensures **Integrity**.

### Can Be a Digital Signature
- Provides **Authentication**.
- Ensures **Non-repudiation**.
- Ensures **Integrity**.

### Collision
- Hash Functions:
  - Take an input of any size.
  - Create a fixed-size string.
  - The result is a message digest or checksum.

### The Hash Should Be Unique
- Different inputs should never create the same hash.
- If they do, it's a **collision**.
![image](https://github.com/user-attachments/assets/ed896ca3-efdd-4e4a-a64d-2fab905b7c4e)

### MD5 Has a Collision Problem
- Found in 1996.
- **Don't use MD5 for anything important**.

### Practical Hashing: Verify a Downloaded File
- Hashes may be provided on the download site.
- Compare the downloaded file hash with the posted hash value to verify integrity.

### Password Storage
- Instead of storing the password, store a **salted hash**.
- Compare hashes during the authentication process.
- **Nobody ever knows your actual password**.

### Adding Some Salt
- **Salt**: Random data added to a password when hashing.
  - Every user gets their own random salt, the salt is commonly stored with the password.
  - **Rainbow tables** won't work with salted hashes, as an additional random value is added to the original password.
  - This slows down brute-force attempts, though it doesn't completely stop reverse engineering.

### Digital Signatures
- Proves the message was not changed: **Integrity**.
- Proves the source of the message: **Authentication**.
- Ensures the signature isn't fake: **Non-repudiation**.

### Sign with the Private Key
- The message doesn't need to be encrypted.
- **Nobody else can sign this**.

### Verify with the Public Key
- Any change in the message will invalidate the signature.


# 1.4 Blockchain Technology

### A Distributed Ledger to Track Transactions
- Everyone on the blockchain network maintains the ledger.
- Records and replicates to anyone and everyone.
- Practical applications include:
  - Payment processing.
  - Digital identification.
  - Supply chain monitoring.
  - Digital voting.

### The Blockchain Process
1. **Transaction Request**: The transaction could be any digital transaction, such as transferring bitcoins, medical records, data backups, or transferring house title information.
2. **Transaction Sent to Network**: The transaction is sent to every computer (or node) in a decentralized network to be verified.
3. **Verification and Block Creation**: The verified transaction is added to a new block of data, containing other recently verified transactions.
4. **Secure Code Calculation**: A secure code (hash) is calculated from the previous blocks of transaction data in the blockchain. The hash is added to the new block of verified transactions.
5. **Block Addition**: The block is added to the end of the blockchain, and the blockchain is updated across all nodes in the network for security.

### Security of the Blockchain
- If any blocks are altered, its hash and all following hashes in the chain are automatically recalculated.
- The altered chain will no longer match the chains stored by the rest of the network and will be rejected.


# 1.4 Certificates

### Public Key Certificates
- **Binds a public key** with a digital signature and other details about the key holder.
- **A digital signature** adds trust, and Public Key Infrastructure (PKI) uses certificate authorities (CAs) for additional trust.
- **Web of Trust** adds other users for additional trust.

### Certificate Creation
- Can be built into the OS:
  - Part of Windows Domain Services.
  - Many third-party options available.

### What’s in a Digital Certificate?
- **X.509**: Standard format.
- Certificate details include:
  - Serial number.
  - Version.
  - Signature algorithm.
  - Issuer.
  - Name of certificate holder.
  - Public key.
  - Extensions.
  - And more.

### Root of Trust
- **Everything associated with IT security requires trust**, a foundational characteristic.
- How to build trust from something unknown?
  - Someone/something trustworthy provides their approval.
- The **root of trust** refers to an inherently trusted component, such as hardware, software, firmware, or another component:
  - Hardware Security Module (HSM), Secure Enclave, Certificate Authority, etc.

### How to Trust an Unknown Entity?
- **Use a trusted third party or authority**:
  - A Certificate Authority (CA) digitally signs a website certificate; trust the CA, and therefore trust the website.
  - Real-time verification ensures continued trust.

### Third-party Certificate Authorities
- Built into your browser.
- Purchase your website certificate, and it will be trusted by everyone's browser.
- CA is responsible for vetting the request and confirming the certificate owner. Additional verification may be required by the CA.

### Certificate Signing Requests
- Used for requesting certificates from a CA.
![image](https://github.com/user-attachments/assets/b6003834-6b9b-4e9d-911c-0d4c2cd450dd)

### Private Certificate Authorities
- **You are your own CA**:
  - Build it in-house.
  - Your devices must trust the internal CA.
  - Needed for medium-to-large organizations with many web servers and privacy requirements.
  - Implement as part of your overall computing strategy using solutions like Windows Certificate Services or OpenCA.

### Self-signed Certificates
- Internal certificates don’t need to be signed by a public CA.
  - Your company is the only one that needs to use it, so there’s no need to purchase trust for devices that already trust you.
  - Build your own CA, issue your own certificates signed by your internal CA.
  - Install the CA certificate/trusted chain on all devices to ensure they trust any certificates signed by your internal CA.

### Wildcard Certificates: Subject Alternative Name (SAN)
- Extension to an X.509 certificate.
- Lists additional identification information.
- Allows a certificate to support many different domains.
- Wildcard domain certificates are based on the name of the server and will apply to all server names in a domain.

### Key Revocation: Certificate Revocation List (CRL)
- Maintained by the Certificate Authority (CA).
- Can contain many revocations in a large file.
- Changes regularly, for example, due to vulnerabilities like Heartbleed (in OpenSSL).

### OSCP Stapling: Online Certificate Status Protocol
- Provides scalability for OCSP checks.
- The CA is responsible for responding to all client OCSP requests, which may not scale well.
- The certificate holder verifies their own status. Status information is stored on the certificate holder’s server.
- OCSP status is "stapled" into the SSL/TLS handshake, digitally signed by the CA.
</details>


<details>
<summary>2.0 Threats, Vulnerabilities, Mitigations</summary>

# 2.1 Threat Actors

**Definition**  
The entity responsible for an event impacting the security of another entity, also known as a malicious actor.

### Purpose
- Useful to categorize the intention or motivation behind an attack.
- Helps determine:  
  - **Why** the attack is happening  
  - **Whether** it’s directed or random  

### Attributes of Threat Actors
- **Internal/External**
- **Resource Funding**

### Level of Sophistication/Capability
- Could range from running scripts blindly to creating custom malware and scripts.

### Motivation
- Determines the purpose behind an attack, which could include:  
  - Data exfiltration, espionage, service disruption, blackmail, financial gain, etc.

---

### Examples of Threat Actor Groups

| Threat Actor      | Location | Resources      | Sophistication | Possible Motivations                          |
|-------------------|----------|----------------|----------------|-----------------------------------------------|
| Nation State      | External | Extensive      | Very High      | Data exfiltration, philosophical, revenge, disruption, war |
| Unskilled         | External | Limited        | Very Low       | Disruption, data exfiltration, philosophical beliefs |
| Hacktivist        | External | Some funding   | Can be high    | Philosophical beliefs, revenge, disruption/chaos |
| Insider Threat    | Internal | Many Resources | Medium         | Revenge, financial gain                       |
| Organised Crime   | External | Often extensive| Very high      | Financial                                     |
| Shadow IT         | Internal | Many resources | Limited        | Philosophical beliefs, revenge                |

---

## Detailed Descriptions of Threat Actor Groups

### Nation States
- **Characteristics**: Highly sophisticated, commonly known as advanced persistent threats (APTs).
- **Motivations**: Data exfiltration, philosophical beliefs, revenge, disruption, warfare.
- **Capabilities**: Military-level control, attacks on utilities and financial sectors.
  
### Unskilled Attackers
- **Characteristics**: Often run pre-made scripts without a deep understanding of them.
- **Motivations**: Disruption, data exfiltration, and personal challenge.
- **Capabilities**: Limited, may be internal or external actors.

### Hacktivists
- **Characteristics**: Hackers with a specific purpose, usually motivated by ideology.
- **Motivations**: Philosophical beliefs, revenge, disruption/chaos.
- **Capabilities**: Range from limited to sophisticated, involving DoS, defacement, document leaks.

### Insider Threats
- **Characteristics**: Internal employees with access to sensitive information.
- **Motivations**: Revenge, financial gain.
- **Capabilities**: Access to internal resources makes them a significant threat.

### Organised Crime
- **Characteristics**: Professional criminal organizations, highly organized.
- **Motivations**: Financial profit.
- **Capabilities**: High sophistication, access to advanced hacking tools and infrastructure.

### Shadow IT
- **Characteristics**: Internal staff circumventing official IT processes, building unsanctioned infrastructure.
- **Motivations**: Work flexibility, philosophical beliefs, or dissatisfaction with IT.
- **Capabilities**: Often limited resources but may use cloud services to bypass restrictions.

# 2.2 Common Threat Vectors

**Definition**  
A method used by an attacker to gain access to or infect a target. Also called an attack vector.

- **Purpose**: Threat actors put significant effort into finding vulnerabilities.
- **Focus**: IT security professionals continuously monitor these vectors to protect against existing threats and to identify new ones before attackers do.

---

### Types of Threat Vectors

### Message-Based Vectors
- **Overview**: A major vector, often through phishing.
- **Methods**:
  - **Email**: Malicious links, phishing sites.
  - **SMS (Smishing)**: Phishing attacks via text messages.

### Phishing Attacks
- **Common Forms**: Links in emails, texts, or IMs.
- **Intent**: Often to deliver malware or engage in social engineering scams like invoice or cryptocurrency scams.

### Image-Based Vectors
- **Difficulty**: Harder to identify threats embedded in images.
- **Methods**:
  - **SVG Files**: Can contain HTML injections or JavaScript.
  - **XSS (Cross-Site Scripting)**: Injects malicious scripts into trusted applications.

### File-Based Vectors
- **Overview**: Malicious code hidden in files.
- **File Types**: PDF, ZIP/RAR, and other compressed formats.

### Voice Call Vectors (Vishing)
- **Methods**:
  - **Spam over IP**: High-volume automated calls.
  - **War Dialing**: Attempting to connect to multiple phone numbers.
  - **Call Tampering**: Disrupting voice calls, often as a form of DoS.

### Removable Device Vectors
- **Device Types**: USB flash drives, among others.
- **Risks**:
  - **Air-gapped Networks**: Can introduce malware even in isolated systems.
  - **Data Exfiltration**: Massive data extraction with zero network bandwidth.

### Vulnerable Software Vectors
- **Overview**: Security flaws in software require frequent updates.
- **Categories**:
  - **Client-Based**: Vulnerabilities in user-installed applications.
  - **Agentless**: Compromised server software affecting all clients.

### Unsupported Systems Vector
- **Risk**: Unpatched, outdated systems pose significant vulnerabilities.
- **Solution**: Maintain an inventory and ensure all systems are up-to-date.

### Unsecure Network Vectors
- **Types**:
  - **Wireless**: Outdated protocols (e.g., WEP, WPA), unsecured networks.
  - **Wired**: Lack of security measures like 802.1X.
  - **Bluetooth**: Vulnerable to reconnaissance and exploitation.

### Open Service Ports
- **Risk**: Open TCP/UDP ports increase attack surface.
- **Challenge**: Each open port presents a potential entry point.

### Default Credentials
- **Issue**: Default usernames and passwords can provide attackers with administrator access.

### Supply Chain Vectors
- **Methods**:
  - **Tampering**: Malicious alterations in manufacturing or infrastructure.
  - **Compromised Equipment**: Counterfeit or vulnerable hardware, as seen in notable breaches like the 2013 Target credit card breach and counterfeit Cisco switches in 2020.

# 2.2 Phishing

**Definition**  
Phishing is a form of social engineering and scam where attackers trick individuals into revealing sensitive information or installing malware. Common targets include usernames, passwords, credit card details, and more.

---

### Signs of a Phishing Email
- **URL Checks**: Look for inconsistencies or slight variations.
- **Visual Cues**: Odd fonts, unusual spacing, or other irregularities.
- **Overall Feel**: Often something will seem "off."

---

### Techniques Used in Phishing

- **Digital Sleight of Hand**: Using tactics to obscure or misdirect attention.
- **Typosquatting**: Creating fake URLs that resemble legitimate ones (URL hijacking).
- **Pretexting**: Fabricating a believable story to gain trust and information.
- **Character Play**: The attacker pretends to be someone trustworthy in a fabricated situation.

---

### Types of Phishing

### Vishing
- **Definition**: Voice phishing conducted over the phone or voicemail.
- **Common Tactics**:
  - **Caller ID Spoofing**: Making the call appear from a trusted source.
  - **Fake Security Checks**: Posing as bank or tech support representatives.

### Smishing
- **Definition**: SMS phishing done via text message.
- **Common Tactics**:
  - **Spoofed Sender ID**: Messages appear to be from a trusted source.
  - **Link Forwarding**: Requests to click links or provide personal details.

### Phishing with Different Bait
- **Definition**: Combines phishing with other social engineering tactics.
- **Goal**: Broaden the approach to increase the chances of success.

# 2.2 Impersonation

**Definition**  
Impersonation occurs when an attacker pretends to be someone they are not in order to trick individuals into revealing personal information.

---

### Tactics in Impersonation

### Eliciting Information
- **Technique**: Extracting information from a target without them realizing it.
- **Common Scenarios**: Often used in vishing, where attackers find it easier to extract information over the phone.
- **Psychology**: Relies on well-documented psychological techniques to manipulate the victim.

### Identity Fraud
- **Definition**: Using someone else’s identity for malicious purposes.
- **Common Examples**:
  - **Credit Card Fraud**: Attacker makes purchases with your credit card or opens a new one.
  - **Bank Fraud**: Attacker gains access to your account or opens a new account in your name.
  - **Loan Fraud**: Taking out loans using your identity.
  - **Government Benefits Fraud**: Claiming benefits or entitlements under your name.

---

### How to Protect Against Impersonation

- **Avoid Volunteering Information**: Do not share unnecessary personal details.
- **Protect Sensitive Details**: Refrain from disclosing personal information, such as your birthday, SSN, address, etc.
- **Always Verify**: Before revealing sensitive information, verify the identity of the requester.
- **Encourage Verification**: Especially important in organizations that handle valuable information. Implement a call-back process or verify through trusted third parties.

# 2.2 Watering Hole Attack

**Definition**  
A watering hole attack is a cyberattack strategy that targets specific groups of users by infecting websites that they frequently visit. This tactic enables attackers to spread malware to all visitors of the compromised site.

---

### Steps in a Watering Hole Attack

1. **Identify Targeted Websites**  
   - Attackers research and determine websites that the targeted group frequently uses.
   - Examples:
     - Common local sites (e.g., coffee shops, sandwich shops)
     - Industry-related websites and forums

2. **Infect the Site**  
   - The attacker finds vulnerabilities in the chosen website and exploits them to inject malicious code.
   - Infection methods may include:
     - Exploiting website vulnerabilities
     - Using infected email attachments sent to the site’s administrators or users

3. **Impact on All Visitors**  
   - Once infected, the site spreads malware to all its visitors, effectively compromising multiple users within the targeted group.

---

### Mitigating Watering Hole Attacks

While there is no foolproof method to prevent a watering hole attack, the following strategies can help mitigate its impact:

- **Defense-in-Depth (Layered Defense)**: Implement multiple security layers to increase resistance against various attack vectors.
- **Firewall and Intrusion Prevention Systems (IPS)**: Block malicious network traffic before it reaches the internal network.
- **Anti-Virus / Anti-Malware**: Regularly update signature definitions to detect and prevent known threats.

# 2.2 Other Social Engineering Attacks

### Misinformation/Disinformation

- **Misinformation**: False or inaccurate information spread unintentionally, often due to lack of verification. This can mislead individuals or groups without malicious intent.
- **Disinformation**: Deliberately false information intended to deceive. Often used in targeted campaigns to manipulate opinions, beliefs, or actions.

Both misinformation and disinformation can influence decision-making, especially when propagated through social media or other trusted communication channels.

---

### Brand Impersonation

- **Definition**: A tactic where attackers pretend to represent a well-known brand, often to build trust and extract sensitive information from victims.
- **Common Examples**:
  - Fake customer support messages from well-known companies
  - Phishing emails designed to look like official brand communications

Brand impersonation can lead to various attacks, including phishing, malware distribution, and financial scams, by exploiting a brand's established reputation and user trust.

--- 

### Protection Against These Attacks

1. **Verify Information Sources**: Check the credibility of sources, especially with sensitive or influential information.
2. **Examine URLs and Email Domains**: Many brand impersonation attempts use similar but slightly altered domain names.
3. **Report Suspicious Content**: Notify relevant authorities or organizations if you encounter potential misinformation, disinformation, or brand impersonation.

# 2.3 Memory Injection

Memory injection is a technique used by attackers to insert malicious code directly into the memory of a legitimate process, allowing malware to run without creating separate, easily detectable processes.

### Key Concepts

- **Memory as Software**: The software on a computer, including malware, is loaded and runs in memory.
- **Memory Forensics**: Analyzing memory can uncover malicious code embedded in active processes.

---

### Memory Components

Memory contains various elements that malware may exploit:
  - **DLLs (Dynamic Link Libraries)**: Shared code libraries used by multiple applications.
  - **Threads**: Units of execution within processes.
  - **Buffers**: Temporary storage for data being processed.
  - **Management Functions**: Control and manage resources within applications.

---

### Malware Injection Techniques

- **Malware Process**: Malware may run as a standalone process or attach itself to a legitimate one.
- **Process Injection**: Malware is inserted into the memory of an existing, legitimate process, making it harder to detect.

---

### DLL Injection

- **What Is DLL Injection?**: A common method of memory injection in Windows environments, where attackers load a malicious DLL into the memory space of a legitimate application.
- **How It Works**: By injecting a path to a malicious DLL, attackers can execute code within the target process, often evading detection by security software.

Memory injection techniques like DLL injection allow attackers to conceal malware within trusted applications, enabling covert and persistent attacks.

![image](https://github.com/user-attachments/assets/fd7d2aad-1886-4290-bb5b-37587965b4a0)

# 2.3 Buffer Overflows

Buffer overflow is an attack where more data is written to a buffer—a temporary data storage area in memory—than it can hold. This excess data "overflows" into adjacent memory locations, potentially corrupting or overwriting critical data.

### How Buffer Overflows Work

- **Overflow Mechanism**: When a buffer receives more data than it is allocated, the overflow spills into adjacent memory spaces.
- **Memory Corruption**: This can disrupt or overwrite data, causing unexpected behavior in the application.

---

### Exploitation and Impact

Attackers can use buffer overflow vulnerabilities to manipulate a program’s execution, often with severe outcomes:
  - **Crashes**: Force the program to crash, resulting in a denial of service.
  - **Unauthorized Access**: Alter the program’s execution flow to gain unauthorized access to sensitive areas.
  - **Execution of Malicious Code**: Inject and execute malicious code, often allowing the attacker to take control of the system.

Buffer overflows are a critical security concern, especially in applications that handle large volumes of input data, as they can enable attackers to compromise system integrity and security.

# 2.3 Race Conditions

A race condition occurs when a system or device tries to perform two or more operations simultaneously, but the correct execution depends on these operations happening in a specific sequence. Race conditions can lead to unexpected behavior and security vulnerabilities if the sequence is disrupted.

### Time-of-Check to Time-of-Use (TOCTOU) Attack

One common example of a race condition vulnerability is the **TOCTOU (Time-of-Check to Time-of-Use)** attack, where an attacker manipulates the time gap between checking a resource and using it.

### How TOCTOU Works:
  - **Check**: The system performs a check on a resource or condition.
  - **Use**: The system then proceeds based on the results of that check.
  - **Attack Window**: An attacker exploits the time gap between these steps, modifying the resource or condition after the check but before its use.

### Potential Impacts
Race conditions, and especially TOCTOU attacks, can lead to unauthorized actions, such as:
  - **Escalation of Privileges**: Gaining access to higher privileges by altering permissions during the gap.
  - **Data Corruption**: Changing critical data, causing system instability or incorrect results.
  - **Access Control Bypass**: Bypassing access controls by exploiting timing gaps.

Mitigating race conditions typically involves implementing synchronization controls and ensuring atomic operations where sequence consistency is essential.

![image](https://github.com/user-attachments/assets/ceee7f0f-c251-4f18-ad24-f8037df43cb9)

# 2.3 Malicious Updates

While software updates are essential for maintaining security, they can also introduce vulnerabilities if compromised. Malicious actors may exploit updates to distribute malware or unauthorized changes. It is essential to follow best practices to minimize these risks.

### Importance of Software Updates
- **Security Patches**: Updates often contain bug fixes and patches for known security vulnerabilities.
- **System Stability**: Updates can improve performance and functionality, but security remains a primary benefit.

### Best Practices for Safe Updating
- **Have a Known-Good Backup**: Always keep a recent backup of critical files before updating in case the update is compromised.
- **Install from Trusted Sources**: Only download updates from official and trusted sources. Avoid updates prompted by random pop-ups during web browsing.

### Downloading and Updating Software
- **Use Caution with Downloads**: Every installation file could be a potential risk. Confirm the legitimacy of the source.
- **Direct Downloads Only**: Visit the official developer's website rather than relying on third-party links.
- **Check for Digital Signatures**: Many operating systems only allow apps with valid digital signatures. Do not disable security settings that prevent unsigned apps from running.

### Automatic Updates
- **Automatic Security Checks**: Automatic updates typically include security checks, such as verifying digital signatures.
- **Developer Trustworthiness**: Updates delivered directly from developers are more reliable, though not immune to risks.

### Example: SolarWinds "Orion" Supply Chain Attack
In one notable incident, attackers compromised the SolarWinds development environment and injected malicious code into updates for their Orion software. This breach gave attackers access to hundreds of organizations, including government agencies and private companies, illustrating the potential risks associated with malicious updates.

# 2.3 Operating System Vulnerabilities

Operating systems (OS) are foundational platforms for all computing, making them prime targets for attackers. Given their complexity and widespread use, vulnerabilities in OS software pose significant security risks.

### Why OS Vulnerabilities Matter
- **Complexity**: Operating systems are built with millions of lines of code, and the larger the codebase, the greater the potential for vulnerabilities.
- **Known Vulnerabilities**: Some security issues are inherent within the OS and remain undiscovered until they are exploited.
- **Wide Reach**: Since almost everyone uses an OS, vulnerabilities can affect vast numbers of users and organizations.

### Example of OS Vulnerability Patch: Microsoft
- **Windows Update Cycle**: Microsoft releases patches on the second Tuesday of each month (Patch Tuesday).
- **Security Patches**: For example, on May 9, 2023, Microsoft issued nearly 50 security patches, addressing vulnerabilities such as:
  - **Elevation of Privilege**: Attackers gaining higher system privileges.
  - **Security Feature Bypass**: Exploiting weaknesses in security features.
  - **Remote Code Execution**: Allowing attackers to run malicious code remotely.

### Best Practices for Mitigating OS Vulnerabilities
- **Regular Updates**: Keep your OS up-to-date with monthly patches or as needed to address security flaws.
  - **Testing**: Some patches may require testing to ensure compatibility, as they could interfere with system functionality.
  - **Rebooting**: Be prepared to restart the system after applying patches. Always save your data before updating.
  - **Backout Plan**: Maintain a backup and have a contingency plan in case a patch causes issues.

By adhering to these best practices, you can reduce the risk posed by OS vulnerabilities and ensure that your system remains secure against potential exploits.

# 2.3 SQL Injection

SQL Injection is a type of **code injection** attack where an attacker manipulates an application's SQL query to execute malicious SQL code on a database. This is typically enabled by improper input validation or failure to sanitize user inputs in the application code.

### What is Code Injection?
Code injection occurs when a computer program is tricked into misinterpreting external input as part of its code. This vulnerability often arises from **bad programming practices**, where input/output is not handled securely. Examples of code injection include:
- **HTML Injection**
- **SQL Injection**
- **XML Injection**
- **LDAP Injection**

### What is SQL Injection?
SQL Injection exploits vulnerabilities in applications that interact with databases using SQL (Structured Query Language). If the application fails to properly validate or sanitize user inputs, an attacker can inject malicious SQL queries, potentially gaining unauthorized access to the database.

# 2.3 Cross-site Scripting (XSS)

**Cross-site Scripting (XSS)** is a vulnerability that allows attackers to inject malicious scripts into web pages viewed by other users. Originally referred to as "cross-site scripting" because of browser security flaws, XSS takes advantage of the trust a user has for a particular site, enabling attackers to execute malicious actions within the user's session.

### Types of XSS Attacks

### Non-persistent (Reflected) XSS Attack
- In a reflected XSS attack, the website allows scripts to run in user inputs, such as search boxes or form fields.
- The attacker sends a malicious link to the victim, which, when clicked, runs a script that can send the victim's credentials, session IDs, or cookies to the attacker.
- The script is embedded in the URL and executes in the victim's browser, often without the victim knowing.
  
### Persistent (Stored) XSS Attack
- In a persistent XSS attack, the attacker posts a message containing a malicious payload to a website, such as a social network.
- This attack is "persistent" because it affects anyone who visits the page with the malicious payload.
- The malicious script can propagate rapidly, especially on social networks, as the payload gets shared when users interact with the message.

### How XSS Works
XSS attacks rely on web applications that allow users to inject unfiltered content into pages, often through input fields like search boxes, forms, or message boards. If the website does not properly sanitize or escape these inputs, the attacker can execute JavaScript code in the victim’s browser.

### Protection Against XSS
To mitigate the risks of XSS attacks:
- **Be cautious when clicking untrusted links**, especially from emails or suspicious sources.
- **Disable or limit JavaScript**: Some browsers or extensions allow users to block or restrict JavaScript, reducing the risk.
- **Keep your browser and applications updated**: Regular updates help close known vulnerabilities that could be exploited by XSS attacks.
- **Input Validation**: Always validate and sanitize user inputs, especially those that are rendered in web pages (e.g., search boxes, comment sections) to prevent the execution of unauthorized scripts.

# 2.3 Hardware Vulnerabilities

Hardware vulnerabilities refer to inherent weaknesses in the architecture of hardware devices. Many of these devices do not even have an accessible operating system, making them a potential security risk. These vulnerabilities provide a perfect entry point for attacks, and as more devices become interconnected, such as light bulbs, garage doors, refrigerators, and door locks, the security landscape continues to expand with the proliferation of IoT devices.

### Key Concepts

### Firmware
- Firmware is the software that resides inside hardware devices, often referred to as the operating system of the device.
- Vendors are typically the only ones who can fix hardware vulnerabilities, provided they are aware of the issue.

### End-of-Life (EOL)
- **End-of-life (EOL)** refers to when a manufacturer stops selling a product.
- Even after EOL, the manufacturer may continue supporting the product for a period.
- **End-of-service life (EOSL)** occurs when the manufacturer stops selling a product, and support is no longer available.
- No security patches or updates are issued once EOSL is reached, which increases the security risks associated with using that device.
- Some manufacturers may offer a premium support option, but ongoing security updates are not guaranteed.

### End-of-Service Life (EOSL) Concerns
- **EOSL** is a significant security concern, especially for legacy platforms. Without continued support or security patches, devices become vulnerable to new exploits.
- Manufacturers typically release security patches as part of normal operations, but this ends once the device reaches EOSL.

### Legacy Platforms
- A legacy platform is a device running an older operating system, outdated applications, or old middleware without current updates.
- These devices may be at risk due to their use of outdated systems, often at EOL or EOSL.
- Devices running legacy platforms require additional security protections, such as more stringent firewall rules and updated intrusion prevention signatures, to mitigate the risks associated with outdated software.

# 2.3 Virtualization Vulnerabilities

Virtualization vulnerabilities share similarities with physical machine vulnerabilities, but they introduce unique risks due to the nature of virtual environments. These vulnerabilities can include issues like local privilege escalations, command injection, and others specific to virtualized systems.

### Key Concepts

### Virtual Machine Escape Protection
- **Virtual machine escape** occurs when an attacker breaks out of the virtual machine (VM) and interacts with the host operating system or hardware.
- If an attacker successfully escapes the VM, they gain significant control over the host system, which represents a huge security exploit.
- Protecting against VM escape is critical to maintaining the security of both the virtual and host environments.

### Resource Reuse
- The **hypervisor** manages the relationship between the physical and virtual resources, such as available RAM, storage space, and CPU availability.
- However, resources can be inadvertently shared between virtual machines (VMs), which may lead to security risks.
- For example, data from one VM could accidentally be accessed or shared with another, creating opportunities for attacks if not properly managed.

# 2.3 Cloud-Specific Vulnerabilities

Security in the cloud presents unique challenges, with vulnerabilities that can impact both cloud infrastructure and the applications running within it. These vulnerabilities can expose sensitive data or allow attackers to exploit various weaknesses.

### Key Cloud Vulnerabilities

- **Directory Traversal**: Attacks where an attacker gains unauthorized access to restricted directories by manipulating file paths.
- **Remote Code Execution (RCE)**: Allows an attacker to execute arbitrary code on a server, often exploiting a vulnerability in a web application.
- **Denial of Service (DoS)**: An attack that overwhelms cloud services, rendering them unavailable to legitimate users.
- **Authentication Bypass**: Exploiting weaknesses in authentication mechanisms to gain unauthorized access to cloud systems.
- **Web Application Attacks**: Such as **Log4j** and **Spring Cloud Function**, which can be exploited to execute arbitrary code or expose sensitive data.
- **Cross-Site Scripting (XSS)**: Attacks where attackers inject malicious scripts into web pages, often exploiting poor input validation in cloud applications.
- **Out of Bounds Write**: Attacks where data is written to unauthorized memory areas, potentially corrupting data or causing code execution.
- **Data Corruption**: Attacks that cause data to become corrupted, leading to issues such as crashes or unauthorized code execution.
- **SQL Injection**: Exploiting vulnerabilities in database-driven applications to gain direct access to cloud databases and manipulate or steal data.

# 2.3 Misconfiguration Vulnerabilities

Misconfigurations are one of the most common and dangerous vulnerabilities, often stemming from human error or a lack of proper security controls. These misconfigurations can leave systems exposed to attackers, who may exploit them to gain unauthorized access or cause damage.

### Key Misconfiguration Vulnerabilities

- **Open Permissions**: Attackers use open permissions as a method of reconnaissance to find exposed data.
    - Hackers often discover boxes with open permissions, particularly in cloud storage.
    - Example: In June 2017, 14 million Verizon records were exposed because a third party left an Amazon S3 data repository open.

- **Unsecured Admin Accounts**: The Linux root account or Windows administrator account (also known as "superuser" accounts) can be targeted if left unsecured.
    - Prevent this by disabling direct login to the root account and protecting accounts with root or administrator access.

- **Insecure Protocols**: Protocols such as Telnet, FTP, SMTP, HTTP, and IMAP send all traffic in plaintext, making it easy for attackers to intercept.
    - Verify with packet captures to view unencrypted traffic.
    - Use encrypted versions like SSH, SFTP, and IMAPS to secure communication.

- **Default Settings**: Every application and network device comes with default login credentials, which can be exploited if not changed.
    - The **Mirai botnet** is an example, taking advantage of default configurations on IoT devices, such as cameras, routers, doorbells, and garage door openers.
    - Mirai was released as open-source software and targets over 60 default configurations.

- **Open Ports and Services**: Services often open ports for network communication, but these ports should be tightly controlled.
    - Limit the number of open ports and manage them using firewalls that control traffic flow, either allowing or denying access based on port number or application.
    - Firewall configurations can become complex, so periodic audits should be scheduled to verify open ports and manage access properly.

# 2.3 Mobile Device Security

Mobile devices are inherently challenging to secure due to their openness and the need for additional security policies and systems to protect sensitive data. The following issues are particularly significant in maintaining the security of mobile devices.

### Key Mobile Device Security Issues

- **Jailbreaking/Rooting**: 
    - Jailbreaking (iOS) and rooting (Android) refer to the process of bypassing the restrictions on the operating system.
    - These actions give users root access to the device, allowing them to install custom firmware and gain uncontrolled access, which circumvents built-in security features.
    - Mobile Device Management (MDM) systems become ineffective on jailbroken or rooted devices, as security controls can be bypassed.

- **Sideloading**: 
    - Sideloading is the process of installing applications from third-party sources instead of official app stores like Google Play or the Apple App Store.
    - Apps from unofficial sources may contain malware, spyware, or viruses since they haven't undergone the security checks of official stores.
    - Sideloaded apps often request excessive permissions and access to personal data, increasing the risk of data breaches or unauthorized actions.
    - Insecure updates to sideloaded apps can expose the device to security vulnerabilities.
    - Sideloading also bypasses security policies, making it easier for unapproved software to run on the device.

# 2.3 Zero-day Vulnerability

A **zero-day vulnerability** is a security flaw in software, hardware, or firmware that is unknown to the vendor or the public. The term "zero-day" refers to the fact that the developers have had zero days to address and mitigate the vulnerability.

### Key Characteristics of Zero-day Vulnerabilities:
- **Exploitation**: Attackers search for unknown vulnerabilities and create exploits that take advantage of them.
- **Unknown to Vendor**: The vendor is unaware of the flaw, meaning no patch or fix is available to prevent exploitation.
- **Zero-day attack**: A zero-day attack occurs when the vulnerability is exploited before the vendor can release a patch or mitigation method. It becomes a race to either exploit the vulnerability or develop a patch.

### Challenges:
- **Difficult to Defend**: Since the vulnerability is unknown, defending against it is extremely difficult until a patch is created or workarounds are implemented.

[Common Vulnerabilities Exposure (CVE) website](http://cve.mitre.org).

# 2.4 An Overview of Malware

Malware (malicious software) refers to any software intentionally designed to cause damage to a computer, server, client, or computer network. It encompasses a variety of malicious programs, including viruses, worms, trojans, ransomware, spyware, adware, and rootkits. Malware can steal, encrypt, or delete data, among other harmful activities.

### Types of Malware and Their Impact:
- **Information Gathering**: Malware may gather sensitive information such as keystrokes (keyloggers).
- **Advertising**: Some malware shows unwanted advertisements.
- **Data Manipulation**: Malware can encrypt or delete your data.

### How Malware Spreads:
For malware to infect your computer, it must run a program. Common methods of malware distribution include:
- **Email links**: Clicking on malicious email attachments or links.
- **Webpage popups**: Malicious popups on compromised websites.
- **Drive-by downloads**: Automatically downloading malware from a website without user interaction.
- **Worms**: Self-replicating malware that spreads across networks.

### Why Data is Targeted:
Data is often the target of malware because it holds value. Examples include:
- **Personal data**: Family pictures, videos, and important documents.
- **Organizational data**: Planning documents, employee personal information (PII), financial information, etc.

### Ransomware:
Ransomware is a type of malware that encrypts all your data, demanding payment for the decryption key.
- **Encryption**: It encrypts files like documents, images, and more.
- **OS Availability**: The operating system remains functional, but files are inaccessible.
- **Payment Demand**: Attackers request payment (usually through untraceable methods like cryptocurrency) for the decryption key.
- **Public-key Cryptography**: The unfortunate use of encryption that makes it difficult to trace the attackers.

### Protecting Against Ransomware:
To protect yourself from ransomware:
- **Backup**: Always have a backup of your data, ideally on an offline server.
- **Update OS**: Keep your operating system up to date to patch vulnerabilities.
- **Update Applications**: Ensure that applications, including antivirus and anti-malware signatures, are always up to date.

# 2.4 Viruses and Worms

### Viruses:
A **virus** is a type of malware that is able to replicate itself from one computer to another. It often requires a human to execute a program for the virus to spread.
- **Replication**: Viruses reproduce through file systems or over the network.
- **Impact**: Some viruses may cause harm, while others can be invisible, operating without noticeable symptoms.
- **Prevalence**: Thousands of new viruses are created every week. Keeping your antivirus signature file updated is crucial to identifying reported viruses.

### Types of Viruses:
- **Program Virus**: Attaches itself to executable files and spreads when the program is run.
- **Boot Sector Virus**: Infects the boot sector of a computer, making it active when the system starts.
- **Script Virus**: Uses scripts (e.g., JavaScript, VBS) to exploit vulnerabilities in software.
- **Macro Virus**: Targets macros within documents, particularly in programs like Microsoft Word or Excel.
- **Fileless Virus**: Operates in memory without installing a file or application, making detection more difficult.

### Worms:
A **worm** is a type of malware that self-replicates and uses the network as a transmission medium. It self-propagates, spreading quickly across systems without requiring user interaction.
- **Rapid Spread**: Worms can take over many systems in a short period.
- **Mitigation**: Firewalls and Intrusion Detection Systems (IDS) or Intrusion Prevention Systems (IPS) can mitigate worm infestations, but they offer little protection once the worm is inside the network.

### Example:
- **Wannacry Worm**: The Wannacry worm exploited vulnerabilities in Windows systems, allowing it to automatically propagate and install ransomware, locking users out of their systems.

# 2.4 Spyware and Bloatware

### Spyware:
**Spyware** is a type of malware designed to spy on your activities without your knowledge or consent.
- **Common Uses**: It is often used for advertising, identity theft, or affiliate fraud.
- **How It Works**: Spyware can trick you into installing software, monitor your web browsing, and even capture keystrokes using keyloggers.

### Bloatware:
**Bloatware** refers to unnecessary software that comes pre-installed on new computers or phones.
- **Impact**:
  - Takes up valuable storage space.
  - May increase overall resource usage, such as CPU or RAM, slowing down the system.
  - Could make the system more vulnerable to exploits or attacks.
  
### Removing Bloatware:
To remove bloatware:
- **Built-in Uninstaller**: Use the system’s default uninstaller to remove unwanted software.
- **Third-party Tools**: If the built-in uninstaller isn't sufficient, third-party uninstallers or cleaner tools may be needed. Always ensure you have a backup before proceeding with these tools.

# 2.4 Other Malware Types

### Keyloggers:
A **keylogger** is malware that tracks and records every keystroke made on a computer or mobile device.
- **Legitimate Use**: It can be used for monitoring employee activity or troubleshooting.
- **Malicious Use**: Keyloggers can steal sensitive information like passwords, credit card numbers, personal messages, etc.
- **Bypasses Encryption**: Even when encryption is used, keystrokes are captured in cleartext.
- **Other Logging**: Some keyloggers also record clipboard data, screen activity, instant messaging, and search queries.

### Logic Bomb:
A **logic bomb** is a type of malware that remains dormant until triggered by a specific event or condition.
- **Types**:
  - **Time Bomb**: Set to trigger at a specific date or time.
  - **User Event Bomb**: Triggered by a specific user action, such as logging in.
- **Challenges**:
  - Hard to identify because they’re designed to be triggered only under specific conditions.
  - Difficult to recover from once activated.
- **Prevention**:
  - Hard to recognize as each one is unique.
  - **Monitoring**: Electronic monitoring and alerts on system changes can help.
  - **Auditing**: Regular audits can help detect any irregularities before they trigger.

### Rootkit:
A **rootkit** is a malicious software designed to hide its presence and gain unauthorized access to a computer or network.
- **Function**: It typically hides deep within the operating system’s kernel, making it difficult to detect.
- **Detection and Removal**:
  - **Anti-malware Scans**: Can help find and remove rootkits, though specialized tools may be needed.
  - **Rootkit-specific Removers**: Developed after the discovery of the rootkit.
  - **Secure Boot**: Use **UEFI** and **BIOS security** features like **SecureBoot** to check the operating system’s signature, preventing unauthorized changes to the kernel.

# 2.4 Physical Attacks

### Brute-force:
A **brute-force** physical attack involves forcing access to a locked area.
- **Considerations**:
  - Ensure that physical security measures are in place to protect sensitive areas.
  - Check the security of windows and doors, as attackers may attempt to exploit these.
  - Attackers may use various methods to gain access, so it's essential to have strong physical security protocols.

### RFID Cloning:
**RFID cloning** involves duplicating access badges, key fobs, or other RFID-based devices.
- **Cloning Tools**: Devices to clone RFID cards are available for as little as $50 online, and the cloning process takes only seconds.
  - Attackers can easily duplicate a card by reading one and copying it to another.
- **Prevention**:
  - Use **Multi-factor Authentication (MFA)** to add an additional layer of security. Even if an RFID badge is cloned, MFA requires a second form of verification, which helps to block unauthorized access.

### Environmental Attacks:
**Environmental attacks** target the physical infrastructure supporting technology systems.
- **Common Attacks**:
  - **Power Disruption**: Shutting off power to the building can cripple systems.
  - **HVAC and Humidity Control**: Manipulating the building’s HVAC or humidity controls can damage hardware.
  - **Fire Suppression**: Disrupting or sabotaging fire suppression systems could damage critical infrastructure.

# 2.4 Physical Attacks

### Brute-force:
A **brute-force** physical attack involves forcing access to a locked area.
- **Considerations**:
  - Ensure that physical security measures are in place to protect sensitive areas.
  - Check the security of windows and doors, as attackers may attempt to exploit these.
  - Attackers may use various methods to gain access, so it's essential to have strong physical security protocols.

### RFID Cloning:
**RFID cloning** involves duplicating access badges, key fobs, or other RFID-based devices.
- **Cloning Tools**: Devices to clone RFID cards are available for as little as $50 online, and the cloning process takes only seconds.
  - Attackers can easily duplicate a card by reading one and copying it to another.
- **Prevention**:
  - Use **Multi-factor Authentication (MFA)** to add an additional layer of security. Even if an RFID badge is cloned, MFA requires a second form of verification, which helps to block unauthorized access.

### Environmental Attacks:
**Environmental attacks** target the physical infrastructure supporting technology systems.
- **Common Attacks**:
  - **Power Disruption**: Shutting off power to the building can cripple systems.
  - **HVAC and Humidity Control**: Manipulating the building’s HVAC or humidity controls can damage hardware.
  - **Fire Suppression**: Disrupting or sabotaging fire suppression systems could damage critical infrastructure.

# 2.4 Denial of Service (DoS)

### Denial of Service (DoS):
A **Denial of Service (DoS)** attack occurs when an attacker causes a service to fail by overwhelming it with excessive inputs, preventing legitimate users from accessing the service.
- **Key Characteristics**:
  - The attacker forces a service to fail or overloads it with requests.
  - Exploits design failures or vulnerabilities in the service.
  - Keeping systems patched can help mitigate some DoS attacks.
  - The attack results in the service being unavailable, causing disruptions.
  - DoS attacks can serve as precursors to other attacks, such as **DNS spoofing**.

### "Friendly" DoS:
A **"friendly" DoS** is an unintentional Denial of Service that disrupts services without malicious intent.
- **Examples**:
  - **Network DoS**: Layer 2 network loops without **Spanning Tree Protocol (STP)** can cause network failures.
  - **Bandwidth DoS**: Downloading large files over slow connections (e.g., multi-gigabyte files over DSL lines) can lead to congestion.

### Distributed Denial of Service (DDoS):
A **Distributed Denial of Service (DDoS)** attack is a malicious attempt to overwhelm a targeted server, service, or network with a flood of internet traffic from multiple sources.
- **Key Features**:
  - Utilizes botnets, networks of compromised devices controlled by the attacker.
  - Botnets are used to launch massive attacks, overwhelming servers with traffic.
  - **Zeus botnet**, for example, infected over 3.6 million PCs and used them to launch coordinated DDoS attacks.
  - DDoS attacks are considered an **asymmetric threat**, where the attacker can use relatively few resources to cause significant damage.

### DDoS Reflection and Amplification:
**DDoS reflection and amplification** techniques turn a small attack into a much larger one by leveraging other devices or services to reflect and amplify the attack.
- **Key Characteristics**:
  - These attacks are increasingly common and use protocols with little or no authentication or verification.
  - Common protocols involved in amplification include **NTP (Network Time Protocol)**, **DNS (Domain Name System)**, and **ICMP (Internet Control Message Protocol)**.
  - Attackers exploit these protocols to redirect large volumes of traffic toward the victim, amplifying the attack.

# 2.4 DNS Attacks

### DNS Attack Overview:
A **DNS attack** targets the Domain Name System (DNS), which is responsible for translating human-readable domain names into IP addresses used by computers to communicate over the network. By compromising DNS operations, attackers can manipulate the network traffic flow and redirect users to malicious sites.

### DNS Poisoning (DNS Cache Poisoning or DNS Spoofing):
**DNS poisoning** occurs when malicious data is injected into the DNS cache of a resolver, causing it to return incorrect IP addresses for domain names. This redirects users to fraudulent or malicious websites without their knowledge.
- **Methods**:
  - Modify the DNS server's cache to serve false information.
  - Modify the client’s **hosts file** to redirect DNS requests.
  - Send fake responses to a valid DNS request, allowing real-time redirection or on-path attacks.

### Domain Hijacking:
**Domain hijacking** occurs when an attacker gains control over a domain's registration, allowing them to manipulate where traffic for that domain is directed.
- **How It Happens**:
  - Attackers gain access to the domain registrar's account via brute force, social engineering, or other methods.
  - Once they have access, they can control the DNS names and IP addresses associated with the domain.

### URL Hijacking (Typosquatting):
**URL hijacking**, also known as **typosquatting**, involves attackers registering domain names similar to popular or legitimate URLs. This exploits typographical errors made by users when entering web addresses in their browsers.
- **Potential Outcomes**:
  - Attackers sell the misspelled domain to the legitimate company or interested parties.
  - Redirect the traffic to competitors' websites.
  - Create phishing sites to steal user data.
  - Infect users with a **drive-by download** (malicious code automatically downloaded without user consent).
  - Exploit common typographical errors or use different top-level domains (e.g., .com to .org) to mislead users.

# 2.4 Wireless Attacks

### Wireless De-authentication Attack:
A **wireless de-authentication attack** is a form of **Denial of Service (DoS)** targeting wireless networks, particularly Wi-Fi.
- **How It Works**:
  - Utilizes **802.11 management frames**, which are essential for managing wireless network operations.
  - These management frames are responsible for actions such as locating access points, managing Quality of Service (QoS), and handling association/disassociation with access points.
  - Early wireless standards did not secure these management frames, leaving them vulnerable to attacks.
  - **De-authentication** and **disassociation** frames are sent in cleartext, making them susceptible to interception and misuse.
  
- **Protection Against Deauth Attacks**:
  - As of **802.11ac**, encryption was added to protect management frames such as disassociate, de-authenticate, and channel switch announcements.
  - However, **beacons**, **probes**, **authentication**, and **association** frames must remain in cleartext for functional purposes.

### Radio Frequency (RF) Jamming:
**RF jamming** is a type of DoS attack that targets wireless communication by transmitting interfering signals on the same frequencies.
- **How It Works**:
  - A **DoS** attack that disrupts wireless communication by generating jamming signals on wireless frequencies.
  - This decreases the **signal-to-noise ratio** at the receiving device, making it impossible for the device to detect the legitimate signal from the access point.
  - Sources of interference can include non-malicious devices like microwaves and fluorescent lights.
  - **Reactive Jamming** occurs only when the attacker detects communication and then interferes with it.

- **Challenges**:
  - Jamming is usually effective only within close proximity to the access point (known as "fox hunting").
  - Directional antennas and attenuators can help attackers locate the source of reactive jamming.

### 2.4 On-Path Attack

An **on-path attack** occurs when an attacker places themselves between two devices, intercepting all the traffic exchanged between them. This is often referred to as a **man-in-the-middle (MITM)** attack.
- The attacker can **redirect your traffic**, passing it along to the intended destination without your knowledge.
- **Key Point**: You remain unaware that your data is being redirected.

**ARP Poisoning** (or ARP Spoofing) is a common method used in these attacks. It takes advantage of the **Address Resolution Protocol (ARP)**, which maps **IP addresses** to **MAC addresses** on a local network.
- The attacker sends false ARP messages to the network, associating their **MAC address** with the **IP address** of another device, such as a gateway or host.
- This can result in:
  - **Man-in-the-middle attacks**
  - **DoS (Denial of Service)**
  - **Data theft**
- **Why it works**: ARP lacks authentication, making it easy for attackers to spoof and redirect traffic.

Another form of on-path attack is the **on-path browser attack**, where malware or a trojan acts as a **proxy**. It redirects traffic before it reaches the network and after it leaves.
- This is relatively easy to execute with **encrypted traffic**.

# 2.4 Replay Attack

A **replay attack** is when a valid data transmission is intercepted and maliciously or fraudulently repeated or delayed. The attacker captures the data, retransmits it, and may even modify it before sending it again. 

### Attack Process:
1. **Interception of Data**: The attacker captures the original data transmission.
2. **Modification and Retransmission**: The attacker may alter the data before sending it again.
3. **Authentication Bypass**: If the data contains authentication information, the attacker can bypass security measures.

To carry out this attack, the attacker needs access to raw network data, which could be obtained through methods like **network taps**, **ARP poisoning**, or **malware on the victim’s system**.

### Pass the Hash (PtH) Attack:
In a **Pass the Hash** attack, an attacker captures the hashed version of a password and uses it to authenticate to a remote server or service.

**Steps involved**:
1. **Hash Capture**: The attacker obtains a hashed password (e.g., from network transmission or memory).
2. **Hash Usage**: The attacker uses the captured hash to authenticate to systems like **NTLM**.
3. **Authentication**: The attacker gains access without needing to know the original password.

**Mitigation**:
- **Salting passwords**: Adding a unique value to the password before hashing can make hash values more secure.
- **Encryption**: Protecting the transmission of passwords with encryption can prevent hash capture.
- **Session IDs**: Using session identifiers for authentication reduces reliance on password hashes.

### Browser Cookies:
Cookies store information on your browser for tracking, session management, and personalization. While not inherently executable, they present a **privacy risk** if stolen by attackers. They are typically not a direct security threat unless the attacker can access them.

### Session Hijacking (Sidejacking):
Session hijacking, or **sidejacking**, occurs when an attacker intercepts a session ID to impersonate the user. This can happen if the session ID is not properly encrypted or protected.

### Header Manipulation:
Attackers may manipulate HTTP headers to modify or hijack sessions.

**Preventing Session Hijacking**:
- **Encrypt end-to-end**: Ensure session IDs are encrypted to prevent interception.
- **Use HTTPS**: Websites should enforce HTTPS to secure communication.
- **Additional security**: Tools like the **HTTPS Everywhere** browser extension or enforcing **Force-TLS** can enhance session security.
- **VPN**: Encrypting sessions to a VPN concentrator further secures the connection.

# 2.4 Malicious Code

Malicious code refers to software or scripts used by attackers to exploit vulnerabilities, gain unauthorized access, or cause damage to systems. This can include techniques such as **social engineering**, **default credentials**, or exploiting **misconfigurations**, which may not require advanced technical skills but still pose serious risks to even well-secured systems.

### What is Malicious Code?
Malicious code is any software or code that an attacker uses to gain access to a system or exploit its vulnerabilities. This can include:
- **Executable files**
- **Scripts**
- **Macro viruses**
- **Worms**
- **Trojan horses**

### Protection Against Malicious Code:
Defense against malicious code requires multiple layers of security, including:
- **Anti-malware software**
- **Firewalls**
- **Continuous software updates and patches**
- **Secure computing habits**

### Example: WannaCry Ransomware
One notable example is **WannaCry**, a ransomware attack that exploited a vulnerability in **Windows SMBv1**. The malicious executable allowed arbitrary code execution, enabling the malware to spread rapidly across networks, encrypting files and demanding ransom.

Malicious code is often opportunistic, and while systems may be well-secured, it's essential to maintain proactive security measures and vigilance.

# 2.4 Application Attacks

Application attacks target vulnerabilities in software programs and web applications, exploiting weaknesses in the code or design. These attacks can lead to serious security breaches, allowing attackers to gain unauthorized access, execute arbitrary code, or manipulate data.

### Code Injection
Code injection occurs when attackers add malicious code into an application's input fields, which the program then processes. This is often enabled by poor programming practices that fail to properly handle input and output.

- **Common injection types**: HTML, SQL, XML, LDAP, etc.
- **Risk**: Allows attackers to execute unintended commands or alter the application's behavior.

### Buffer Overflow
A buffer overflow happens when a program writes more data to a buffer than it can handle. Buffers are temporary storage areas for data, and when data exceeds the buffer's size, it can overwrite adjacent memory, leading to crashes or exploitable conditions.

- **Consequences**: Crashes, arbitrary code execution, data corruption, and security bypass.
- **Mitigation**: 
  - **Bounds checking**: Ensure data fits within buffer limits.
  - **Safe functions**: Use functions with built-in checks like `strncpy` instead of `strcpy`.
  - **Address Space Layout Randomization (ASLR)**: Randomize memory addresses to make exploitation harder.
  - **Data Execution Prevention (DEP)**: Mark certain memory areas as non-executable to block injected code.
  - **Static and Dynamic Analysis**: Use tools to detect and fix vulnerabilities in code.

### Privilege Escalation
Privilege escalation occurs when attackers gain higher levels of access to a system by exploiting bugs, design flaws, or vulnerabilities, allowing them to perform actions normally restricted to privileged users.

- **Mitigation**: 
  - **Patch vulnerabilities**: Keep software up to date.
  - **Anti-virus/Anti-malware**: Ensure software is current and capable of detecting known threats.
  - **Block known exploits**: Prevent known vulnerabilities from being exploited.
  - **DEP & ASLR**: Protect memory and prevent unauthorized code execution.

### Cross-Site Request Forgery (CSRF)
Cross-Site Request Forgery (CSRF) tricks a user’s browser into executing unwanted actions on a different website where the user is authenticated. The attacker exploits the trusted relationship between the user’s browser and the website.

- **Risk**: Unauthorized actions, such as transferring funds or posting content, on behalf of the user.
- **Mitigation**: 
  - **Anti-forgery tokens**: Use cryptographic tokens to ensure requests come from trusted sources.
  - **User validation**: Check that each request is valid and originates from a legitimate source.

### Directory Traversal / Path Traversal
Directory traversal, or path traversal, allows attackers to access files and directories on a server that are outside the scope of the website’s directory. This could give them access to sensitive files, such as configuration files.

- **Risk**: Attackers can browse directories beyond the web server's root, potentially accessing critical system files.
- **Mitigation**: 
  - Ensure proper directory access controls are in place.
  - Avoid using unsafe file paths like `../` in web application code.

# 2.4 Cryptographic Attacks

Cryptographic attacks aim to break the security of encrypted data, often exploiting weaknesses in how cryptographic algorithms or protocols are implemented. While encryption itself is a powerful tool for securing data, poor implementation or outdated protocols can make it vulnerable.

### Birthday Attack
A **birthday attack** targets hash functions by exploiting the probability of finding two different inputs that produce the same hash value, known as a **collision**. This attack is named after the "birthday paradox," which shows that it’s easier to find two matching items (like birthdays) than most expect.

- **Steps**:
  1. Generate a large number of inputs.
  2. Compute hash values for each input.
  3. Search for collisions—two inputs that result in the same hash.
  
- **Mitigation**: 
  - Use strong hash functions like SHA-256 or SHA-3.
  - Incorporate randomization to make collisions harder to predict.
  - Regularly update cryptographic algorithms.
  - Choose hash functions with a larger output size to reduce collision probability.

### Collisions
A **collision** occurs when two different pieces of data produce the same hash. Since hash functions are meant to be unique, a collision undermines the integrity of the hash and potentially the security of the data.

### Downgrade Attack
A **downgrade attack** forces a system to use an older, less secure version of a software or communication protocol, weakening the overall security. This is often done by exploiting legacy support or intentionally manipulating the version negotiation process.

- **Examples**:
  - **SSL/TLS Downgrade**: An attacker intercepts the handshake process between a client and server, tricking them into using an older, vulnerable version of SSL/TLS.
  - **Cryptographic Algorithm Downgrade**: Forcing a system to use weaker cryptographic algorithms, such as downgrading from AES to DES.
  - **Software Version Downgrade**: Tricking software or systems into reverting to an older version with known vulnerabilities.

- **Mitigation**: 
  - Disable legacy protocols and algorithms.
  - Perform strict version checking during the handshake process to ensure only secure versions are used.
  - Use strong ciphersuites and disable outdated or weak encryption methods.
  - Regularly update and patch software.
  - Enforce security policies to mandate the use of the latest, secure versions and configurations.

In the context of web security, **SSL/TLS downgrade attacks** strip the 'S' from HTTPS, making the connection insecure.

![image](https://github.com/user-attachments/assets/3083ce1a-1ae7-4881-9f96-abbe73624c93)

# 2.4 Password Attacks

**Plaintext/Unencrypted Passwords**  
Some applications store passwords in plaintext, meaning they are not encrypted at all. This is a major security risk.

- **Problem**: Storing passwords in plaintext makes them easily accessible to attackers if they gain access to the application’s database or storage.
- **Recommendation**: Avoid using applications that store passwords in plaintext. Always choose applications that hash passwords before storing them.

**Hashing a Password**  
Hashing is a technique used to securely store passwords. A hash function transforms the password into a fixed-length string, called a "message digest" or "fingerprint."

- **How It Works**: 
  - Each unique input produces a different hash.
  - It is computationally infeasible to reverse-engineer the original password from the hash.
  - Hashing is a standard method for securely storing passwords.

**Spraying Attack**  
In a **spraying attack**, attackers try to access multiple accounts using the top three or more most commonly used passwords.

- **How It Works**: 
  - The attacker attempts to log in to multiple accounts using a common password (e.g., "123456" or "password").
  - If one password doesn’t work, they move to another account.
  - By using a small number of login attempts on each account, attackers avoid triggering lockouts or alerts.

**Brute Force Attack**  
A **brute force attack** involves trying every possible password combination until the correct one is found.

- **How It Works**: 
  - The attacker systematically tests all possible combinations.
  - This can take a significant amount of time, especially for complex passwords.
  - Using a strong hashing algorithm can slow down brute force attacks by making it more computationally expensive.

# 2.4 Indicators of Compromise (IOC)

Indicators of Compromise (IOC) refer to events or signs that suggest a system has been compromised by an attacker.

- **Common Indicators**: 
  - **Unusual network activity**: Significant or unexpected traffic spikes.
  - **Changes to file hash values**: Files may be altered or replaced by malware.
  - **Irregular international traffic**: Unexpected traffic patterns, especially from foreign IP addresses.
  - **Changes to DNS servers**: Unusual DNS server modifications may indicate DNS poisoning.
  - **Uncommon login patterns**: Logins from unusual devices or locations.
  - **Spikes in read requests to specific files**: Potential exfiltration or malicious access to sensitive data.
  
**Account Lockout**  
When credentials fail multiple times, the account may be locked out or disabled.

- **What It Indicates**: Too many unsuccessful login attempts could indicate a brute force attack or an attempt to gain unauthorized access.

**Concurrent Session Usage**  
Multiple logins to the same account from different locations or devices, often seen with automated attacks.

- **What It Indicates**: Could point to a compromised account being accessed from multiple locations at once, making it difficult to track the attacker.

**Blocked Content**  
Attackers may block auto-update connections or security patches to maintain their access and avoid detection.

- **What It Indicates**: This is a sign of an attacker trying to stay undetected and prevent security measures from being applied.

**Impossible Travel**  
Authentication logs showing login attempts from geographically distant locations in a short timeframe.

- **What It Indicates**: If a user logs in from one location and then from a distant location shortly afterward, this is a strong indicator of account compromise.

**Resource Consumption**  
Unusual spikes in resource use, such as bandwidth consumption or file transfers.

- **What It Indicates**: It could be a sign of data exfiltration or unauthorized activities. Firewalls often log these outgoing transfers.

**Resource Inaccessibility**  
Servers or resources becoming unavailable, possibly due to network disruptions or cyberattacks.

- **What It Indicates**: A server downtime, encrypted files (often due to ransomware), or denied access could indicate a serious attack.

**Out-of-Cycle Logging**  
Logs occurring at unexpected times, such as outside the regular maintenance or patch cycles.

- **What It Indicates**: Unauthorized access or actions may be logged outside of standard patch schedules. This could be an indication of system exploitation.

**Missing Logs**  
Attackers often remove or alter logs to cover their tracks, making it harder to detect the attack.

- **What It Indicates**: Missing logs such as authentication logs, file access logs, or firewall logs can suggest that an attacker is trying to erase their activity. Monitoring and securing logs is critical.

# 2.5 Segmentation and Access Control

**Segmentation** is a technique used to isolate and secure different parts of a network or system. It is done for several reasons, including improving performance for high-bandwidth applications, enhancing security, and ensuring compliance with regulations.

### Physical Segmentation
This involves using separate physical devices and infrastructure to create isolated segments within a network or system.
- **Dedicated Hardware**: Different segments are maintained on separate physical hardware such as routers, switches, and cables.
- **Complete Isolation**: Physical separation ensures that segments are entirely isolated, without shared components.
- **High Security**: Because there’s no direct way to traverse between segments without physical access, this method offers a high level of security.
  
**Example**: A corporate network where the finance department has its own dedicated server, switch, and cabling, separate from the other departments.

### Logical Segmentation
Logical segmentation divides a network into smaller segments using software and network configurations.
- **VLANs**: This is often achieved by using Virtual Local Area Networks (VLANs), which partition a single physical network into multiple logical networks.
- **Access Control**: Traffic between segments is controlled by network devices such as switches and routers that manage traffic based on defined policies.
- **Flexible Configuration**: Logical segmentation is more flexible and easier to reconfigure than physical segmentation, enabling dynamic network management.
  
**Example**: A university network that separates student, faculty, and administrative traffic using VLANs on the same physical network infrastructure.

### Virtual Segmentation
Virtual segmentation creates isolated virtual environments within a single physical host, typically through virtualization technologies.
- **Virtual Machines (VMs)**: Multiple VMs can run on a single physical server, each with its own operating system and applications, isolated from each other.
- **Hypervisors**: A hypervisor manages the creation and operation of VMs, ensuring proper isolation and resource allocation.
- **Network Virtualization**: Virtual switches and routers can be used to segment network traffic within virtualized environments.
  
**Example**: A cloud service provider hosts multiple virtual servers for different customers on the same physical hardware, using VMs and virtual networks to ensure data and application isolation.

### Access Control Lists (ACLs)
ACLs are used to control traffic by specifying which users or devices can access specific resources and under which conditions.
- **Restrictions**: ACLs allow traffic based on criteria like source IP, destination IP, port numbers, application types, and even time of day.
- **Risk**: Careful planning is needed when creating ACLs, as improper configuration can lock users or administrators out of critical systems.
  
**Examples of ACL Permissions**:
- **Bob** can read files.
- **Fred** can access the network.
- **James** can access network 192.157.1.0/24 using TCP ports 80, 443, and 8088.

Many operating systems use ACLs to manage access to files, directories, and network resources.

### Application Allow/Deny Lists
Security policies can use allow and deny lists to control application execution.

- **Allow List**: Only applications that are explicitly approved can run. This method is very restrictive but offers high security.
- **Deny List**: Only applications on the "bad list" are blocked from execution, typically used by anti-virus and anti-malware software.

**Examples of Allow and Deny Lists**:
- **Application Hash**: Only applications with a specific, approved hash value can run.
- **Certificate**: Only applications signed with a valid certificate are allowed to execute.
- **Path**: Only applications located in designated folders can be executed.
- **Network Zone**: Applications can only run if they are located within a specific network zone.

# 2.5 Mitigation Techniques

Mitigation techniques refer to the strategies and processes used to reduce the impact of security events or potential security breaches.

### Patching
Patching is crucial for maintaining system stability and applying security fixes to vulnerabilities.
- **Monthly Updates**: Regular, incremental updates that address known security issues.
- **Third-Party Updates**: Updates for third-party applications, device drivers, and software components.
- **Auto-Update**: While convenient, it is not always the best option due to potential compatibility issues or unexpected outcomes.
- **Emergency Out-of-Band Updates**: Critical security patches that are applied outside of the regular update schedule, often to address zero-day vulnerabilities or high-severity threats.

### Encryption
Encryption ensures that unauthorized parties cannot access application data or files.
- **File-Level Encryption**: Encrypts specific files using technologies like EFS (Encrypted File System).
- **Full Disk Encryption (FDE)**: Encrypts the entire contents of a disk, such as using BitLocker (Windows) or FileVault (macOS).
- **Application Data Encryption**: Managed by the application itself, this protects stored data from unauthorized access.

### Monitoring
Monitoring involves collecting data from various devices and systems to detect potential security events.
- **Built-In Technology**: Many devices come with built-in logging and monitoring capabilities.
- **Integrated Into Servers**: Servers often include sensors, IPS (Intrusion Prevention Systems), firewall logs, authentication logs, and more.
- **Collectors and Consoles**: Data aggregation tools such as SIEM (Security Information and Event Management) consoles, syslog servers, and proprietary tools help consolidate and analyze logs.
- **Correlation Engines**: Many SIEM systems include correlation engines that compare data from diverse sensors to identify unusual patterns.

### Least Privilege
The principle of least privilege dictates that users should only have the minimum permissions necessary to perform their tasks.
- **Minimal User Rights**: User accounts should be restricted to only the permissions required for their role.
- **Application Privileges**: Applications should run with the least privileges, and administrative rights should be granted sparingly.
- **Limiting Malicious Behaviour**: Restricting administrative privileges limits the scope of any potential damage caused by malicious actions.

### Configuration Enforcement
Ensures that devices meet security requirements before being allowed access to the network.
- **Posture Assessment**: Devices are assessed for compliance each time they connect to the network, checking factors like OS patch levels, EDR (Endpoint Detection and Response) versions, and firewall status.
- **Compliance Checks**: Systems that do not meet the required configuration are quarantined, often in a private VLAN with limited access.
- **Recheck After Corrections**: Devices that were initially out of compliance are rechecked after corrections have been made to ensure they meet the security standards.

### Decommissioning
Proper decommissioning is critical to prevent data leakage or unauthorized access to sensitive information.
- **Data Removal**: Sensitive data should be completely removed from devices before decommissioning, especially from storage devices like HDDs, SSDs, and USB drives.
- **Device Reuse**: If devices are recycled for use in other systems, all data must be wiped or destroyed to ensure confidentiality.
- **Device Disposal**: Devices should be securely wiped and destroyed to prevent unauthorized recovery of any data.

# 2.5 Hardening Techniques

Hardening techniques involve strengthening systems to minimize vulnerabilities and reduce the likelihood of successful attacks.

### System Hardening: Server
To secure a server, various hardening practices should be followed:
- **Updates**: Regularly apply operating system updates, service packs, and security patches to fix known vulnerabilities.
- **User Accounts**: Enforce policies for minimum password lengths and complexity, as well as restrictions on account usage and login attempts.
- **Network Access**: Limit network access to only necessary services, reducing the attack surface.
- **Monitoring and Security**: Deploy anti-virus, anti-malware tools, and continuously monitor system activity for potential threats.

### Encryption
Encryption helps prevent unauthorized access to data and communication:
- **File System Encryption**: Encrypt sensitive files using built-in tools like EFS (Encrypting File System) on Windows.
- **Full Disk Encryption (FDE)**: Tools like BitLocker (Windows) and FileVault (macOS) encrypt entire disk drives, securing data even if the device is lost or stolen.
- **Network Communication Encryption**: Encrypt all network traffic with a VPN and encrypt application data to ensure confidentiality during transmission.

### The Endpoint
The endpoint is the user’s access point to systems, applications, and data. Protecting endpoints is crucial for a layered security approach:
- **Defense in Depth**: Implement multiple layers of security, from hardware to software, to protect the endpoint from various threats.

### Endpoint Detection and Response (EDR)
EDR provides advanced protection to endpoints by detecting, investigating, and responding to security incidents:
- **Threat Detection**: EDR systems use signatures, behavioral analysis, and machine learning to detect threats. They go beyond traditional signature-based detection.
- **Root Cause Analysis**: Investigate incidents to determine how an attack occurred and its impact.
- **Automated Response**: EDR systems can automatically isolate affected systems, quarantine threats, and roll back changes without user or technician intervention.

### Host-Based Firewall
A host-based firewall runs on individual endpoints and controls application-level traffic:
- **Traffic Control**: It allows or denies incoming and outgoing traffic based on application processes.
- **Malware Prevention**: It can identify and block unknown processes, potentially stopping malware before it can execute.
- **Centralized Management**: These firewalls can be managed centrally to enforce consistent security policies across endpoints.

### Host-Based Intrusion Prevention System (HIPS)
HIPS helps detect and block known attacks by securing the OS and application configurations:
- **Signature-Based Detection**: Uses predefined signatures to identify and block known threats.
- **Heuristic and Behavioral Analysis**: Identifies abnormal behavior and potential attacks based on patterns rather than known signatures.
- **Protection**: Can detect buffer overflows, unauthorized registry updates, and file modifications to sensitive areas of the OS.

### Open Ports and Services
Every open port is a potential entry point for an attacker:
- **Limit Open Ports**: Only keep necessary ports open and control access to them using firewalls, including Next-Generation Firewalls (NGFWs).
- **Service Management**: Disable unused or unnecessary services, which may come pre-installed with the OS or third-party applications.
- **Port Scanning**: Use tools like Nmap to identify open ports and services, ensuring no unnecessary services are exposed.

### Default Password Changes
Many devices come with default management interfaces and passwords:
- **Change Default Credentials**: Always change default passwords for network devices, critical systems, and applications.
- **Add Extra Security**: Implement additional authentication measures and strong passwords to increase security.

### Removal of Unnecessary Software
Removing unneeded software reduces the attack surface:
- **Software Management**: Unused software can introduce security vulnerabilities through bugs and unpatched exploits.
- **Risk Reduction**: By removing unnecessary software, you reduce the number of vulnerabilities and simplify patch management.
</details>

<details>
<summary>3.0 Security Architecture</summary>

# 3.1 Cloud Infrastructure

The Cloud Responsibility Matrix, also known as the shared responsibility model, outlines the division of responsibilities between a Cloud Service Provider (CSP) and its customers.

### Summary:
- **IaaS**: Virtualised computing resources
- **PaaS**: Platform for application development
- **SaaS**: Ready-to-use software applications

![image](https://github.com/user-attachments/assets/d82b1dd2-60bd-4ced-a55a-7b3bd83dca02)


### Infrastructure as a Service (IaaS)
IaaS provides virtualised computing resources over the internet, offering fundamental building blocks like virtual machines, storage, and networking, allowing users to run their own applications and operating systems.

#### Key Characteristics:
- **Resources**: Virtual machines, storage, networks, and load balancers
- **User Control**: Users have maximum control over the infrastructure, including the OS, storage, and deployed applications
- **Scalability**: Easily scalable resources as needed, without the need for physical hardware
- **Cost**: Pay-as-you-go pricing model, users pay for the resources they use.

#### Examples:
- Amazon Web Services (EC2)
- Microsoft Azure Virtual Machines
- Google Cloud Compute Engine

### Platform as a Service (PaaS)
PaaS provides a platform allowing customers to develop, run, and manage applications without dealing with the underlying infrastructure. It includes services for application development, deployment, and testing.

#### Key Characteristics:
- **Resources**: Middleware, development tools, database management systems, and more
- **User Control**: Users manage the applications and data while the provider manages the infrastructure and platform
- **Development Focus**: Streamlines the development process by providing pre-configured environments and tools
- **Scalability**: Automatically manages scaling of the underlying infrastructure

#### Examples:
- Google App Engine
- Microsoft Azure Services
- Heroku

### Software as a Service (SaaS)
SaaS delivers software applications over the internet on a subscription basis. Users can access these applications through web browsers, and the service provider manages all underlying infrastructure and platforms.

#### Key Characteristics:
- **Resources**: Software applications delivered over the internet
- **User Control**: Users interact with the application itself, with no control over the underlying infrastructure or platform
- **Convenience**: Ready-to-use applications that require no installation or maintenance by the user
- **Accessible**: From any device with an internet connection

#### Examples:
- Google Workspace
- Microsoft Office 365
- Salesforce

### Hybrid Considerations
A hybrid cloud involves more than one public or private cloud, which adds an additional level of complexity:
- **Network Protection Mismatches**: Authentication across platforms, firewall configurations, server settings, etc.
- **Different Security Monitoring**: Logs are diverse and cloud-specific
- **Data Leakage**: Data is shared across the public internet

### Third-party Vendors in the Cloud
Third-party vendors provide various services and solutions that complement or extend the capabilities of primary cloud service providers. They offer specialised services, tools, and applications that enhance functionality, security, and management of cloud environments.

### Serverless Architecture
Serverless refers to a cloud-native development model that allows developers to build and run applications and services without needing to manage infrastructure or server-side IT.

#### Key Characteristics:
- **No Server Management**
- **Event-Driven**
- **Auto-Scaling**
- **Pay-Per-Use**
- **Stateless**

#### Examples:
- Microservices: Breaking down applications into smaller, independent functions that can be developed, deployed, and scaled separately.
- Real-time File Processing: Automatically processing files when they are uploaded to a storage service
- API Backends: Building lightweight, scalable backends for mobile or web applications
- IoT Data Processing: Processing data from IoT devices in real-time
- Automation and Orchestration

### Microservices and APIs
Monolithic applications involve one big application that does everything, containing all decision-making processes, business logic, data input/output, etc. This creates challenges with a large codebase and change control.

#### APIs:
- **Scalable**: Scale only the microservices you need
- **Resilient**: Outages are contained
- **Security and Compliance**: Containment is built-in

# 3.1 Network Infrastructure

### Physical Isolation
Physical isolation involves separating devices so that if an attacker gains access to one part of the network, they cannot access other parts. For example:
- Web servers in one rack, database servers in another rack, with an air gap between different services.
- Customer A on switch 1 and Customer B on switch 2, ensuring no opportunity for mixing data.

![image](https://github.com/user-attachments/assets/1bf2139d-74d9-42f2-99fd-4104e4b0bc21)


### Logical Segmentation with Virtual Local Area Networks (VLANs)
Logical segmentation involves separating networks at the data link layer rather than physically. Devices in different VLANs cannot communicate with each other unless routed through a layer 3 device, such as a router.

### Software Defined Networking (SDN)
SDN is a network architecture that decouples the control plane from the data plane, making the network more flexible and easier to manage.

#### Key Components of SDN:
- **Data Plane**: Handles the forwarding of data packets, including functions like encryption, trunking, NAT, and more.
- **Control Plane**: Manages routing tables and determines the path that data should take through the network. It controls the data plane's behavior by updating session, routing, and NAT tables.
- **Management Plane**: This layer allows for the configuration and management of network devices, influencing the control plane, which in turn adjusts the data plane.

### Layers of SDN:
1. **Infrastructure Layer / Data Plane**: Responsible for forwarding data, such as network frames and packets. Includes tasks like forwarding, trunking, and encryption.
2. **Control Layer / Control Plane**: Manages the network's routing and session tables and updates dynamic routing protocols.
3. **Application Layer / Management Plane**: Provides the configuration and management of network devices, which then influence the actions of the control and data planes.

![image](https://github.com/user-attachments/assets/03575fb3-ba8d-4051-b45f-11fe1fdab392)
![image](https://github.com/user-attachments/assets/9511ca12-5c49-4c1c-87dc-bd6044b56c63)

# 3.1 Other Infrastructure Concepts

### IT Security Categories
IT security is generally divided into two main categories:
- **On-premises data**: Data stored and managed within the organization’s own infrastructure.
- **Cloud-based data**: Data stored and managed by a third-party provider in a cloud environment.

### Cloud-based Security
Cloud-based security is centralized, making it cost-effective:
- No need for dedicated hardware or a physical data center to secure.
- Third-party providers handle all security and infrastructure management.

### On-premises Security
On-premises security places the responsibility on the client:
- The organization must manage and secure its data center infrastructure.
- Offers more control over security but requires significant resources.

#### Customizing Security Posture:
- Full control when security and data are kept in-house.
- An on-site IT team can better manage security but may be expensive and challenging to staff.
- Local teams can maintain uptime and availability with regular checks and direct support, but security changes might take time and incur additional costs.

### Centralised vs Decentralised Security Management
Organizations often operate in a physically decentralised manner, spanning multiple locations or cloud services. Managing such a diverse network of systems can be challenging. A **centralised approach** provides several benefits:
- Consolidated security management from a single console.
- Correlated alerts and log analysis, offering a comprehensive view of system status.
- Maintenance patching and monitoring of users, devices, and applications.
- Potential downsides include a single point of failure, performance issues, and additional resource requirements like storage and CPU power.

### Virtualisation
Virtualisation enables the running of multiple operating systems on a single hardware unit:
- Each virtual machine operates independently with its own OS.
- Although it allows better resource utilization, it can add overhead and complexity, making virtualisation relatively expensive.

### Application Containerisation
Application containerisation allows multiple applications to run simultaneously on the same hardware, with each isolated in its own container:
- Applications are self-contained, preventing interaction between them.
- Containers use a standard image format and the host system’s kernel, ensuring secure separation between applications.
- Containers include everything needed to run an application: code, libraries, and dependencies.
![image](https://github.com/user-attachments/assets/370db21c-b591-4955-9c15-e6af10a4eeb8)
-----------------------------------------------------------------------------------------
![image](https://github.com/user-attachments/assets/a4b01691-dec3-4051-ab33-b24bad70e8a6)


### Internet of Things (IoT)
The **Internet of Things (IoT)** refers to devices connected to the network for various purposes:
- **Examples**: Sensors, smart devices (e.g., thermostats, doorbells), wearables (smartwatches), and facility automation (temperature, air quality).
- Security concerns arise from weak default settings as IoT manufacturers may not prioritize security.

### SCADA / ICS (Supervisory Control and Data Acquisition / Industrial Control Systems)
Large-scale systems used to manage industrial processes:
- **SCADA/ICS systems**: Used in power generation, refining, manufacturing, energy, and logistics.
- **Distributed Control Systems**: Provide real-time information and control within industrial environments.
- Requires **extensive segmentation** to ensure there is no access from external sources.

### RTOS (Real-Time Operating System)
An **RTOS** is an operating system designed for deterministic processing:
- Critical in industries such as **automotive**, **military**, and **industrial control systems** where processes must be completed within strict time constraints.
- Security concerns are amplified because RTOS systems must always be available, and knowing what security measures are in place can be difficult.

### Embedded Systems
**Embedded systems** are hardware and software designed for specific tasks:
- Used in devices like **traffic lights**, **digital watches**, and **medical imaging systems**.
- Highly focused on their task but may lack flexibility and have limited security features.

### High Availability
High availability systems are critical to ensuring continuous operation, particularly in environments requiring minimal downtime.

# 3.1 Infrastructure Considerations

### Availability
Availability refers to system uptime, which is crucial for accessing data and completing transactions:
- Ensures systems are accessible but only to authorized users.
- It is a foundation of IT security.
- A balancing act between making systems available while maintaining security.
- A significant investment in monitoring and redundant systems is necessary to maintain availability.

### Resilience
Resilience refers to the ability to recover from failures and continue operating:
- Focus on how quickly the system can recover if something breaks.
- Address the root cause of the issue.
- Important factors include the installation of replacement hardware, software patch availability, and redundant systems.
- **MTTR** (Mean Time to Repair) is a key metric for recovery efficiency.

### Cost
The cost of maintaining infrastructure is an important consideration:
- Initial installation costs.
- Ongoing maintenance costs, including annual operational expenses.
- Replacement and repair costs, which may require extra resources.
- Considerations between operating vs capital expenses, including tax implications.

### Responsiveness
Responsiveness is critical, particularly for interactive applications:
- The speed at which a system can respond to user requests is important.
- Speed is a key metric, and the performance of all components in an application contributes to this.
- There is always a potential "weakest link" that can hinder responsiveness.

### Scalability
Scalability refers to the ability to adjust capacity to meet demand:
- The ability to scale up or down efficiently, also known as **elasticity**.
- Security monitoring must also scale with the system to maintain protection as the infrastructure grows or shrinks.

### Ease of Deployment
Deploying applications involves managing multiple components:
- Key elements include web servers, databases, caching servers, and firewalls.
- Deployment may require managing hardware resources, cloud budgets, and orchestrating automation or change control processes.

### Risk Transference
Risk transference involves transferring some of the risks to third parties:
- **Cybersecurity Insurance**: Covers losses from attacks, such as ransomware, and mitigates the cost of downtime and legal issues.
- Insurance can help recover internal losses, such as those resulting from business downtime, and reduce costs associated with legal proceedings.

### Ease of Recovery
Recovery from failures is an essential part of infrastructure resilience:
- **Malware Infection**: In case of infection, quickly reload the operating system from the original media (1 hour) or reload the corporate image (10 minutes).
- The quicker the recovery, the less impact it has on business operations.

### Patch Availability
Regular patching is crucial for maintaining security and software health:
- Software is rarely static; it requires bug fixes, security updates, etc.
- Ensure systems are running the latest version, typically checked after installation.
- Companies with regular patching schedules (like Microsoft's monthly updates) are more secure than those who rarely patch.

### Inability to Patch
Some devices, such as embedded systems, may be difficult or impossible to update:
- Systems like HVAC controls or time clocks may not allow end-user updates.
- Security risks may arise, and additional security measures like firewalls may be necessary to protect these systems.

### Power
Power is a foundational requirement for infrastructure:
- Data centers and office buildings have different power needs.
- Primary power is supplied by one or more providers, and backup services include **UPS** (Uninterruptible Power Supply) and generators.

### Compute
Compute resources perform the processing and data handling tasks:
- Compute engines may be limited to a single processor or spread across multiple CPUs.
- The use of multiple CPUs across clouds adds complexity but provides enhanced scalability.

# 3.2 Secure Infrastructures

### Device Placement
Every network is unique, but common principles can be applied to enhance security. Placement of devices within the network plays a crucial role in securing infrastructure:
- Firewalls: Separate trusted networks from untrusted networks, ensuring controlled communication.
- Honeypots, jump servers, load balancers, and sensors can create a more secure computing environment by trapping or redirecting potential attackers and balancing traffic loads.

![image](https://github.com/user-attachments/assets/64e71a5c-1f12-4bb0-909b-4ca496168b7d)


### Security Zones
Zone-based security technologies provide more flexibility and security than traditional IP address-based ranges. Each area of the network is associated with a specific zone:
- Trusted Zone: Includes internal networks or systems that are trusted and protected.
- Untrusted Zone: External networks or systems, such as the internet, that pose higher security risks.
- Internal Zone: The internal corporate network or systems.
- External Zone: External connections that require filtering or inspection.
- Screened Zone: A monitored area used for special security controls.

This zoning model simplifies security policies:
- **Trusted to Untrusted**: Communications allowed from trusted zones to untrusted zones.
- **Untrusted to Screened**: Communications from untrusted zones to a screened zone are filtered and monitored.
- **Untrusted to Trusted**: Prevents or tightly controls communications from untrusted zones to trusted zones.

### Attack Surface
The attack surface is the total set of vulnerabilities in a system or network that could be exploited by attackers:
- **Application Code**: Flaws or vulnerabilities in the application code can be targeted.
- **Open Ports**: Exposed ports can be entry points for attacks.
- **Authentication Process**: Weaknesses in how users authenticate can be exploited.
- **Human Error**: Mistakes made by users or administrators can create vulnerabilities.

To minimize the attack surface:
- Regularly audit the code for security flaws.
- Block unused ports on the firewall to limit exposure.
- Monitor network traffic in real-time to detect any unusual or unauthorized access attempts.

### Connectivity
Ensuring secure connections between devices and networks is vital for maintaining a safe infrastructure:
- **Secure Network Cabling**: Protect physical network cables from tampering or unauthorized access.
- **Application-Level Encryption**: Use encryption to protect data at the application layer.
- **Network-Level Encryption**: Utilize **IPsec tunnels** and **VPN connections** to secure data transmission at the network layer, ensuring private communication over public networks.

# 3.2 Intrusion Prevention

### Intrusion Prevention System (IPS)
An **Intrusion Prevention System (IPS)** actively monitors network traffic in real-time to detect and prevent potential intrusions. The system inspects data packets as they traverse the network and takes action to block malicious traffic before it can enter the network.

### Intrusions
Intrusions typically exploit vulnerabilities in operating systems, applications, or other systems. Common types of intrusions include:
- **Exploits** against operating systems or applications
- **Buffer overflows**, where excess data overflows into adjacent memory
- **Cross-site scripting (XSS)**, which targets web applications
- Other **vulnerabilities** that attackers can exploit

### Detection vs Prevention
The key difference between intrusion detection and prevention is their approach to handling threats:
- **Intrusion Detection System (IDS)**: Primarily designed to detect malicious activity and generate alerts or alarms when a potential threat is identified.
- **Intrusion Prevention System (IPS)**: Actively blocks malicious traffic and stops intrusions before they can enter the network, offering a more proactive defense.

### Failure Modes
- **Fail-open**: In the event of a failure, the system allows data to continue flowing. This can be useful in situations where availability is prioritized over security, but it may expose the network to attacks.
- **Fail-closed**: When the system fails, data does not flow, effectively blocking all traffic. While this prevents unauthorized access, it can lead to service disruption.

### Device Connections
- **Active Monitoring**: In this configuration, the system is connected inline with network traffic, meaning it can immediately identify malicious traffic and block it in real-time as it passes through the system. Intrusion prevention is typically implemented through active monitoring.
  
- **Passive Monitoring**: In passive monitoring, the system examines a copy of the network traffic (using a tap or port mirror) and cannot take action to block or prevent traffic. Intrusion detection systems (IDS) are commonly used in passive monitoring setups, as they can only alert administrators about potential threats but do not actively block them.

# 3.2 Network Appliances

### Jump Server
A **Jump Server** provides secure access to protected network zones. It serves as a gateway for users to access systems in secure areas of the network.

Key Features:
- **Highly-secured device**: The jump server is hardened and closely monitored to ensure that it remains secure.
- **Access Mechanism**: Users typically connect to the jump server using protocols such as SSH, Tunnel, or VPN to securely access other network resources.
- **Security Concern**: If the jump server is compromised, it could lead to a significant security breach, as it often serves as the gateway to more sensitive areas of the network.

### Proxy
A **Proxy** sits between the user and the external network, acting on behalf of the user by forwarding their requests.

Key Functions:
- **Request Forwarding**: The proxy receives user requests and sends them to the external network, masking the user's identity and location.
- **Caching**: Proxies can cache information, improving network performance by reducing the need to fetch the same data multiple times.
- **Access Control**: Proxies can be used to control access to certain resources, ensuring that only authorized users can access specific sites or services.
- **URL Filtering**: Proxies can filter URLs to block access to malicious or undesirable websites.
- **Content Scanning**: Proxies can scan content for malicious or unwanted material before it reaches the user.
- **Explicit Configuration**: Some applications may require explicit configuration to work with a proxy, meaning users or devices must be set up to route their traffic through the proxy server.

# 3.2 Port Security

### Port Security on Network Interfaces
**Port Security** refers to securing the individual interfaces on a network switch or wireless access point to prevent unauthorized access. It restricts which devices can connect to the network and ensures only authorized devices are granted access.

### Extensible Authentication Protocol (EAP)
**EAP** is an authentication framework used to define several different ways to authenticate devices or users. It is widely used in wireless networks and integrates with 802.1X to enforce security.

Key Features:
- **Various Authentication Methods**: EAP allows different authentication methods based on RFC standards, and manufacturers can create their own EAP methods.
- **Integration with 802.1X**: EAP works in conjunction with **IEEE 802.1X**, a network access control (NAC) standard, to prevent access to the network until successful authentication occurs.

### IEEE 802.1X
**IEEE 802.1X** is a port-based network access control (NAC) protocol that ensures devices cannot access the network until they authenticate properly.

Key Features:
- **Port-based Control**: 802.1X secures the network by controlling access to network ports. Devices must authenticate before gaining access to the network.
- **Authentication Process**: It is used in combination with an authentication database, such as **RADIUS**, **LDAP**, **TACACS+**, or **Kerberos**, to validate credentials.

### EAP and 802.1X Interaction
EAP integrates with **802.1X** to enforce port security by requiring authentication before granting network access.

Components of the Authentication Process:
- **Supplicant**: The client device that requests access to the network.
- **Authenticator**: The network device (e.g., a switch or wireless access point) that controls access to the network.
- **Authentication Server**: A server (e.g., RADIUS) that validates the credentials provided by the supplicant before granting access.

# 3.2 Firewall Types

### Overview of Firewalls
**Firewalls** are security devices or software designed to control the flow of network traffic. They enforce corporate security policies by regulating both inbound and outbound data, protecting sensitive material, controlling access to inappropriate content, and preventing attacks such as viruses and malware.

Key Functions:
- **Control Network Traffic**: Firewalls control the flow of traffic between networks, ensuring only legitimate traffic passes through.
- **Corporate Control**: Used to manage sensitive information and restrict access to unauthorized sites and services.
- **Protection Against Attacks**: Firewalls help defend against viruses, malware, and other cyber threats.

### Network-Based Firewalls
Network-based firewalls filter traffic by examining port numbers or applications. They operate at different layers of the OSI model.

Key Features:
- **OSI Layer 4 vs Layer 7**: Firewalls may filter traffic at OSI Layer 4 (Transport Layer, e.g., port numbers) or Layer 7 (Application Layer, e.g., web applications).
- **Traditional vs NSFW Firewalls**: Network-based firewalls are often configured to block traffic deemed not safe for work (NSFW), such as adult content.
- **Traffic Encryption and VPN**: Firewalls can encrypt traffic and establish VPN tunnels between sites.
- **Layer 3 Functionality**: Many firewalls also act as routers, sit on the ingress/egress of the network, provide NAT (Network Address Translation), and authenticate dynamic routing communications.

### Unified Threat Management (UTM) / All-in-One Security Appliance
**UTM** appliances combine multiple security functions in one device. These are typically focused at Layer 4 and filter traffic based on port numbers.

Key Features:
- **URL Filtering**: Blocks or allows access to specific websites.
- **Content and Malware Inspection**: Scans network traffic for harmful content and malware.
- **Spam Filtering**: Protects against unwanted email.
- **Additional Functions**: May include CSU/DSU, routers, switches, IDS/IPS, bandwidth shaping, and VPN endpoints.

### Next-Generation Firewall (NGFW)
**NGFWs** work at the OSI Application Layer and can make forwarding decisions based on the applications in use.

Key Features:
- **Deep Packet Inspection (DPI)**: Every packet is analyzed, and decisions are made based on detailed inspection of the application layer traffic.
- **Advanced Decodes**: Identifies who is sending the traffic, where it’s going, and what’s in the application layer.
- **Application-Based Control**: NGFWs control traffic based on the specific applications that generate it.
- **Intrusion Prevention**: NGFWs include IPS features that apply application-specific vulnerability signatures to traffic.
- **Content Filtering**: Controls access to websites and content through URL filters.

### Web Application Firewall (WAF)
**WAFs** are specialized firewalls designed to protect web applications by filtering and monitoring HTTP/HTTPS traffic.

Key Features:
- **Analyzes Web Input**: WAFs apply rules to control incoming and outgoing web traffic.
- **Protection Against Attacks**: WAFs block common exploits such as SQL injection, cross-site scripting (XSS), and other methods of exploiting web applications.
- **PCI DSS Compliance**: WAFs are often required for compliance with the Payment Card Industry Data Security Standard (PCI DSS), which mandates protection of payment-related data.

# 3.2 Secure Communication

### VPNs (Virtual Private Networks)
A **VPN** creates an encrypted link across a public network, such as the internet, ensuring secure data transmission between endpoints.

#### VPN Concentrator
A **VPN concentrator** is the endpoint device that employees connect to when using an encrypted link to access the corporate network.

Key Features:
- **Encryption/Decryption**: The concentrator encrypts outgoing data and decrypts incoming data.
- **Integration with Firewalls**: Often, a VPN concentrator is integrated into a firewall device.

### Encrypted Tunnel
An **encrypted tunnel** ensures privacy and confidentiality of data traveling across the public internet.

![image](https://github.com/user-attachments/assets/8e3b099a-6763-4a7a-b66f-5c2298607333)


Key Features:
- **Data Encryption**: The tunnel wraps data in multiple layers of encryption to prevent unauthorized access.
- **Headers and Trailers**: The original data packet is wrapped in IPsec headers and trailers, which the VPN concentrator uses to determine where the data should go.

### SSL/TLS VPN (Secure Sockets Layer VPN)
**SSL/TLS VPNs** use the widely recognized SSL/TLS protocol (TCP/443) to encrypt and secure the communication channel.

Key Features:
- **Firewall-Friendly**: SSL/TLS VPNs typically do not encounter firewall issues because they operate over port 443.
- **No VPN Clients**: Users do not need to install large VPN clients, as the communication can occur through a browser or lightweight software.
- **Authentication**: Unlike IPsec, SSL/TLS VPNs often do not require digital certificates or shared passwords for user authentication.
- **On-Demand Access**: SSL/TLS VPNs allow remote devices to connect on-demand via a VPN client or a browser.
- **Always-On Configuration**: Some VPN software can be configured to always remain connected.

### Site-to-Site IPsec VPN
**Site-to-site IPsec VPNs** are "always-on" connections between two networks, usually connected through firewalls that act as VPN concentrators.

Key Features:
- **Always-On**: The connection remains active continuously, making it ideal for business-to-business or branch office connections.
- **Firewall Integration**: Firewalls are often configured to handle IPsec VPN connections, providing a seamless and secure connection between sites.

### SD-WAN (Software-Defined Wide Area Network)
**SD-WAN** is an advanced networking solution designed to optimize the connectivity and performance of wide area networks, especially for cloud-based applications.

Key Features:
- **Cloud-Based Optimization**: SD-WAN enables direct communication with cloud-based applications without routing traffic through a central point.
- **Flexibility**: SD-WAN is built for flexibility, improving cloud application performance and reducing dependency on traditional data centers.

### SASE (Secure Access Service Edge)
**SASE** is a next-generation solution that combines network security with WAN capabilities, offering secure access to applications and data, particularly in cloud environments.

Key Features:
- **Efficiency in Communication**: SASE streamlines communication to cloud-based applications, improving security and performance.
- **Comprehensive Security**: It offers a blend of security solutions, including firewalling, secure web gateways, and zero trust network access (ZTNA).
- **Planning and Implementation**: Implementing SASE requires careful planning, as it is a complex, integrated solution combining networking and security functions.

### Selection of Effective Controls
When selecting secure communication options, consider the following:

- **VPN**: 
  - SSL/TLS VPNs for user access.
  - IPsec tunnels for site-to-site communication.
  
- **SD-WAN**: 
  - Manages network connectivity to the cloud but may not fully address security concerns.
  
- **SASE**: 
  - Offers a comprehensive, secure solution for cloud-based communication, requiring careful planning and implementation to ensure effectiveness.

# 3.3 Data Types and Classifications

### Data Types

1. **Regulated Data**
   - Managed by third-party organizations and subject to government laws and statutes.
   - **Example**: Credit card data must be stored in a manner compliant with PCI DSS regulations.

2. **Trade Secrets**
   - Information unique to an organization, such as secret formulas or business processes.
   - Protected from disclosure to maintain competitive advantage.

3. **Intellectual Property**
   - May be publicly visible but is protected by copyright, trademarks, or patents.
   - Protects innovations and creations of an organization.

4. **Legal Information**
   - Information that should be publicly available but must also protect private data.
   - Includes court records, judge and attorney information, and other legal documentation.
   - **Example**: PII (Personally Identifiable Information) should be kept private.

5. **Financial Information**
   - Includes internal financial details, customer financial information, and payment records.
   - **Example**: Credit card data, bank records, and payment details.

6. **Human-Readable vs. Non-Human Readable Data**
   - **Human-Readable**: Data that is clear and understandable by humans (e.g., CSV, XML, JSON).
   - **Non-Human Readable**: Data encoded or represented in formats that humans cannot directly interpret (e.g., barcodes, images).

---

### Data Classifications

1. **Proprietary Data**
   - Data owned by an organization, often including trade secrets or other unique information specific to the organization.

2. **PII (Personally Identifiable Information)**
   - Information that can be used to identify an individual, including but not limited to:
     - Name
     - Date of birth
     - Mother's maiden name
     - Biometric data

3. **PHI (Protected Health Information)**
   - Health-related information about an individual, including:
     - Health status
     - Healthcare records
     - Payments for healthcare services

4. **Sensitive Data**
   - Data that includes intellectual property, PII, and PHI. This data is particularly sensitive and requires additional security measures.

5. **Confidential Data**
   - Very sensitive data that requires approval to access. May include trade secrets or internal business processes that are critical to the organization’s success.

6. **Public / Unclassified Data**
   - Data that is freely accessible to the public without restrictions.

7. **Private / Classified / Restricted Data**
   - Data with restricted access, often requiring a non-disclosure agreement (NDA) or other formal agreements for access.

8. **Critical Data**
   - Data essential to the organization's operations and business continuity. Critical data requires the highest level of security and ensures 100% availability whenever needed.

# 3.3 States of Data

### Data at Rest
- Refers to data stored on a storage device such as an HDD, SSD, or Flash Drive.
- **Security Measures**:
  - **Encryption**: Apply whole disk encryption, database encryption, or file/folder-level encryption to protect the data when not in use.
  - **Permissions**: Use access control lists (ACLs) to restrict access, ensuring only authorized users can access the data.

### Data in Transit
- Refers to data being transmitted over a network or data in motion, traveling through switches, routers, and other devices.
- **Risks**: Data can be intercepted by attackers during transit if not adequately protected.
- **Security Measures**:
  - **Network-based Protection**: Firewalls and Intrusion Prevention Systems (IPS) can help monitor and control traffic.
  - **Encryption**: Use transport encryption protocols such as TLS (Transport Layer Security) or IPsec (Internet Protocol Security) to secure data in transit.

### Data in Use
- Refers to data actively being processed in system memory, including RAM, CPU registers, and cache.
- **Risks**: Data in use is often decrypted for processing, making it vulnerable to attackers who may extract it from memory.
- **Security Measures**:
  - **Memory Protection**: Tools to protect data in memory, such as encryption in use or sandboxing, can reduce exposure.

### Data Sovereignty
- Refers to the legal implications of where data is stored and processed based on the country it resides in.
- **Laws**: Different countries have laws that govern how data is handled, and data must comply with the laws of the country where it is stored.
  - **Example**: Under GDPR, data collected on EU citizens must be stored within the EU.
- **Implications**: Compliance with local data protection laws may restrict where data can be stored or processed.

### Geolocation
- Refers to the physical location of data and users.
- **Location Tracking**: Various technologies like 802.11 (Wi-Fi), GPS, and mobile provider data can be used to determine the location of data or users.
- **Security Measures**:
  - **Access Control**: Geolocation can help manage access to data, restricting access based on location, such as preventing access from unauthorized regions or allowing administrative access only within secure zones.

# 3.3 Protecting Data

### Geographic Restrictions
- Refers to controlling access based on the network location of the user.
  - **Identification**: Identifying the location via IP subnet or geolocation.
  - **Challenges**: Mobile devices can make it difficult to pinpoint location, but GPS and 802.11 wireless are highly accurate methods.
  - **IP Address**: Less reliable, as it’s harder to track the physical location of a user accurately through IP.

### Geofencing
- **Definition**: A technology that automatically restricts or allows access based on the user's geographical location.
  - **Example**: Restricting access to an app unless the user is near a specific location, such as an office.
  
### Protecting Data
- **Primary Goal**: Protecting data, which exists in many forms across storage drives, networks, CPUs, memory, etc.
  - **Methods**: 
    - Encryption
    - Security policies
    - Data permissions, ensuring that only authorized users can access sensitive data.

### Encryption
- **Definition**: Converts plaintext (cleartext) into unreadable ciphertext.
  - **Process**: Requires a decryption key to revert ciphertext back to plaintext.
  - **Goal**: Secure data from unauthorized access by making it unreadable without the correct decryption key.
  
### Hashing
- **Definition**: A method for representing data as a short string (hash), which is a one-way process.
  - **Uses**: 
    - Store passwords securely.
    - Verify the integrity of data (e.g., checking if a downloaded document matches the original).
    - Often used for non-repudiation, digital signatures, and ensuring data integrity.
  - **Characteristics**: Hashing is collision-resistant, meaning that two different inputs won’t produce the same hash.

### Obfuscation
- **Definition**: Making understandable data difficult to interpret.
  - **Purpose**: Helps obscure the inner workings of a system, preventing attackers from easily identifying security vulnerabilities.
  - **Note**: Though it adds complexity, it doesn’t make it impossible for attackers to reverse the obfuscation.

### Masking
- **Definition**: Hiding part of the original data to protect sensitive information.
  - **Example**: Masking a Social Security Number (SSN) or credit card number.
  - **Consideration**: Data may still be intact in storage, but its full visibility is restricted based on permissions.
  - **Techniques**: Substitution, shuffling, encryption, or partial data removal.

### Tokenisation
- **Definition**: Replacing sensitive data with a placeholder that has no direct value.
  - **Example**: Replacing a credit card number with a temporary token during transactions.
  - **Benefit**: Even if an attacker captures the token, it cannot be used outside the specific context where it was generated.
  - **Difference**: Unlike encryption or hashing, tokenisation doesn’t transform the original data, but rather substitutes it with a non-sensitive placeholder.

### Segmentation
- **Definition**: Dividing a network or system into isolated segments to enhance security, performance, and simplify management.
  - **Benefit**: By splitting data into smaller, isolated sections, attackers have to breach multiple segments to access all the data, making attacks more difficult.
  - **Best Practice**: Sensitive data should be highly segmented and have the strongest security measures in place.

### Permission Restrictions
- **Definition**: Controlling access to data and systems based on user accounts and permissions.
  - **Process**:
    - During account creation or management, rights and permissions are set.
    - Ensure users only have access to data they are authorized to view or modify.
    - Authentication methods like password policies and multi-factor authentication (MFA) act as another layer of defense.

# 3.4 Resiliency

### High Availability
- **Definition**: Systems that are designed to be "always on" and continuously available, minimizing downtime.
  - **Components**: Typically involves multiple components working together, with **active/active** configurations providing scalability and better resource distribution.
  - **Cost**: Achieving higher availability often involves higher costs, as additional resources and redundancy are necessary.

### Server Clustering
- **Definition**: Combining two or more servers to operate as a single larger server, presenting a unified service to users.
  - **Benefits**:
    - Increased capacity and availability.
    - Often managed and configured at the OS level.
    - Devices in the cluster typically use the same OS for consistency.

![image](https://github.com/user-attachments/assets/1e0e15d5-7873-46ee-a2f9-f234ad8a418c)

  
### Load Balancing
- **Definition**: A device or software that distributes incoming network traffic across multiple servers, ensuring no single server is overwhelmed.
  - **Flexibility**: The servers behind the load balancer may run different operating systems.
  - **Scalability**: The load balancer dynamically adjusts the number of active servers by adding or removing them based on demand and server availability.

### Site Resiliency
- **Definition**: The ability of IT infrastructure, systems, and applications to operate smoothly or recover quickly from disruptions.
  - **Disruptions**: Can include hardware failures, power outages, natural disasters, or cyber-attacks.
  - **Redundancy**: Allows for recovery by switching to alternate sites or servers if the primary site fails.

### Types of Recovery Sites:
- **Hot Site**: 
  - An exact replica of your data center, including hardware and systems, which is kept continuously synchronized.
  - **Benefit**: Instant failover with minimal downtime.
  - **Drawback**: Very costly since you duplicate everything.
  
- **Cold Site**: 
  - A basic site with no infrastructure; it can be built up as needed.
  - **Benefit**: Least expensive, but requires time and effort to bring online.
  
- **Warm Site**: 
  - A middle ground, containing partial infrastructure like empty racks or minimal hardware.
  - **Benefit**: Faster recovery than a cold site, but still less costly than a hot site.

### Geographic Dispersion
- **Definition**: Deploying infrastructure in multiple physical locations away from the primary site.
  - **Risk Mitigation**: Helps ensure operations continue in the event of a natural disaster, such as hurricanes, floods, or tornadoes.
  - **Challenge**: Logistical challenges, including transporting equipment and moving employees to the backup site, can make geographic dispersion difficult to manage.

### Platform Diversity
- **Definition**: The use of multiple operating systems to reduce vulnerability risks.
  - **Benefit**: Different OS vulnerabilities (e.g., Windows vs. Linux) don't usually affect each other, thus reducing exposure to single-platform threats.
  - **Drawback**: Increases the attack surface by adding more platforms, which can also complicate system management and security.

### Multi-cloud Systems
- **Definition**: Using multiple cloud service providers (e.g., AWS, Microsoft Azure, Google Cloud) to host data and applications.
  - **Benefit**: Geographic and service provider diversification ensures that an outage with one provider doesn’t affect operations with others.
  - **Consideration**: You must plan for cloud outages and ensure that data is sufficiently distributed across different regions and providers.

### Continuity of Operations Planning (COOP)
- **Definition**: Planning and preparing to continue essential functions during emergencies, such as natural disasters, cyber-attacks, or pandemics.
  - **Examples**: Having manual processes (e.g., paper records, phone transactions) in place for when technology fails.
  - **Key Requirement**: COOP plans must be documented and regularly tested to ensure they are effective during disruptions.

# 3.4 Capacity Planning

### Balanced Approach for Capacity Demand
Capacity planning requires finding a balance between people, technology, and infrastructure to ensure the organization can meet demand efficiently and effectively.

### People
- Some services require human intervention to operate properly, such as:
  - **Call center support lines**
  - **Technology services**
  
- **Challenges**:
  - **Too few employees**: Can lead to delays in service or response times.
    - **Solution**: Recruit new staff, though this can be time-consuming.
  - **Too many employees**: Can lead to inefficiency and increased operational costs.
    - **Solution**: Redeploy employees to other parts of the organization or downsize.

### Technologies
- **Scalability**: Choose technologies that can scale up or down based on demand.
  - **Web services**: 
    - Distribute load across multiple services to manage high traffic volumes.
  - **Database services**: 
    - **Clustering** multiple SQL servers to improve performance.
    - **Database partitioning** to increase capacity and reduce strain on individual systems.
  - **Cloud services**: 
    - Provide **on-demand scalability**.
    - Offer seemingly unlimited resources, depending on payment and usage.

### Infrastructure
- Infrastructure includes all physical and cloud-based resources necessary for the organization’s operations, such as:
  - **Application servers**
  - **Network services**
  - **CPU, network, and storage devices**

#### Physical Devices
- **Challenges**: Requires significant investment in purchasing, configuring, and installing physical hardware.
  
#### Cloud-Based Devices
- **Benefits**: 
  - Easier and quicker to deploy.
  - Adaptable for sudden and unexpected capacity increases.
  - Offer flexibility with resources that can be scaled up or down based on current demand.

# 3.4 Recovery Testing

### Importance of Testing Before an Actual Event
Testing your recovery procedures and infrastructure before an actual event helps ensure the effectiveness of your plan. It is crucial to:
- **Schedule regular update sessions**: Annual or semi-annual tests.
- **Define specific rules of engagement**: Establish clear guidelines to follow during the test.
- **Use realistic scenarios**: Create scenarios with limited time to assess the team's response.
- **Evaluate and document**: Analyze the response, identify areas for improvement, and discuss lessons learned.

### Tabletop Exercise (TTX)
A **discussion-based simulation** used to assess and improve organizational preparedness for emergency situations.
- **Benefits**:
  - Improved **preparedness** for real incidents.
  - Enhanced **coordination** among teams.
  - **Identification of gaps** in processes and systems.
  - Increased **training and awareness** across the organization.
  - Boosted **confidence** in handling emergencies.

### Failover Testing
Failover testing evaluates whether redundant configurations can successfully take over if a failure occurs.
- **Process**:
  - The **failover** happens automatically, with users being redirected to alternative resources.
  - **Redundant infrastructure** is created and implemented to ensure minimal disruption during failures.

### Simulation Testing
Simulation tests assess the organization's security by replicating real-world attack scenarios.
- **Examples**:
  - **Phishing attacks**.
  - **Password requests**.
  - **Data breaches**.

### Phishing Simulations
- **Create and send phishing emails** to the organization's user community.
- **Objective**: Assess internal security (e.g., Did the email filters block it?).
- **Test users**: See who clicks on the phishing link and require additional training for those who fall for it.

### Parallel Processing
**Parallel processing** involves using multiple CPUs to perform tasks simultaneously.
- **Use Cases**:
  - A **single computer with multiple CPU cores** or multiple physical CPUs.
  - **Multiple computers** working together on complex tasks.
  
- **Benefits**:
  - **Improved performance** by splitting complex tasks across processors.
  - **Improved recovery**: Quickly identify faulty systems and remove them from the processing pool while continuing operations with the remaining functional processors.

# 3.4 Backups

### Importance of Backups
Backups are crucial for recovering important and valuable data in case of disasters. Proper planning is necessary to ensure that critical data is regularly backed up and can be quickly restored when needed.

### Types of Backup Implementations
Backups vary based on several factors:
- **Total amount of data** to be backed up.
- **Type of backup** (full, incremental, differential).
- **Backup media** (disk, tape, cloud).
- **Storage location** (onsite, offsite).
- **Backup and recovery software** used to manage the process.
- **Frequency of backups** (daily, weekly, or hourly).

### Onsite Backup
- **Advantages**:
  - No internet connection required.
  - Data is immediately available for recovery.
  - Generally less expensive than offsite backups.
  
### Offsite Backup
- **Advantages**:
  - Data is transferred over the internet or WAN link.
  - Data is available for recovery after a disaster, even if onsite systems are compromised.
  - Restoration can occur from anywhere.

Many organizations use both onsite and offsite backups to ensure redundancy.

### Backup Frequency
The frequency of backups depends on the nature of the data:
- **Systems with low change frequency** might only need weekly backups.
- **High-change systems** may require hourly or daily backups.
- Organizations often maintain **multiple backup sets** (daily, weekly, monthly) for different types of data.
- Managing a large number of backup sets requires **significant planning**.

### Backup Encryption
Encryption ensures that backup data, particularly offsite backups, is protected against unauthorized access.
- **Important for cloud backups** to prevent eavesdropping.
- A **recovery key** is required to restore encrypted backups.

### Snapshots
Snapshots provide an efficient way to back up entire systems with a single operation:
- A snapshot is a **point-in-time copy** of a system's configuration and data.
- **Daily snapshots** may contain only changes from the previous snapshot, allowing fast recovery.
- Users can **revert to any snapshot** for quick restoration.

### Recovery Testing
Regularly testing backups is essential to confirm that data can be restored successfully:
- **Disaster recovery testing** simulates a real disaster and ensures backups can be restored.
- **Periodic audits** are necessary to maintain the integrity of backup systems.

### Replication
Replication involves creating a copy of data at multiple locations in real-time:
- **Real-time backup** ensures that data is always synchronized across locations.
- Useful for ensuring **availability and disaster recovery**.
- Data can be replicated to **remote sites**, providing redundancy in case of a disaster.

### Journaling
Journaling is used to ensure data consistency and integrity, especially in file systems and databases:
- A **journal log** records changes made to the data before they are written to storage.
- **Power outages** or interruptions during writes can result in corrupted data, but journaling helps recover to a usable state.
- **Journal entries** are updated before and after data is written to storage, ensuring a consistent state.

# 3.5 Power Resiliency

### Importance of Power Resiliency
Power is a critical foundation for all technological systems, and planning for power outages is essential for ensuring continuous operations. Since power is typically provided by third-party providers, it’s not always possible to control availability. However, several strategies can mitigate the impact of power issues.

### Types of Power Issues
- **Short Power Outages**: These are brief interruptions that can be addressed with short-term backup solutions.
- **Long-Term Power Issues**: Extended outages may require more robust and long-term power solutions to maintain operations.

### Uninterruptible Power Supply (UPS)
A UPS provides short-term backup power during outages, helping to prevent data loss and system shutdowns:
- **Functions**:
  - Protects against blackouts, brownouts, and power surges.
  - Provides enough time to safely shut down systems during an outage.

#### Types of UPS
1. **Offline/Standby UPS**: Provides basic backup, activating only when power failure is detected.
2. **Line-interactive UPS**: Provides more stable power by adjusting voltage fluctuations while offering backup power.
3. **On-line/Double-conversion UPS**: Offers the highest level of protection by continuously converting power, providing clean and stable electricity even during power disruptions.

#### UPS Features
- **Auto Shutdown**: Automatically shuts down systems to prevent damage when power is lost.
- **Battery Capacity**: Determines how long the UPS can supply power to devices.
- **Outlets**: The number of devices the UPS can support.
- **Phone Line Suppression**: Protects against surges in phone lines.

### Generators
Generators provide long-term power backup, allowing systems to remain operational during extended power outages:
- **Fuel Storage Required**: Generators require fuel to operate, which must be stored and maintained.
- **Full-Building Power**: Can power an entire building or specific areas, with outlets marked for generator use.
- **Start-up Time**: Generators may take a few minutes to start up; during this time, a UPS can be used to keep systems running until the generator is fully operational.
</details>

<details><summary>4.0 Security Operations</summary>

# 4.1 Secure Baselines

### Definition of Secure Baselines
Secure baselines define the security configurations that must be consistently applied across an application environment to ensure its integrity and protection. These baselines cover essential security aspects like:
- Firewall settings
- Patch levels
- OS file versions
- Other critical configuration settings

All application instances within the environment must adhere to these baselines to maintain security. Regular updates are required to ensure the baselines remain relevant and secure.

### Integrity Measurements
To ensure that systems remain secure, regular checks should be performed to compare the current state of the system against the established baselines. These checks help identify deviations that may indicate security issues.
- These integrity checks should be frequent to catch any misconfigurations or vulnerabilities early.
- Any failure to meet the baseline requirements should result in immediate correction actions.

### Establishing Baselines
To create a secure baseline, organizations can use a combination of security policies and standard configurations retrieved from trusted sources such as:
- Application developers
- Operating system vendors
- Appliance manufacturers

Operating systems, like Windows, provide a wealth of configuration options to support baseline security, such as over 3,000 group policy settings in Windows 10. Additionally, tools like the **Microsoft Security Compliance Toolkit** help automate the process of setting and enforcing these baselines.

### Deploying Baselines
Once the security settings are defined, they must be deployed across all components within the network environment. This typically involves:
- Centralized management via a console, such as Active Directory or Mobile Device Management (MDM) systems.
- Automation to ensure that settings are consistently applied to many devices, reducing human error and ensuring scalability.

### Maintaining Baselines
While many baseline settings are static and rarely change, they need to be maintained and updated to account for:
- Newly discovered vulnerabilities
- Updates to applications or operating systems
- New installations or hardware deployments

As environments evolve, it's important to test and measure to ensure that updates or changes to baselines do not conflict with other security configurations. Balancing multiple baselines in complex environments can sometimes lead to conflicts, so careful management and testing are essential to ensure the overall integrity and security of the system.

# 4.1 Hardening Targets

### Importance of Hardening
No system is secure with default configurations. Hardening is essential to ensure that software and hardware are configured to minimize vulnerabilities. Hardening guidelines are often specific to the software or platform, and manufacturers can provide the best details for securing their systems.

### Mobile Devices
Mobile devices, such as smartphones and tablets, require dedicated hardening:
- **Updates**: Ensure regular updates, including bug fixes and security patches, to address known vulnerabilities.
- **Segmentation**: Separate company and user data to protect sensitive information.
- **Mobile Device Management (MDM)**: Implement MDM solutions to manage and control mobile devices effectively.

### Workstations (Desktops, Laptops, etc.)
For workstations, continuous monitoring and updates are critical:
- **Automated Patching**: Automate monthly patches for operating systems, applications, and firmware to keep systems up to date.
- **Remove Unnecessary Software**: Eliminate unused or unnecessary software to reduce the attack surface and limit vulnerabilities.

### Network Infrastructure Devices (Switches, Routers, etc.)
Network infrastructure devices, such as switches and routers, need specific hardening measures:
- **Authentication Configuration**: Ensure proper authentication is set up, avoiding the use of default credentials.
- **Manufacturer Guidance**: Regularly check for security updates from the manufacturer, as these devices may not receive frequent updates, but they are critical for securing the network.

### Cloud Infrastructure
Securing cloud infrastructure involves controlling the cloud management workstation and services:
- **Least Privilege**: Apply the principle of least privilege to limit user and application access, ensuring only the necessary permissions are granted.
- **Endpoint Detection and Response (EDR)**: Set up EDR to monitor for potential attacks and ensure that it's regularly updated.
- **Backup**: Implement Cloud-to-Cloud (C2C) backups for disaster recovery and data protection.

### Servers (Windows, Linux, etc.)
Servers need robust hardening practices:
- **Regular Updates**: Apply operating system updates, service packs, and security patches promptly.
- **User Account Management**: Enforce minimum password lengths, complexity requirements, and account limitations to follow the principle of least privilege.
- **Network Access Control**: Limit network access to essential services only.
- **Security Tools**: Implement EDR, anti-malware, anti-virus, and client-based security technologies to protect against threats.

### SCADA/ICS (Supervisory Control and Data Acquisition Systems)
SCADA systems manage large-scale industrial processes and require specialized hardening:
- **Extensive Segmentation**: Segment the network to prevent unauthorized access, ensuring that SCADA systems are isolated from other networks.
- **No External Access**: Restrict access from outside the organization to protect against cyber threats.

### Embedded Systems
Embedded systems, such as smart appliances and wearables, need secure configurations:
- **Patch Vulnerabilities**: Apply security patches to address vulnerabilities and remove potential threats.
- **Network Segmentation**: Use segmentation and firewalls to prevent unauthorized access, as these systems are often vulnerable.

### Real-Time Operating Systems (RTOS)
RTOS, which have deterministic processing schedules, require isolation and hardening:
- **System Isolation**: Prevent access from other areas of the network to isolate the system.
- **Minimize Services**: Run only the minimum number of services to reduce the potential for exploitation.
- **Secure Communication**: Use secure communication protocols and host-based firewalls to protect the system.

### IoT Devices
IoT devices, including HVAC, lighting, and wearable technology, present significant security risks:
- **Change Default Passwords**: Manufacturers of IoT devices may not prioritize security, so changing default passwords is crucial.
- **Timely Updates**: Apply updates quickly to address security concerns and vulnerabilities in IoT devices.

# 4.1 Securing Wireless and Mobile

### Site Surveys
Determine existing wireless landscape, sample with existing wireless spectrum.
- Identify existing access points
- Work around existing frequencies, layout and plan for interference
- Plan for ongoing site surveys, things will change
- Heat maps, identify wireless signal strengths

![image](https://github.com/user-attachments/assets/26066874-4960-43a6-9988-de46196dfcb6)


### Wireless Survey Tools
- Signal coverage
- Potential interference
- Built-in tools
- 3rd party tools
- Spectrum analyser, will show you all signals on a particular frequency

![image](https://github.com/user-attachments/assets/ca7504a6-22f3-4f26-9e8d-24f2bab3773d)

### Mobile Device Management (MDM)
Manage company-owned and user-owned mobile devices. BYOD - Bring your own Device
- Centralised management of the mobile devices, specialised functionality
- Set policies on apps, data, camera, etc.
- Control the remote device, the entire device or a "partition"
- Manage access controls, force screen locks and PINs on these single-user devices

### BYOD: Bring your own Device (Bring your own Technology)
- Employees' devices need to meet the company's requirements
- Difficult to secure, it's both a home device and a work device
- How is data protected? What happens to the data when a device is sold or traded in?

### COPE: Corporate owned, personally enabled
- Company buys the device
- Used as both a corporate device and a personal device
- Organisations keep full control of the device, similar to company-owned laptops and desktops
- Information is protected using corporate policies, information can be deleted at any time.
- CYOD - Choose your own Device, similar to COPE, but with the user's choice of device.

### Cellular Networks
Mobile devices, "cell" phones, 4G, 5G
- Separate land into "cells", antenna coverage a cell with certain frequencies
- Security concern, traffic monitoring, location tracking, worldwide access to a mobile device
- Wi-Fi, local network access, local security problems
- Same security concerns as other Wi-Fi devices
- Data capture, encrypt your data.
- On-path attack (MitM), modify and/or monitor your data
- DoS attack, frequency interference

### Bluetooth
High-speed communication over short distances, PAN (Personal Area Network)
- Connects to our mobile devices, smartphones, tethering, etc.
- Do not connect to unknown Bluetooth devices

# 4.1 Wireless Security Settings

### Authentication
An organization's wireless network can contain confidential information.
- Authenticate users before granting access
- Username, password, MFA
- Ensure all communication is confidential, encrypt all wireless data
- Verify the integrity of all communication, a Message Integrity Check (MIC)

### The WPA2 PSK Problem
WPA2 has a PSK brute-force problem.
- Four-way handshake
- Capture the hash
- With the hash, attackers can brute force the pre-shared key (PSK)
- A weak PSK is easy to brute force due to GPU processing speeds and cloud-based password cracking.

### WPA3 and GCMP
Wi-Fi Protected Access 3 (WPA3), 2018
- **GCMP**: Galois/Counter Mode Protocol, stronger encryption than WPA2
- **Security Services**:
  - Data confidentiality with **AES**
  - Message Integrity Check (MIC) with **Galois Message Authentication Code (GMAC)**

### Simultaneous Authentication of Equals (SAE)
WPA3 changes the PSK authentication process.
- Mutual authentication
- Creates a shared session key without sending that key across the network
- No more four-way handshake, no hashes, no brute force attacks
- A Diffie-Hellman derived key exchange with an authentication component
- Everyone uses a different session key, even with the same PSK
- An IEEE standard - the **dragonfly handshake**

### Wireless Authentication Methods
Gain access to a wireless network, mobile users, temporary users.
- **Credentials**: Shared password/pre-shared key (wireless password)
- **Centralised Authentication** (802.1X)

### Wireless Security Modes
Configure the authentication on your wireless access point / wireless router
- **Open System**:
  - No authentication password is required
- **WPA3-Personal / WPA3-PSK**:
  - WPA2 or WPA3 with a pre-shared key
  - Everyone uses the same 256-bit key
- **WPA3-Enterprise / WPA3-802.1X**:
  - Authenticate users individually with an authentication server (e.g., RADIUS)

### AAA Framework
- **Identification**: This is who you claim to be, usually your username
- **Authentication**: Prove who you say you are, password and other authentication factors
- **Authorization**: Based on your identification and authentication, what access do you have?
- **Accounting**: Resources used, login time, data sent and received, logout time (Logs)

![image](https://github.com/user-attachments/assets/27970461-7bef-46cb-b502-17c5733b4a20)

### RADIUS (Remote Authentication Dial-in User Service)
One of the more common AAA protocols.
- Supported on a wide variety of platforms and devices
- Centralizes authentication for users, routers, switches, firewalls, server authentication, remote VPN access, 802.1X network access
- RADIUS services available on almost any server operating system

### IEEE 802.1X
Port-based Network Access Control (NAC). You don't get access to the network until you authenticate.
- Used in conjunction with an access database such as: **RADIUS**, **LDAP**, **TACACS+**

### EAP (Extensible Authentication Protocol)
An authentication framework, used to embed the authentication within the 802.1X process.
- Many different ways to authenticate based on **RFC** standards, manufacturers can build their own EAP methods.

# 4.1 Application Security

### Secure Coding Concepts
A balance between time and quality, programming with security in mind is often secondary.
- **Testing**: Quality assurance (QA) process, functionality + security checks
- Vulnerabilities will eventually be found and exploited

### Input Validation
What is the expected input?
- Validate actual vs expected
- Document all input methods, forms, fields, types
- Check and correct all input (normalization), a zip code should only be X characters
- Fix any data with improper input
- The fuzzers will find what you missed

### Secure Cookies
Cookies are small bits of information stored on your browser that contain tracking information for sites you visit, personalize information shown on a web page, or manage sessions.
- Not executable, not generally a security risk unless someone gets access to them
- **Secure cookies**: Have a secure attribute set, browser will only send them over HTTPS
- Sensitive information should not be saved in a cookie, as this isn't designed to be secure storage

### Static Code Analyzer
Static Application Security Testing (SAST), helps identify security flaws.
- Many vulnerabilities found easily: buffer overflows, database injections, etc.
- Not all security concerns can be found using this method, such as authentication security, insecure cryptography, etc.
- **Verify** each finding, as false positives are common

### Code Signing
A process used to digitally sign software or code to verify its authenticity and integrity. The owner applies a digital signature to the code using a cryptographic algorithm.
- **Asymmetric Encryption**: A trusted **CA** signs the developer's public key
- Developer signs the code with their private key
- For internal apps, use your own **CA**

### Sandboxing
Applications cannot access unrelated resources; they play in their own sandbox.
- Commonly used during development, can be a useful production technique
- Virtual machines, mobile devices, browser inline frames, windows user account control (UAC)

### Application Security Monitoring
Real-time information on application usage, access demographics.
- View blocked accounts, SQL injection attempts, patched vulnerabilities
- **Audit logs**: Find the information gathering and hidden attacks
- **Anomaly detection**: Unusual file transfers, increase in client access

# 4.2 Asset Management

### Acquisition/Procurement Process
Starts with a request from a user.
- A multi-step process for requesting and obtaining goods and services
- Includes budget information and formal approvals
- Negotiate with suppliers, terms, and conditions
- Purchase, invoice, and payment

### Assignment/Accounting
A central asset tracking system.
- **Ownership**: Associate a person with an asset, useful for tracking a system
- **Classification**: Type of asset, hardware (capital expenditure), software (operating expenditure)

### Monitoring/Asset Tracking
Inventory every asset.
- **Laptops, desktops, servers, routers, switches**, etc.
- Associate a support ticket with a device make and model, can be more detailed than a user's description
- **Enumeration**: Lists all parts of an asset, CPU, memory, storage device, keyboard, mouse, etc.
- Add an asset tag, barcode, RFID, or visible tracking number with the organization name

### Media Sanitization
System disposal or decommissioning.
- Completely remove data
- No usable information remains
- Clean hard drive for future use
- Permanently delete a single file
- Use a utility that can securely delete or remove files, no way to recover using forensic tools
- Reuse the storage media to save costs

### Physical Destruction
- **Shredder/pulverizer**: Heavy machinery for complete destruction
- **Drill/hammer**: Quick and easy physical destruction
- **Electromagnetic (degaussing)**: Removes the magnetic field, destroys hard drive data and renders it unusable

### Certificate of Destruction
Destruction is often done by a third party.
- Service will include a **certificate of destruction**
- A paper trail of broken data

### Data Retention
Backup your data: how much and where? Copies, versions of copies, lifecycle of data, purging old data.
- **Regulatory compliance**: A certain amount of data backup may be required
- Emails, corporate financial data
- **Operational needs**: Accidental deletion, disaster recovery
- Differentiate by type and application, recover the data you need and when you need it

# 4.3 Vulnerability Scanning

### Vulnerability Scanning
Used to determine if a system is susceptible to an attack.
- **Usually minimally invasive**
- Checks if there's potential for an attack, such as a **port scan**
- Identify systems and security devices
- Test from the outside and inside, don't dismiss insider threats
- Vulnerability scans gather a large amount of data, not everything in it is always accurate

### Static Code Analyzers
Identify security flaws.
- **Buffer overflows**
- **Database injections**
- **Authentication security, insecure cryptography**, etc., won't be identified by a static code analyzer
- **False positives** may occur

### Dynamic Analysis (Fuzzing)
Takes random input and puts it into an application to see what happens.
- **Fault injecting**, robustness testing, syntax testing, etc.
- Looking for something out of the ordinary, such as application crashes, server errors, exceptions, etc.

### Fuzzing Engine and Frameworks
Platform-specific, language-specific, etc.
- **Very time and processor heavy**

### Package Monitoring
The process of continually tracking and analyzing software packages, libraries, or dependencies used within an application or system.
- Downloaded from a trusted source or third party?
- Confirm the package is **legitimate**
- No added **malware** or embedded vulnerabilities
- Confirm a safe package before deployment, like on a **sandbox**

# 4.3 Threat Intelligence

### Threat Intelligence
I.T. Professionals will be expected to keep up to date with all the latest threats that could be affecting your organisation. Research the threats and threat actors.
- **Hacker group profiles**, tools used by the attackers, and much more
- Make a decision based on this intelligence, **invest in the best prevention**
- Used by researchers, security operations teams, and others

### Open-source Intelligence (OSINT)
Information available to anyone, you just need to know where to find it.
- **Publicly available sources**
- A good place to start
- **Internet**, discussion groups, social media
- **Government data**, mostly public hearings, reports, websites, etc.
- **Commercial data**, maps, financial reports, databases
- **Newsletters**, tl;dr and more

### Proprietary/Third-party Intelligence
Someone else has already compiled the threat information, and you can buy it.
- **Threat intelligence services**, threat analytics, correlation across different data sources
- **Constant threat monitoring**, identify new threats, create automated prevention workflows

### Information-sharing Organisations
- **Public threat intelligence**, often classified information made public
- **Private threat intelligence**, extensive resources
- Need to share critical security details, **real-time, high-quality cyber threat information sharing**

### Cyber Threat Alliance (CTA)
Members upload specifically formatted threat intelligence, CTA scores each submission and validates it across other submissions. Other members can extract the data.

### Dark Web Intelligence
Overlay networks that use the internet, requiring specific software and configurations to access.
- **Hacking groups and services**, activities
- **Tools and techniques**, credit card sales, accounts, and passwords
- Monitor forums for activity

# 4.3 Penetration Testing

### Simulate an attack on our own systems
Similar to vulnerability scanning except we actually try to exploit the vulnerabilities, rather than just look for them.
- Often a compliance mandate, **regular penetration testing by a 3rd-party**.
- NIST - Technical Guide to Information security testing and assessment ([NIST SP 800-115](https://www.nist.gov/privacy-framework/nist-sp-800-115))

### Rules of Engagement
A formal list of rules so that everyone knows the scope and the purpose of the testing.
- When penetration testing is allowed, on-site physical breach, internal test, external test, etc.
- Normal working hours or after 6 PM only, etc.
- The rules: **IP address ranges**, emergency contacts, how to handle sensitive information, **in-scope and out-of-scope** devices or applications.

### Exploiting Vulnerabilities
Try to break into the system, this can cause a **denial of service** or **loss of data**.
- **Buffer overflow** can cause instability
- **Gain privilege escalation**
- You may need to try many different vulnerability types: **Password brute-force**, **social engineering**, **database injections**, **buffer overflows**.

### The Process
1. **Initial exploitation**, getting into the network
2. **Lateral movement**, move from system to system, the inside of the network is relatively unprotected
3. **Persistence**, once you're there, you need to make sure there's a way back in, set up a backdoor, build user accounts, change or verify default passwords
4. **The pivot**, gain access to systems that would normally not be accessible, use a vulnerable system as a proxy or relay

### Responsible Disclosure Program
It takes time to fix a vulnerability.
- Software changes, testing, deployment, etc.
- **Bug bounty programs**, a reward for discovering vulnerabilities, earn money for hacking a system, document the vulnerability and earn cash.
- A controlled information release: researcher reports the vulnerability, manufacturer creates a fix, the vulnerability is announced publicly.

# 4.3 Analysing Vulnerabilities

### Dealing with False Information
- **False positives**: A vulnerability identified that doesn't really exist.
  - Different from a low-severity vulnerability.
- **False negatives**: A vulnerability exists but was not detected.
- **Update to the latest signatures before scanning**.
- Work with the vulnerability detection manufacturer, they may need to update their signatures.

### Prioritising Vulnerabilities
- Some vulnerabilities may not be significant, while others could be critical.
- This may be difficult to determine.
- **Refer to public disclosures and vulnerability databases**, the industry is well versed in tracking vulnerabilities.

### CVSS: Common Vulnerability Scoring System
- Quantitative scoring of vulnerabilities, ranging from **0 to 10**.
- The scoring standards change over time.
- Different scoring for **CVSS 2.0** vs **CVSS 3.x**.
- Industry collaboration, enhanced feed sharing, and automation.

### CVE: Cross-referencing Vulnerabilities
- Vulnerabilities can be cross-referenced online; most scanners provide a place to go.
  - National vulnerability database: [http://nvd.nist.gov/](http://nvd.nist.gov/)
  - Common Vulnerabilities and Exposure: [https://cve.mitr.org/cve/](https://cve.mitr.org/cve/)
  - Microsoft security bulletins: [http://www.microsoft.com/technet/security/current.aspx](http://www.microsoft.com/technet/security/current.aspx)

### Manual Checks for Certain Vulnerabilities
- Some vulnerabilities cannot be definitively identified, requiring manual checks to confirm.
- Scanners will give a heads-up about these vulnerabilities.

### Vulnerability Classifications
- **Application Scans**: Desktops, mobile apps.
- **Web application scans**: Software on a web server.
- **Network scans**: Misconfigured firewalls, open ports, vulnerable devices.

### Exposure Factor
- The **loss of value** or business activity if the vulnerability is exploited, usually expressed as a percentage.
  - A small **DDoS** may limit access to a service (50% exposure factor).
  - A **buffer overflow** may completely disable a service (100% exposure factor).
- A key consideration when prioritising; the worst possible outcome should probably be addressed first.

### Environmental Variables
- What type of environment is associated with this vulnerability?
  - Prioritising and patching frequency: Is it in an isolated test lab or a database server in the public cloud?
  - The environment's number and type of users (internal or external), revenue-generating applications, potential for exploitation, and ease of solutions can all affect prioritisation.

### Industry/Organisational Impact
- Some exploits have significant consequences, making the type of organisation an important consideration.
  - **Example**: Tallahassee Memorial HealthCare, which was hit by ransomware, closed for two weeks, diverting emergency cases and cancelling surgeries.

### Risk Tolerance
- The amount of risk acceptable to an organisation.
  - **Timing of security patches**: Patching needs to be tested before being applied.
  - Testing takes time, leaving systems vulnerable during the testing phase.

# 4.3 Vulnerability Remediation

### Patching
- An update or piece of code released by software vendors to fix vulnerabilities, bugs, or security flaws in their software or operating systems.
  - **The most common mitigation technique**.
  - Scheduled vulnerability/patch notes are typically released monthly or quarterly.
  - **Unscheduled patches** address zero-day vulnerabilities and often require urgent attention.
  - This is an ongoing process, as patches keep coming. It's an **easy way to prevent most exploits**.

### Insurance
- **Cybersecurity insurance coverage**: Executed after an event occurs to cover revenue losses or data recovery costs.
  - **Examples of coverage**:
    - Money lost to phishing.
    - Privacy lawsuit costs.
  - **Exclusions**:
    - Does not cover intentional acts, funds transfers, or certain types of attacks (e.g., ransomware).
  - The increasing popularity of **ransomware** has driven growth in cybersecurity liability insurance.

### Segmentation
- A technique used to **isolate different parts of a network** or system for security.
  - Limits the scope of an exploit, ensuring that a breach only gives attackers access to the segment they manage to infiltrate.
  - If quick patching is not possible, **disconnect or turn off** the infected segment.
  - Use **internal Next-Generation Firewalls (NGFWs)** to block unwanted traffic between VLANs and identify malicious traffic inside the network.

### Physical Segmentation
- The use of **separate devices** or infrastructure to create security boundaries.
  - **VLANs** allow for logical segmentation of devices on the same hardware.

### Compensating Controls
- Optimal security methods may not always be available, so compensatory methods are used.
  - **Examples**: If you cannot deploy a patch right now or lack internal firewalls, consider:
    - Disabling the problematic service.
    - Revoking access to the affected application.
    - Limiting external access or modifying internal security controls (software or firewalls).
  - **Compensating controls** provide coverage until a patch can be deployed or similar optimal security measures are implemented.

### Exceptions and Exemptions
- While removing the vulnerability is optimal, **not everything can be patched**.
  - A balancing act is required to **provide the service** while **protecting data and systems**.
  - Not all vulnerabilities share the same severity—some may require local login, physical access, or other specific criteria.
  - **Exceptions** may be made, often through a formal approval process.

### Validation of Remediation
- After a vulnerability is patched, validation is needed:
  - **Does the patch really stop the exploit**?
  - **Did you patch all vulnerable systems**?
  - Perform an **extensive vulnerability scan**.
  - **Audit**: Check remediated systems to ensure the patch was successfully deployed.
  - **Verification**: Manually confirm the security of the system after remediation.

### Reporting
- Ongoing checks are required since new vulnerabilities are continuously discovered.
  - **Challenges**: Managing vulnerabilities without automation can be time-consuming.
  - **Continuous reporting** includes:
    - The number of identified vulnerabilities.
    - Systems patched vs unpatched.
    - New threat notifications.
    - Errors, exceptions, and exemptions.

# 4.4 Security Monitoring

### Overview
- **Attackers** are constantly trying to access systems and services, making continuous monitoring essential.
  - Monitor all **entry points**: logins, publicly available services, data storage locations, and remote access.
  - React to security events: account access, firewall rule changes, additional scanning.
  - Use **status dashboards** to get a quick overview of system statuses.

### Monitoring Computing Resources
- **Systems**: Monitor authentication attempts and login patterns, especially from unusual locations.
- **Server Monitoring**: Track service activity, backups, and software versions to ensure everything is functioning as expected.

### Applications
- **Availability**: Monitor uptime and response time to ensure systems are operational.
- **Data Transfers**: Track increases or decreases in data transfer rates to identify potential security issues.
- **Security Notifications**: Stay informed about security updates from developers or manufacturers.

### Infrastructure
- **Remote Access Systems**: Monitor access by employees, vendors, and guests to ensure proper security.
- **Firewall and IPS Reports**: Review attack reports or increases in certain types of attacks to adjust defenses accordingly.

### Log Aggregation
- **SIEM (Security Information and Event Management)** or **SEM (Security Event Management)**: 
  - Centralize log data from servers, firewalls, VPN concentrators, SANs, and cloud services.
  - Correlate logs to track authentication/access, application usage, and data transfers.
  - **Centralized Reporting**: View all information in one place, helping to make informed decisions.

### Scanning
- The **threat landscape is constantly changing**, with new vulnerabilities discovered daily.
  - Many organizations have systems in place to **constantly scan all systems** connected to their network.
  - Provides **metrics** such as operating system types, device driver versions, installed applications, and anomalies.
  - Gathers raw data that can be used to identify potential security issues.

### Reporting
- **Analyze collected data** and create actionable reports that help direct the next steps.
  - **Status Information**: Report on devices that are up to date or in compliance.
  - Identify devices running outdated software or those that need updates.
  - Assess vulnerabilities: How many systems are vulnerable to new threats?

### Ad Hoc Information Summaries
- Prepare for unexpected events by summarizing relevant data quickly and efficiently.

### Archiving
- It takes, on average, **9 months** for a company to identify and contain a breach.
  - **Archiving data** over an extended period is crucial for effective incident management.
  - Some organizations have **mandates** or **laws** requiring them to store data for a specific time.

### Alerting
- **Real-time notifications** of security events help maintain situational awareness.
  - Examples: Increases in authentication errors, large file transfers, etc.
  - **Actionable data**: Ensure the right people are informed to enable quick responses.
  - **Notification Methods**: Use SMS/text, email, or security console/SOC alerts.

### Alert Response and Remediation
- **Quarantine**: A foundational response to prevent the spread of potential security issues.
- **Alert Tuning**: Balancing accuracy to minimize false positives and negatives.
  - **Continuous improvement**: Alert tuning gets more accurate over time as more data is collected.

# 4.4 Security Tools

### Security Content Automation Protocol (SCAP)
- **SCAP** allows security tools to evaluate threats in a standardized way, enabling them to identify and act on the same criteria.
  - Helps in validating **security configurations**, confirming patch installations, and scanning for breaches.
  - Useful for large environments with multiple operating systems and applications.
  - Automation types: ongoing monitoring, notifications, alerting, and remediation of non-compliant systems.
  
### Using SCAP
- SCAP content can be shared between different tools, ensuring consistent configuration compliance across various systems.
  - **Automation**: Ensures compliance and vulnerability detection are automated, even with diverse tools.
  
### Benchmarks
- **Security best practices** should be applied universally across all systems, including OS, cloud providers, and mobile devices.
  - **Popular Benchmarks**: Centre for Internet Security (CIS) provides a benchmark for securing systems.
  - Example for mobile devices: 
    - Disable screenshots, force encryption, and configure a "lost phone" message.

### Monitoring Types
#### Agent-based Monitoring
- **Agent-based monitoring** requires installing a software agent on each device.
  - Provides **real-time notifications** and continuous monitoring.
  - Needs ongoing maintenance and updates.
  
#### Agentless Monitoring
- **Agentless monitoring** collects data without installing software on the target device.
  - Relies on standard protocols to gather information.
  - Does not provide real-time alerts unless actively running.

### SIEM: Security Information and Event Management
- **SIEM** consolidates log files from various systems into a central database.
  - **Log Collection**: Gathers real-time security event data and stores logs long-term.
  - **Data Correlation**: Links diverse data types and provides forensic analysis after an event.

### Anti-virus and Anti-malware
- **Anti-virus** (now also referred to as **anti-malware**) prevents and removes malicious software from devices.
  - Protects against a variety of threats: trojans, worms, viruses, spyware, ransomware, and fileless malware.
  
### Data Loss Prevention (DLP)
- **DLP** strategies are designed to detect and prevent unauthorized access or transmission of sensitive data.
  - Protects sensitive data such as **social security numbers**, **credit card numbers**, and **medical records**.
  - Stops **data leakage** before it happens, securing data at endpoints or in cloud systems.

### Simple Network Management Protocol (SNMP)
- **SNMP** is used to monitor and manage network devices (routers, switches, servers, etc.).
  - Gathers data from devices at fixed intervals to create **historical performance graphs**.
  - **SNMP Traps** alert when specific thresholds (like error rates) are exceeded.

### NetFlow
- **NetFlow** monitors traffic flows across a network and gathers statistics related to application usage.
  - Used to create **reports** and monitor **traffic flows** between devices on the network.

### Vulnerability Scanners
- **Vulnerability scanners** perform minimally invasive checks to gather information about potential vulnerabilities.
  - Can identify open ports, system vulnerabilities, and misconfigurations.
  - **Port scans** and system scans gather details but may result in **false positives/negatives**.

# 4.5 Firewalls

### Network-based Firewalls
- **Network-based firewalls** filter traffic based on port numbers or applications.
  - Can be either **traditional** or **Next-Generation Firewalls (NGFW)**.
  - Often placed at the **ingress/egress** points of a network.
  - **Encrypt traffic** and provide VPNs between sites.
  - **Network Address Translation (NAT)** and **dynamic routing** are common features.
  - Some firewalls operate at **Layer 3** (routers) to manage traffic.

### Next-Generation Firewall (NGFW)
- Combines traditional firewall features with additional security capabilities.
  - **Application Awareness and Control**: Monitors and manages application traffic.
  - **Integrated Intrusion Prevention System (IPS)**: Detects and prevents intrusions.
  - **Cloud-delivered Threat Intelligence**: Provides up-to-date threat information.
  - Operates at **Layer 7** (Application Layer).
  - **Stateful Multilayer Inspection**: Analyzes each packet thoroughly.
  - Uses **Deep Packet Inspection (DPI)** to inspect and categorize all packets.
  - Makes forwarding decisions based on the **protocol** (TCP or UDP) and **port number**.

### Firewall Rules
- Firewall rules follow a logical path, typically from **top to bottom**.
  - More **specific rules** are placed higher in the list, while general ones are placed lower.
  - Most firewalls have an **implicit deny** rule at the bottom to block any unspecified traffic.
  - **Access Control Lists (ACLs)** specify rules that either **allow** or **deny** traffic based on:
    - Source IP, destination IP, port numbers, time of day, or applications.

### Screened Subnet (DMZ)
- A **Screened Subnet** or **Demilitarized Zone (DMZ)** separates the internal LAN from untrusted external networks.
  - Adds an extra layer of security by isolating **external-facing services** from the internal network.
  - Public-facing resources are available to external users, while **private data remains protected**.

### IPS Rules (Intrusion Prevention System)
- **IPS rules** are commonly integrated into **NGFWs** to detect and prevent malicious traffic.
  - Methods to detect malicious traffic:
    - **Signature-based**: Looks for exact matches of known attack patterns.
    - **Anomaly-based**: Builds a baseline of normal behavior and flags deviations.
  - Actions upon detecting malicious traffic: **Block**, **Allow**, **Alert**, etc.
  - IPS rules can be customized by group or individually to balance security with reducing false positives.
  - Finding the right balance of **security** and minimizing **alert noise** is crucial for efficient monitoring.

# 4.5 Web Filtering

### Content Filtering
- Controls traffic based on the data within the content itself.
  - **URL Filtering**: Restricts access to specific websites or categories of websites.
  - **Corporate Control**: Prevents the transmission of sensitive materials and inappropriate content.
  - **Parental Controls**: Blocks access to non-work-safe sites.
  - **Malware Protection**: Blocks traffic that may contain malicious code like viruses.

### URL Scanning
- Allows or restricts access based on the **Uniform Resource Locator (URL)**.
  - Often managed via **allow lists** or **block lists**.
  - Can be organized by **category** (e.g., auction sites, malware sites, travel, etc.).
  - **NGFW** often integrates URL filtering by category or specific URL.
  - While effective, URLs aren't the only method to access content on the internet.

### Agent-Based Filtering
- Involves installing **client software (agent)** on each user's device.
  - The agent filters content locally, regardless of the user's location or when they connect to the network.
  - **Always on** and continuously filtering.
  - **Cloud-based updates** are pushed to all agents, and update status can be monitored from a central console.

### Proxies
- A **proxy** acts as an intermediary between users and external websites.
  - **Forward Proxy**: Installed within an organization to control users' access to the internet.
  - **Caching**: Proxies can store frequently accessed data to improve response times.
  - **Access Control**: Proxies can enforce access control and URL filtering.
  - **Content Scanning**: Proxies can scan content for malware and other security risks.
  - Proxies may either be **explicit** (configured by applications) or **transparent** (invisible to users).

### Forward Proxy
- A **forward proxy** is placed between users and the internet, controlling internet access for internal users.
  - Used primarily to **protect and control** user access to external resources.

### Block Rules
- Filters based on specific **URLs** or **site categories**.
  - Categories are often divided into **50+ topics** such as:
    - Adult, educational, gambling, government, malware, etc.
  - Different dispositions for each category:
    - **Educational**: Allow
    - **Home and Garden**: Allow with alert
    - **Gambling**: Block

### Reputation-Based Filtering
- Filters URLs based on their **perceived risk** or reputation.
  - Websites with a **good reputation** are allowed access.
  - **Bad reputation** sites are blocked.
  - Reputation can be **automated** (sites are scanned and categorized automatically) or **manual** (administrators assign reputations to sites).
  - Risk levels:
    - **High risk**: Block
    - **Trustworthy**: Allow

### DNS Filtering
- Prevents access to harmful websites by intercepting **DNS requests**.
  - **DNS lookup** checks the website's IP address against **real-time threat intelligence**.
  - If a site is on a blacklist (commercial or public), the DNS will not resolve the domain, thus preventing the connection.
  - DNS filtering works for **all DNS lookups**, not just for web filtering.

# 4.5 Operating System Security

### Active Directory (AD)
- **Active Directory** is a centralized database used primarily in Windows environments to manage various network resources like computers, user accounts, file shares, printers, and groups.
  - **Authentication**: Users log in with their **AD credentials**.
  - **Centralized Access Control**: Manages which users can access specific resources across the network.
  - **Help Desk Usage**: Commonly used by help desk personnel for tasks such as **password resets** and **account management** (adding/removing users).

### Group Policy
- **Group Policy** enables the management of user and computer configurations via policies.
  - **Local and Domain Policies**: Policies can be applied locally to individual computers or across an entire domain.
  - **Group Policy Management Editor**: The central console for managing these policies, which includes configuring login scripts, **QoS (Quality of Service)** settings, **network configurations**, and **security parameters**.
  - Provides comprehensive control with hundreds of configuration options to manage the security and behavior of user and computer settings.

### Security-Enhanced Linux (SELinux)
- **SELinux** provides enhanced security features for Linux operating systems by introducing **Mandatory Access Control (MAC)**.
  - Traditionally, Linux uses **Discretionary Access Control (DAC)**, where users control access to their own resources. SELinux introduces a more stringent access control model.
  - **Limits application access**: By enforcing the principle of least privilege, SELinux limits what applications can do, reducing the scope of potential breaches.
  - **Open Source**: SELinux is available as an open-source tool for improving Linux security.

# 4.5 Secure Protocols

### Unencrypted Network Data
- Some network protocols do not encrypt traffic, making the data vulnerable to interception. Examples include:
  - **Telnet**, **FTP**, **SMTP**, **IMAP**
  - You can verify if traffic is unencrypted using packet capture tools.

### Protocol Selection
- **Use secure protocols** with built-in encryption to ensure data protection:
  - **Remote Console**: Replace **Telnet** with **SSH** (Secure Shell)
  - **Web Browsing**: Replace **HTTP** with **HTTPS** for encrypted browsing
  - **Email Client Access**: Use **IMAPS** instead of **IMAP** for secure email communication
  - **File Transfer**: Replace **FTP** with **SFTP** (Secure File Transfer Protocol) for secure file transfers

### Port Selection
- Secure and insecure versions of protocols may operate on different ports, making it easy to identify which traffic is secured and which is not.
  - **HTTP**: Port 80 (unencrypted)
  - **HTTPS**: Port 443 (encrypted)

### HTTP and HTTPS
- **HTTP** and **HTTPS** handle web browsing traffic:
  - **HTTP** operates on **Port 80** and is **unencrypted**, leaving data exposed.
  - **HTTPS** operates on **Port 443** and **uses encryption** (SSL/TLS) to protect data.
  - **Port numbers** alone do not guarantee security, so always verify that encryption is enabled. Packet captures can help confirm encryption.

### Transport Method
- **Transport-level encryption** is essential for securing data, especially over open or public networks.
  - **802.11 Wireless**: On an **Open Access Point**, there is **no transport-level encryption**. Data is transmitted in plaintext, vulnerable to interception.
  - **WPA3**: Encrypts all user data over the wireless network, providing secure communication.
  - **VPN**: Creates an **encrypted tunnel**, ensuring that all traffic is protected, often relying on third-party services and software to establish the secure connection.

# 4.5 Email Security

### Email Security Challenges
- **Protocols** used for email transfer often lack sufficient security checks, making emails vulnerable to various threats such as phishing, spoofing, and spam.

### Mail Gateway
- The **Mail Gateway** acts as a gatekeeper that evaluates the source of inbound emails before they reach the user.
  - It **blocks malicious emails** at the gateway, preventing them from reaching the inbox.
  - Checks the **validity** of the email's source, discarding or sending untrusted emails to the **spam folder**.
  - Mail gateways are typically located in the **screened subnet**, providing an additional layer of security.

### Sender Policy Framework (SPF)
- **SPF** is a protocol that allows the sender to configure a list of authorized servers that can send emails on behalf of their domain.
  - **SPF TXT Record**: A DNS record is used to list the authorized mail servers.
  - **Mail Server Checks**: The receiving mail server checks the incoming email's source to verify it matches the authorized server list.

### DomainKeys Identified Mail (DKIM)
- **DKIM** allows the sender to digitally sign all outgoing emails.
  - The **signature** is validated by the receiving mail servers, but is generally **invisible** to the end user.
  - This helps verify that the email has not been tampered with during transmission.

### Domain-based Message Authentication, Reporting, and Conformance (DMARC)
- **DMARC** builds on SPF and DKIM, allowing domain owners to specify what actions receiving servers should take for emails that fail SPF and DKIM checks.
  - The domain owner writes the policy into a **DNS TXT record**, specifying whether to **accept**, **send to spam**, or **reject** such emails.
  - **Compliance Reports**: The domain owner receives reports from receiving servers, helping them understand how many emails passed or failed authentication.

# 4.5 Monitoring Data

### File Integrity Monitoring (FIM)
- **FIM** monitors important operating system and application files to ensure their integrity.
  - Tracks files that **never change**, and flags when any changes occur.
- **Windows - SFC (System File Checker)**:
  - Scans all operating system files for changes, and replaces modified files with a fresh version from the original installation.
- **Linux - Tripwire**:
  - A tool used to monitor and verify the integrity of files on Linux systems.
- **Host-based IPS** can also be utilized for monitoring system files and detecting unauthorized changes.

### Data Loss Prevention (DLP)
- **DLP** systems are designed to detect sensitive data (e.g., SSNs, credit card numbers, medical records) being transmitted across the network, and block it in real-time to prevent leakage.
  - **Data in Use**: Monitored on endpoints through **Endpoint DLP** to control data manipulation.
  - **Data in Motion**: Monitored on the network to prevent transmission of sensitive data.
  - **Data at Rest**: Monitored on servers to ensure sensitive data is secure even when not actively in transit.

### USB Blocking
- DLP can be applied to block the use of unauthorized USB devices on workstations, preventing data leakage through external media.

### Cloud-based DLP
- Located between users and the internet, **cloud-based DLP** examines all network traffic without requiring hardware or software on the user’s machine.
  - Can block **custom-defined data strings** unique to an organization (e.g., proprietary data).
  - Manages **URL access**, preventing file transfers to unauthorized cloud storage.
  - Detects and blocks viruses, malware, and other malicious content as it traverses the network.

### DLP and Email
- **Email continues to be a major risk vector** for data loss.
  - **Inbound Threats**: DLP can scan incoming emails for keywords, suspicious senders, or malicious content, and quarantine emails as needed.
  - **Outbound Threats**: DLP checks outgoing emails for sensitive information, such as fake wire transfers or personal employee data, and can block or drop such messages to prevent data leakage.

# 4.5 Endpoint Security

### Endpoint Device
- **Endpoint devices** (e.g., laptops, smartphones, desktops) are vulnerable points where applications and data can be exploited by attackers to gain access to user data and sensitive information.

### Edge vs. Access Control
- **Edge Control**: Managed primarily through **firewall rules**, the edge controls the perimeter of your network. Firewall rules generally remain static and change infrequently.
- **Access Control**: Focuses on limiting **user access** to specific data types or resources, based on rules such as:
  - User identity
  - User group
  - Location
  - Application
  - Access can be easily adjusted and revoked, allowing you to change your security posture as needed.

### Posture Assessment
- **Posture assessment** evaluates the overall security stance of an organization, including identifying vulnerabilities, weaknesses, and areas for improvement. It covers all devices in the organization (desktops, mobile devices, servers, etc.).
  - **Key areas checked**:
    - Security patches, firmware, and updates are up-to-date.
    - Presence of malware or missing anti-malware solutions.
    - Unauthorized applications.
  - **Pre-connection checks** include ensuring:
    - Device is trusted.
    - Anti-virus is running and updated.
    - Corporate applications are installed.
    - Device encryption is in place.
    - Company certificates are applied.
  
#### Health Checks/Posture Assessment:
- **Persistent Agent**: A permanent agent installed on the system, performing periodic updates and monitoring running files or applications.
- **Dissolvable Agent**: A temporary agent that runs only during the posture assessment and terminates afterward.
- **Agentless NAC**: Integrated with Active Directory, it checks the device status during login/logoff but cannot be scheduled.

### Failing Your Assessment
- If a device fails the posture assessment:
  - The device may be placed in **quarantine**.
  - Administrators are notified to take corrective action.
  - Once the device becomes compliant, the assessment can be reattempted.

### Endpoint Detection and Response (EDR)
- **EDR** solutions are designed to monitor, detect, and respond to suspicious activity on endpoints (e.g., computers, servers, mobile devices).
  - Uses **signatures**, **behavioral analysis**, **machine learning**, and **process monitoring**.
  - A **lightweight agent** is placed on the endpoint.
  - EDR systems investigate threats, perform **root cause analysis**, and respond by isolating the affected system, quarantining threats, or rolling back to a previous configuration.

### Extended Detection and Response (XDR)
- **XDR** extends the capabilities of EDR by integrating additional intelligence and broader detection scope, including:
  - **Network-based detection** to investigate network anomalies.
  - Correlation of data across endpoints, network, and cloud.
  - Improved detection rates and simplified investigation of security events.
  - Aims to reduce false positives and improve detection efficacy.

### User Behavior Analytics (UBA)
- XDR systems often incorporate **User Behavior Analytics (UBA)**, which involves:
  - Monitoring user behavior across devices, hosts, networks, and data repositories.
  - Creating a baseline of normal activity.
  - Using statistical analysis, pattern matching, and rules to detect anomalies.
  - Real-time detection of unusual behavior, helping identify potential threats based on deviations from normal patterns.

# 4.6 Identity and Access Management (IAM)

### Overview
- **Identity and Access Management (IAM)** is the process that begins when a user needs access and ends when that user no longer requires access.
  - **Digital Identity**: Every entity (user, device, service) is assigned a digital identity.
  - **Access Control**: Ensures entities are granted access to necessary resources.
  - **Authentication & Authorization**: Entities must prove their identity (authentication) and be authorized to access specific resources.
  - **Identity Governance**: Involves tracking an entity’s access to resources, often a regulatory requirement.

Applications can be accessed across various platforms such as desktops, browsers, and mobile devices, while data may reside in multiple locations, including cloud storage and private data centers. IAM manages access for different user types, including employees, vendors, contractors, and customers.

### Key Principles
- **Provisioning/De-provisioning User Accounts**: The process of creating and removing user accounts based on certain events like hiring, transfers, promotions, and job separations.
  - Account details may include name, attributes, group permissions, and other access rights.
  - **Initial Checkpoint**: Controls and limits access during account creation.
  - **No Administrator Access**: Prevents users from being assigned administrator rights unnecessarily.

- **Permission Assignments**: Ensures entities only have the minimum permissions needed to perform their job tasks.
  - **Principle of Least Privilege**: Limits access to just enough to do the job.
  - **Group Assignments**: Common method for organizing permissions.
  - **Private Data**: Files and storage can be restricted to individual users, even when others share the device.
  - **No OS-Level Privileges**: User accounts should not have privileged access to the operating system.

### Identity Proofing
- The IAM process should verify the identity of users:
  - **Resolution**: Determining who the system believes the user to be.
  - **Validation**: Gathering information such as passwords, security questions, or multi-factor authentication (MFA).
  - **Verification/Attestation**: Confirming identity through documents (e.g., passports) or in-person meetings.

### Key IAM Technologies
- **Single Sign-On (SSO)**: Allows users to authenticate once and access all authorized resources without needing to authenticate again for a specified period (e.g., 24 hours).
  
- **LDAP (Lightweight Directory Access Protocol)**: A protocol for reading and writing directories over an IP network, often used to store user information (like a phone directory).
  
- **X.500 Distinguished Names**: A naming convention used in directory services to identify users or resources by specifying attribute-value pairs, typically in a hierarchical structure.

- **Security Assertion Markup Language (SAML)**: An open standard for authentication and authorization, enabling third-party authentication to grant access. Initially not designed for mobile apps.
  - **SAML Authentication Flow**:
    1. Client requests access to an application.
    2. Authentication server sends an encrypted SAML request.
    3. After successful login, the SAML token is generated.
    4. The user presents the SAML token to the resource server.

- **OAuth**: An authorization framework that grants access to resources across applications. Unlike SAML, OAuth doesn't handle authentication itself—this is managed by OpenID Connect. OAuth enables third-party applications to access resources without sharing user credentials.
  
- **Federation**: Allows authentication across different organizations without relying on local authentication databases. Users can authenticate with third-party credentials (e.g., using Facebook login) across different federated systems.
  - Enables **Single Sign-On (SSO)** and more.

- **Interoperability**: IAM systems can communicate with various authentication services based on the environment, allowing diverse authentication protocols like LDAP, OAuth, and SAML to work together.
  - **VPN and LDAP Integration**: For instance, a VPN concentrator might connect to an LDAP server for authentication.
  - Applications might use OAuth for authentication APIs, enhancing interoperability as part of a comprehensive IAM strategy.

# 4.6 Access Controls

### Overview of Access Control Concepts
**Authorization**: Ensures that only authorized rights are exercised by users.
- **Policy Enforcement**: Enforces policies that govern user rights.
- **Policy Definition**: Determines the rules under which users are granted or denied access.
- Rights are assigned based on the Access Control model in place, tailored to business or mission requirements.

### Key Access Control Models
- **Least Privilege**: 
  - Assign only the minimum rights necessary for users to complete their tasks.
  - Users and applications should run with minimal privileges.
  - **No Administrative Privileges**: Users should not have administrative access unless absolutely necessary to reduce the scope of potential malicious behavior.

- **Mandatory Access Control (MAC)**:
  - Access is restricted based on security clearance levels assigned to both objects and users.
  - Objects (files, data) are labeled with security levels such as **Top Secret**, **Secret**, **Confidential**, etc.
  - Only administrators can decide who can access each security level.
  - Users cannot change these access settings.

- **Discretionary Access Control (DAC)**:
  - The owner or administrator of a system defines access control policies.
  - **Owner Control**: The creator of a resource (like a document or spreadsheet) can grant or restrict access at their discretion.
  - DAC is flexible but less secure because the owner has full control over access permissions.

- **Role-based Access Control (RBAC)**:
  - Rights and permissions are assigned based on the roles users hold within the organization (e.g., **Manager**, **Director**, **Project Manager**).
  - Users inherit permissions implicitly based on their group membership.
  - In Windows, **Groups** are often used to manage RBAC.

- **Rule-based Access Control**:
  - Access is determined by a set of predefined rules set by system administrators.
  - Rules are typically condition-based and automatically enforced.
  - Examples of rules might include:
    - **Time of Day**: Access may only be granted during specified hours (e.g., access to a network may be limited to 9 am - 5 pm).
    - **Action Type**: Access to certain actions may be restricted to specific conditions (e.g., only certain browsers allowed).

- **Attribute-based Access Control (ABAC)**:
  - Access is determined by evaluating multiple characteristics of users, resources, and environments.
  - Fine-grained control can be applied, considering context-sensitive decisions.
  - **Attributes** may include:
    - **User Attributes**: Role, department, security clearance.
    - **Resource Attributes**: Classification, type, ownership.
    - **Environmental Attributes**: Time of day, IP address, location, device type.
  
### Time-of-Day Restrictions
- Security devices can restrict access based on the time of day or specific days of the week.
- **Examples**:
  - **Training Room**: Network access is restricted between midnight and 6 am.
  - **Conference Room**: Access is unavailable after 8 pm.
  - **R&D Databases**: Accessible only from 8 am to 6 pm.

# 4.6 Multifactor Authentication (MFA)

Multifactor Authentication (MFA) is a security mechanism that requires users to prove their identity using more than one factor from different categories. It strengthens security by making it harder for attackers to impersonate legitimate users.

### Types of Authentication Factors

1. **Something You Know**:
   - **Password**: A secret string of characters used for authentication. 
   - **PIN**: A personal identification number, typically shorter than a password, often used for device or account access.
   - **Pattern**: A series of movements or designs that the user must complete, often used on mobile devices.

2. **Something You Have**:
   - **Smart Card**: A physical card integrated with a microchip, often used with a PIN for two-factor authentication.
   - **USB Security Key**: A small physical device that holds a certificate for authentication, often used for two-factor authentication (e.g., YubiKey).
   - **Hardware or Software Tokens**: Generates a pseudo-random authentication code that is used in conjunction with a password. These codes typically expire after a short period.
   - **Phone (SMS or App-based)**: A code sent via SMS or generated by an app (e.g., Google Authenticator) that the user enters in addition to their password.

3. **Something You Are**:
   - **Biometric Authentication**: Involves using unique physical characteristics for identification, such as:
     - **Fingerprint**
     - **Iris Scan**
     - **Voice Print**
   - Biometric data is stored as a mathematical representation and is challenging to alter, offering a high level of security. It's used in specific high-security situations.

4. **Somewhere You Are**:
   - **Location-Based Authentication**: Uses the user's physical location to verify identity.
     - For example, access to sensitive data may only be permitted if the user is within a specified geographic region.
   - **IP Address**: Often used to track a user's location; works well with IPv4 addresses but is less effective with IPv6 due to the large address space and more complex network structures.

### Benefits of MFA
- **Enhanced Security**: Requires multiple factors, making it harder for attackers to gain unauthorized access.
- **Reduced Risk of Credential Theft**: Even if an attacker steals one factor (like a password), they still need other factors to succeed.
- **Protection Against Phishing**: MFA helps protect against phishing attacks where an attacker might steal a user’s credentials.

By incorporating multiple authentication methods, MFA significantly strengthens access control mechanisms and reduces the likelihood of unauthorized access.

# 4.6 Password Security

Password security is a critical component of securing user accounts and sensitive data. Implementing strong password policies and practices can greatly reduce the risk of unauthorized access.

### Key Concepts in Password Security

1. **Password Complexity and Length**:
   - **Entropy**: Refers to how unpredictable a password is. The more unpredictable, the stronger the password.
   - **Brute-force Protection**: Passwords should be complex enough to resist brute-force attacks.
   - **Best Practices**:
     - Avoid single words or easily guessable passwords.
     - Use a mix of upper and lower case letters, numbers, and special characters.
   - **Length**: Strong passwords typically have at least 8 characters, and as computing power increases, longer passwords are recommended.

2. **Password Age**:
   - **Expiration**: Regularly change passwords to reduce the risk of compromised credentials. Common expiration cycles are 30, 60, or 90 days.
   - **Password History**: Many systems prevent the reuse of previous passwords, ensuring that users create unique passwords each time.

3. **Password Managers**:
   - **Importance**: Using different passwords for each account reduces the risk of a breach. Password managers help store and organize these passwords securely.
   - **How It Works**: Password managers encrypt and protect all passwords in a central database, which can include multi-factor tokens for extra security.
   - **Enterprise Solutions**: In an organizational context, password managers allow centralized management and recovery options, making it easier to control and secure access.

4. **Passwordless Authentication**:
   - **Description**: An alternative to traditional passwords, where users authenticate using other methods like biometrics, one-time passcodes, or magic links.
   - **Methods**:
     - **Biometrics**: Fingerprints, facial recognition, or voice prints.
     - **One-Time Passcodes (OTP)**: Temporary codes sent via email or SMS.
     - **Security Keys**: Hardware devices (like YubiKeys) that provide additional authentication.
   - **Usage**: Passwordless authentication is often used in combination with other methods (like multi-factor authentication) for added security.

5. **Just-In-Time Permissions**:
   - **Temporary Administrator Access**: Administrator rights are granted only for a limited time to prevent long-term vulnerabilities.
   - **Principle of Least Privilege**: Users are given only the minimum necessary access, reducing the potential damage in the event of a breach.
   - **Access Request Process**: Users request elevated access from a central authority, which grants or denies access based on predefined security policies.
   - **Password Vaulting**: Primary credentials are stored in a secure vault and only accessible for short durations. This prevents permanent access to sensitive credentials.

### Best Practices
- Enforce strong password complexity and length requirements.
- Regularly change passwords and prevent the reuse of old ones.
- Utilize password managers to store and manage unique, complex passwords for each service.
- Consider implementing passwordless authentication methods to reduce the reliance on traditional passwords.
- Use just-in-time permissions to minimize the risks of unnecessary elevated access.



# 4.7 Scripting and Automation


### Key Concepts in Scripting and Automation

1. **Automate and Orchestrate**:
   - **Scripting**: Scripts eliminate typing delays and reduce human errors. They are designed to automate mundane tasks that are repetitive and time-consuming.
   - **Orchestration**: Involves integrating and automating complex workflows across multiple systems, ensuring everything works together efficiently.

2. **Benefits of Automation**:
   - **Time Saving**: Automation speeds up processes by eliminating manual tasks.
   - **Repetition**: Scripts can be run multiple times without variation, ensuring consistency and reliability.
   - **Security Enforcement**: Automation can ensure that security patches are applied promptly. For example, if a patch is missing, automation can identify and install it automatically.
   - **Infrastructure Configuration**: Standard configurations can be automated through scripts. This includes setting up default router configurations, firewall rules, and IP setups.
   - **Secure Scaling**: Automation helps in scaling cloud resources securely, quickly adjusting to changing needs without compromising security.
   - **Employee Retention**: By automating repetitive tasks, employees can focus on more complex and rewarding work, reducing burnout and improving job satisfaction.
   - **Faster Reaction Time**: Automation allows for immediate responses to events, improving incident response times.

3. **Common Use Cases for Automation**:
   - **User and Resource Provisioning**: Automating tasks such as user on-boarding and off-boarding, assigning access to resources.
   - **Guard Rails**: Automated validations ensure that security policies are properly implemented, reducing human error.
   - **Security Groups**: Automating the assignment or removal of access to security groups, along with constant auditing to maintain compliance.
   - **Ticket Creation and Escalation**: Scripts can automatically generate tickets for identified issues, or escalate issues to the appropriate team if not resolved.
   - **Service Management**: Automating the enabling and disabling of services based on certain triggers.
   - **Development and Code Updates**: Ensuring that software development and updates are securely tested and deployed automatically.
   - **API Integrations**: Automating interactions with third-party devices and services, such as cloud services, firewalls, and operating systems, through APIs.

4. **Considerations for Scripting and Automation**:
   - **Cost**: While automation saves time, it often requires upfront investment, whether it’s for hiring professionals to create scripts or for implementing the automation system.
   - **Single Point of Failure**: If an automation script fails, it can cause significant problems across multiple devices or systems. It's crucial to ensure that scripts are robust and monitored.
   - **Technical Debt**: Over time, the failure to maintain scripts can lead to technical debt, making it costly and difficult to fix issues down the line.

### Best Practices for Scripting and Automation
- **Design for Scalability**: Ensure that your automation scripts can handle growing environments and are flexible enough to scale.
- **Continuous Monitoring**: Regularly monitor automated tasks to catch errors early and prevent cascading failures.
- **Documentation**: Keep clear and up-to-date documentation for all scripts and automated processes to ensure transparency and ease of troubleshooting.
- **Backup Plans**: Have contingency plans in place in case of script failure, such as alerts or manual overrides.

# 4.8 Incident Response

Incident response is the process of identifying, managing, and recovering from security incidents. These incidents can be breaches, failures in security controls, or threats to the Confidentiality, Integrity, or Availability (CIA) of systems and data.

### Types of Security Incidents:
- **Unauthorized Access**: When an attacker gains access to systems or data without permission.
- **Data Breach**: Unauthorized disclosure or exposure of sensitive data.
- **Malware Infection**: The introduction of malicious software into the environment.
- **DDoS/Botnet Attack**: Distributed Denial of Service attacks or botnet-driven attacks.
- **Insider Threats**: Threats posed by individuals within the organization.
- **Phishing Attacks**: Fraudulent attempts to obtain sensitive information by impersonating legitimate entities.

### NIST SP800-61 - Computer Security Incident Handling Guide: Incident Response Lifecycle
1. **Preparation**: Preparation involves setting up the necessary resources, policies, and protocols for handling incidents.
2. **Detection and Analysis**: Identifying and analyzing potential security incidents through monitoring and analysis tools.
3. **Containment, Eradication, and Recovery**: Taking action to isolate the incident, remove malicious elements, and recover the system.
4. **Post-Incident Activity**: Reviewing the incident after resolution to improve future responses and learn from the experience.

### Preparing for an Incident
- **Communication Methods**: Ensure that you have reliable communication channels in place, such as phones and contact information.
- **Incident Go-Bag**: A prepared kit containing incident handling tools and software, including laptops, removable media, forensic software, and digital cameras.
- **Incident Analysis Resources**: Gather documentation, network diagrams, and critical file hash values to assist with incident investigation.
- **Incident Mitigation Software**: Have clean operating system images and applications ready to help mitigate the incident.
- **Incident Handling Policies**: Ensure everyone is aware of their roles and the procedures to follow during an incident.

### The Challenge of Detection
Effective detection requires extensive knowledge to differentiate between normal activity and potential targeted attacks. Identifying a real attack often involves understanding system behaviors, network traffic, and security logs.

### Incident Analysis
During an incident, various tools and techniques are used to gather information:
- **Web Server Logs**: Reviewing logs for unusual activity or indicators of compromise.
- **Vulnerability Scanners**: Identifying known weaknesses in systems or software.
- **Exploit Announcements**: Monitoring for information on new vulnerabilities or exploits.
- **IPS/IDS Alerts**: Detecting suspicious activity such as buffer overflow attempts.
- **Anti-virus/Malware Alerts**: Identifying malware or other security threats.
- **Host-based Monitoring**: Detecting changes in system configurations or abnormal behavior.
- **Network Traffic Analysis**: Identifying deviations from normal traffic patterns.

### Isolation and Containment
- **Sandboxes**: Running suspected malware in an isolated environment to analyze its behavior without risk to the production systems.
- **Isolated OS**: Using a contained operating system to analyze the malware's impact and behavior safely.

### Recovery After an Incident
- **Eradication**: Remove malicious software, disable compromised accounts, and patch vulnerabilities.
- **Restoration**: Restore systems from backups, rebuild systems from scratch, replace compromised files, and strengthen security controls.
- **Lessons Learned**: After recovery, conduct a post-incident review to identify areas of improvement.

### Post-Incident Meeting
- **What Happened?**: Review the sequence of events, including timestamps and affected systems.
- **Incident Response Effectiveness**: Evaluate how well the incident response process worked.
- **Improvement Plans**: Identify areas for improvement and lessons learned for future incidents.
- **Indicator Review**: Discuss what indicators to monitor in the future to prevent similar incidents.

### Training for Incident Response
- **Initial Response Training**: Ensure the team is trained on how to handle incidents from the start.
- **Investigation Plans**: Have clear procedures for investigating incidents.
- **Incident Reporting**: Establish guidelines for reporting incidents to internal and external stakeholders.

# 4.8 Incident Planning

Incident planning involves preparing, testing, and refining processes to respond effectively to security incidents.

### Exercising: Test Yourself Before an Actual Event
- **Scheduled Update Sessions**: Regularly test incident response processes through annual or semi-annual exercises.
- **Rules of Engagement**: Define clear boundaries and rules for exercises to avoid impacting production systems.
- **Evaluate Response**: After each exercise, document results and conduct a debrief to evaluate the effectiveness of the response.

### Tabletop Exercise
A tabletop exercise is a simulated scenario designed to test the team’s readiness to respond to various incidents. These can include:
- **Simulated Attacks**: Role-playing different types of attacks such as phishing, password requests, or data breaches to assess team preparedness and response strategies.

### Root Cause Analysis
Root cause analysis is a systematic process for identifying the underlying causes of an incident or problem. This process helps organizations understand what went wrong and develop strategies to prevent future occurrences.

### Threat Hunting
Threat hunting is a proactive approach to identifying and isolating advanced threats that may bypass automated detection mechanisms. The goal is to find and neutralize the attacker before they can cause damage or compromise systems. This practice involves searching through networks, systems, and data sets to uncover hidden threats.

# 4.8 Digital Forensics

Digital forensics involves the process of collecting, preserving, and analyzing data to investigate security incidents or criminal activities. It is vital for legal and internal investigations to ensure that evidence is properly handled and remains admissible in court.

### Standard Digital Forensic Process
The forensic process must be meticulously detailed and follows these key stages:
- **Acquisition**: Securely gather data from various sources.
- **Analysis**: Examine the collected data for signs of intrusions, unauthorized access, or other malicious activities.
- **Reporting**: Document findings, methodologies, and conclusions to ensure transparency and proper legal use.

### Legal Hold
A legal hold is a process initiated by legal professionals to ensure that data is preserved for potential litigation. The steps involved include:
- **Hold Notification**: Notifies individuals about the need to preserve specific data.
- **Separate Repository**: Maintains electronically stored information (ESI) separately for easy access during legal proceedings.
- **Ongoing Preservation**: There is a continuous obligation to preserve data once a legal hold is in effect.

### Chain of Custody
Maintaining the integrity of evidence throughout the forensic process is critical:
- **Integrity**: The chain of custody ensures that evidence is not tampered with or altered.
- **Documentation**: Every person who accesses the evidence must be logged, and digital signatures or hashes are used to protect the evidence from tampering.
- **Storage**: Evidence must be properly sealed, labeled, and cataloged for secure storage.

### Acquisition
Data acquisition is the first step in the forensic process, involving the extraction of relevant data:
- **Sources**: Data can come from various sources, such as disk drives, RAM, firmware, OS files, and network logs.
- **Virtual Systems**: Capture snapshots of virtual machines, including all data and configurations.
- **Mobile Devices**: Gather data from mobile devices, including logs, apps, and system files.

### Reporting
Documenting the findings is essential for both internal and legal purposes:
- **Summary**: An overview of the security event or breach.
- **Detailed Process**: Step-by-step description of how data was acquired, preserved, and analyzed.
- **Findings**: A thorough analysis of the data and how it links to the event.
- **Conclusion**: Professional results based on the analysis, suitable for use in court or other legal proceedings.

### Preservation
Ensuring that collected data remains unaltered is critical:
- **Isolation**: Data must be isolated to prevent unauthorized access or alteration.
- **Data Collection**: Work from copies of the original data to preserve the integrity of the original.
- **Live Collection**: Sometimes, live data collection is necessary, particularly when data is encrypted or unavailable after powering down a device.
- **Best Practices**: Follow legal and technical standards to ensure the data’s admissibility in court.

### E-discovery
E-discovery focuses on gathering electronic documents for legal processes:
- **Collection**: Data is collected to meet legal requirements without considering the intent behind it.
- **Forensics**: In contrast, digital forensics involves recovering and analyzing deleted or altered data from devices.
- **Collaboration**: Forensic experts collaborate with e-discovery teams to recover and interpret missing or hidden data on storage devices.

# 4.9 Log Data

Log data is crucial for monitoring, analyzing, and troubleshooting security incidents. It provides detailed records of various security-related activities and events across systems and networks.

### Security Log Files
These logs provide detailed security-related information:
- **Traffic Flows**: Record blocked and allowed traffic.
- **Exploit Attempts**: Document any detected exploit attempts.
- **URL Categories**: Logs blocked URL categories.
- **DNS Sinkhole Traffic**: Captures traffic directed to a sinkhole for malicious domains.
- **Traffic Documentation**: Provides a summary of attack information, often correlated with other data sources for analysis.

### Firewall Logs
Firewall logs capture detailed information about network traffic:
- **Source/Destination IP**: Logs the originating and destination IP addresses of network traffic.
- **Port Numbers**: Records the source and destination ports.
- **Next-Generation Firewalls (NGFW)**: Logs more advanced data such as application usage, URL filtering categories, and suspicious traffic anomalies.

### Application Logs
Application-specific logs vary greatly depending on the application:
- **Windows**: Event Viewer and application-specific logs.
- **Linux/MacOS**: Logs stored in `/var/log`.
- **SIEM Filtering**: Security Information and Event Management (SIEM) systems can be used to parse these logs, filtering out unneeded information.

### Endpoint Logs
Endpoints often serve as the entry point for attacks:
- **Devices**: Includes phones, laptops, tablets, desktops, etc.
- **Event Types**: Includes logon events, policy changes, system events, processes, and account management activities.
- **SIEM Correlation**: Endpoint logs feed into SIEM systems for correlation with other security events, such as Intrusion Prevention System (IPS) logs.

### OS-Specific Security Logs
Operating system security logs track important security-related activities:
- **Brute Force Attacks**: Attempts to access accounts through repeated incorrect logins.
- **File Changes**: Logs tracking unauthorized file modifications.
- **Authentication Details**: Logs associated with login attempts and successes/failures.
- **Filtering**: OS logs may require filtering to focus on significant security-related events.

### IPS/IDS Logs
Intrusion Prevention and Detection System logs provide data on potential vulnerabilities:
- **Common Data Points**: Includes timestamp, attack type/class, source, and destination IP/port.
- **Vulnerabilities**: Helps identify predefined vulnerabilities based on patterns.

### Network Logs
Logs from network infrastructure devices such as switches, routers, and VPN concentrators:
- **Network Changes**: Logs updates and changes to routing tables and configurations.
- **Authentication Issues**: Tracks failed or unauthorized authentication attempts.
- **Security Issues**: Records any network-related security incidents.

### Metadata
Metadata provides essential context about other data, making it easier to understand, locate, and manage:
- **Email**: Includes sender, destination, subject, and timestamp.
- **Mobile**: Logs information like phone type, location (GPS coordinates).
- **Web**: Includes OS, browser type, and IP address of the user.
- **Files**: Contains file details such as name, owner, and related metadata like phone numbers and titles.

### Vulnerability Scans
These scans detect potential security weaknesses within the network:
- **Security Controls**: Identifies missing firewalls, antivirus software, or misconfigurations.
- **Vulnerabilities**: Detects real vulnerabilities, including outdated software or open shares.

### Automated Reports
SIEM systems often include report generators to automate the process of generating common security reports:
- **Common Reports**: Helps in tracking security incidents, compliance, and vulnerabilities.

### Security Operations Centre Dashboard
A real-time dashboard used to monitor the status of the network and security infrastructure:
- **Real-Time Status**: Displays the most critical information, including potential threats and incidents.

### Packet Capture
Packet capture tools are used for troubleshooting complex network or application issues:
- **Network Traffic**: Captures detailed traffic data, including packet-level analysis to identify unknown or suspicious traffic.
</details>

<details>
<summary>5.0 Security Program Management Oversight</summary>

# 5.1 Security Policies

Security policies are critical in ensuring the security and stability of an organization's information systems. These policies define high-level strategies and provide the guidelines necessary for implementing security controls and maintaining the CIA triad: Confidentiality, Integrity, and Availability.

### Security Policy Guidelines
A security administrator's primary goal is to uphold the CIA triad, focusing on:
- **High-Level Strategies**: Outlines the organization's security approach, including data storage requirements and procedures for handling security events.
- **Detailed Security Goals**: Specifies actions like appropriate Wi-Fi usage and remote access requirements.
- **"What" and "Why"**: Security policies define the purpose of security practices, whereas technical security controls (such as firewalls and encryption) define the "how" of their implementation.

### Information Security Policies
An information security policy is a comprehensive set of rules aimed at maintaining the CIA triad:
- **Compliance Requirements**: Ensures adherence to legal and regulatory obligations.
- **Security Procedures**: Outlines actions taken during incidents or breaches.
- **Roles and Responsibilities**: Details the security duties of employees, departments, and stakeholders.

### Acceptable Use Policy (AUP)
An AUP defines what is considered acceptable use of company assets and technology:
- **Documentation**: Clearly outlines what is allowed and what is prohibited in terms of internet, phone, and device usage.
- **Rules of Behaviour**: Often forms part of a larger policy aimed at limiting legal liability for the organization.
- **Legal Protection**: Protects the organization from misuse and ensures that users understand their responsibilities.

### Business Continuity (BC)
Business continuity planning ensures that an organization can continue its operations during and after a disruption:
- **Disruptions**: Address how disasters (natural or otherwise) can cause interruptions to normal operations.
- **Alternatives**: Establish manual procedures, such as paper receipts or phone approvals, to maintain critical operations when automated systems fail.
- **Planning**: Prepares the organization for potential disruptions, reducing downtime and maintaining essential services.

### Disaster Recovery Plan (DRP)
A disaster recovery plan is a subset of business continuity planning, focusing specifically on how the organization will recover from a disaster:
- **Recovery Location**: Identifies where business operations will resume after a disaster.
- **Data Recovery**: Details methods for recovering lost data, including backups.
- **Restoration of Applications**: Specifies steps to restore essential applications.
- **Team and Availability**: Ensures the IT team and employees are available to implement recovery procedures.

### Security Incidents
Security incidents are events that may compromise the organization's information or network security:
- **Phishing Attacks**: An employee clicks a phishing email, which installs malware.
- **DDoS Attacks**: Distributed Denial of Service (DDoS) attacks, often carried out by botnets.
- **Data Theft**: Loss of confidential data, which may be sold or publicly disclosed.

### Incident Response Roles
- **Incident Response Team (IRT)**: A trained group of professionals responsible for responding to security incidents.
- **IT Security Management**: Provides resources and personnel to address incidents effectively.
- **Compliance Officers**: Ensure that response actions comply with regulations.
- **Technical Staff**: Includes experts who manage the technical aspects of an incident response.

### NIST SP800-61, Computer Security Incident Handling Guide
This framework outlines the lifecycle of handling a security incident:
1. **Preparation**: Preparing resources and plans before an incident occurs.
2. **Detection and Analysis**: Identifying and assessing the incident.
3. **Containment, Eradication, and Recovery**: Limiting damage, removing threats, and restoring systems.
4. **Post-Incident Activity**: Reviewing the incident and improving future response strategies.

### Change Management
Change management ensures that modifications to systems, such as software upgrades or configuration changes, are performed in a controlled and secure manner:
- **Clear Policies**: Outlines the process for making changes, including approval workflows.
- **Frequency and Duration**: Defines how often changes can occur and how long the change process will take.
- **Fallback Procedures**: Details how to revert to previous configurations in case of failure.

# 5.1 Security Standards

Security standards are formal definitions for implementing security technologies and processes within an organization. They serve to ensure consistency, reduce risks, and promote security best practices across the organization. Security standards can be written in-house or based on well-established frameworks, such as ISO and NIST.

### Security Documentation
- **Complete Documentation**: Clear documentation of security standards reduces security risks by ensuring that everyone understands the expectations and requirements.
- **Customization**: Standards can be tailored to an organization’s unique needs, but adopting globally recognized standards like ISO or NIST can help align the organization with industry best practices.

### Password Policies
- **Complexity Requirements**: A formal password policy should specify acceptable password complexity, including length, character types, and expiration rules.
- **Authentication Methods**: Standardize authentication methods, such as using LDAP linked to the Active Directory (AD) database for centralized account management. Local accounts should be avoided.
- **Password Resets**: Establish secure password reset policies to prevent unauthorized access and ensure that resets are properly controlled.
- **Additional Password Rules**: Policies should also define frequency for password changes, how passwords are securely stored (e.g., hashing), and other related security measures.

### Access Control Policies
- **Access Rights**: Policies should define what types of information employees can access and at what times, ensuring the principle of least privilege is applied.
- **Access Control Models**: Determine the type of access control model used (e.g., role-based access control) and document how users are granted access.
- **Privilege Documentation**: Ensure all access rights are properly documented and controlled, including how access can be removed when no longer required.

### Physical Security Policies
- **Physical Access**: Define rules for granting physical access to facilities, distinguishing between employee and visitor access privileges.
- **Physical Security Systems**: Specify security measures like electronic door locks, security cameras, motion detection, and alarm systems, and outline how they are monitored and maintained.

### Encryption Standards
- **Password Storage**: Establish standards for securely storing passwords, including using strong hashing algorithms and salt to protect data.
- **Data Encryption**: Define encryption standards for different states of data:
  - **Data in Use**: Techniques to secure data being actively processed.
  - **Data in Transit**: Encryption protocols like TLS or VPN for protecting data as it moves across networks.
  - **Data at Rest**: Standards for encrypting stored data, including databases and file systems, to ensure it remains secure even if compromised.
- **Encryption Algorithms**: Select appropriate encryption algorithms (e.g., AES) based on the sensitivity of the data and regulatory requirements.

# 5.1 Security Procedures

Security procedures define structured approaches to managing key aspects of an organization’s security, including change management, onboarding/offboarding, playbooks, monitoring, and governance. These procedures are essential for maintaining operational integrity and reducing risks.

### Change Management
- **Scope of Change**: Clearly define the scope of the change to avoid misunderstandings or unintended consequences.
- **Risk Analysis**: Assess the risks associated with the change to determine the potential impact on security and operations.
- **Change Plan**: Develop a comprehensive plan outlining which parts of the system will be affected and how the change will be implemented.
- **End-user Approval**: Obtain approval from relevant stakeholders, particularly those affected by the change.
- **Change Control Board**: Present the change proposal to a change control board for review and approval.
- **Backout Plan**: Prepare a backout plan to roll back the change if it causes issues or fails.
- **Documentation**: Ensure all changes are thoroughly documented, including the reasons for changes and any troubleshooting actions.

### Onboarding
- **IT Agreements**: Ensure that employees sign any necessary IT-related agreements, such as Acceptable Use Policies (AUP).
- **Account Creation**: Create user accounts and assign the appropriate access based on their role and department.
- **Provisioning IT Hardware**: Provide the necessary hardware (laptops, tablets, etc.) with preconfigured settings, ensuring they are ready for immediate use.

### Offboarding
- **Pre-planned Process**: Offboarding should be planned in advance to ensure a smooth transition when an employee exits the organization.
- **Handling of Hardware and Data**: Specify how company hardware will be returned and what happens to data stored on the devices.
- **Account Deactivation**: Deactivate user accounts, and where appropriate, delete them, ensuring that access is revoked immediately.

### Playbooks
- **Conditional Steps**: Playbooks outline step-by-step procedures for specific security events, such as investigating a data breach or handling an incident.
- **SOAR Integration**: Playbooks are often integrated with SOAR platforms, which automate and orchestrate tasks, improving efficiency.
- **Automation**: Automate repetitive tasks to minimize human error and save time, such as generating reports or performing initial checks.

### Monitoring and Revision
- **Security Posture Updates**: Continuously assess and update security measures to address evolving threats.
- **Procedure and Playbook Revisions**: Regularly review and update security procedures and playbooks to reflect new challenges or weaknesses.
- **New Security Concerns**: As new threats emerge, procedures may need to be revised or expanded to address them.

### Governance Structures
- **Boards**: Governance boards set the high-level tasks and requirements for security procedures.
- **Committees**: Committees, composed of subject-matter experts, analyze the board’s tasks, evaluate options, and make recommendations.
- **Government Entities**: External entities may influence security procedures, especially when legal, regulatory, or political considerations are involved.
- **Centralized vs Decentralized Governance**:
  - **Centralized**: Decision-making is concentrated within a single group or location.
  - **Decentralized**: Decision-making is spread across multiple individuals or locations, allowing for a broader input in decision-making.

# 5.1 Security Considerations

Security considerations span regulatory, legal, industry-specific, and geographical factors that shape how an organization protects its data and adheres to required standards.

### Regulatory Considerations
- **Security Processes**: Regulatory frameworks often mandate foundational security measures, including logging, data storage, protection, and retention.
- **Logging and Data Storage**: Regulations often require strict guidelines for how data is logged and stored, ensuring it is accessible for auditing and protection purposes.
- **HIPAA**: Specific to the healthcare industry, HIPAA establishes stringent standards for the storage, use, and transmission of healthcare-related data, with a focus on patient privacy.

### Legal Considerations
- **Formal Procedures**: Security teams must adhere to formal processes for handling illegal activities, breaches, or legal hold scenarios.
- **Breach Notifications**: Legal obligations exist to notify affected parties in the event of a security breach, often governed by local or international law.
- **Challenges with Cloud Computing**: The movement of data across borders without human intervention can complicate legal compliance, as different jurisdictions may have different laws regarding data protection.
- **Adherence to Legal Guidelines**: The security team must ensure all processes align with relevant legal guidelines to avoid legal repercussions.

### Industry-Specific Considerations
- **Electrical Power and Public Utilities**: Systems must be isolated and protected with specific controls to prevent disruption, ensuring the integrity and availability of critical services.
- **Healthcare Industry**: Data encryption, secure storage, and detailed access logs are required to protect sensitive health data, with an emphasis on preventing unauthorized access and ensuring compliance with standards like HIPAA.

### Geographical Security Considerations
- **Local and Regional**: Security measures must address local concerns, including the protection of city and state government records, as well as ensuring uptime and availability for public-facing services.
- **National**: Federal governments and defense agencies have national-level security concerns, requiring comprehensive measures to protect sensitive national information and infrastructure.
- **Global**: For multinational companies, legal and security concerns vary widely across jurisdictions. These organizations must navigate the complexities of international regulations and legal frameworks to ensure global compliance.

# 5.1 Data Roles and Responsibilities

Data roles are essential to understanding how data is managed, protected, and processed within an organization. These roles often go beyond technical responsibilities and can involve key stakeholders at various levels within the organization.

### High-Level Data Relationships and Organizational Responsibilities
- **Data Owner**: The data owner is accountable for specific sets of data, typically a senior officer in the organization. They are responsible for overseeing the management and protection of the data.
    - Example: The **VP of Sales** is the data owner of customer relationship data, ensuring its proper handling and use.
    - Example: The **Treasurer** is the data owner of financial information, overseeing its security and compliance.

### Key Data Roles

- **Data Controller**: The data controller manages the purposes and means by which personal data is processed. They make decisions about how and why data is collected and used.
    - Example: A company’s internal legal or compliance department might act as the data controller to ensure that data processing aligns with privacy regulations.

- **Data Processor**: The data processor processes personal data on behalf of the data controller, often being a third party or a separate entity within the organization. They handle the data according to the controller's instructions but are not responsible for deciding how the data is used.
    - Example: A cloud services provider that processes and stores company data on behalf of the organization.

- **Data Custodian/Steward**: The data custodian (or steward) is responsible for ensuring the accuracy, privacy, and security of the data. They manage access rights to the data and are responsible for implementing appropriate security controls to protect the data.
    - Example: A security or IT team member who ensures that only authorized users have access to sensitive data and that the data is backed up and protected from unauthorized access.

### Example: Payroll Controller and Processor

- **Payroll Controller**: The payroll department within the company defines payroll amounts, timeframes, and the conditions under which payroll information is processed. They are the data controller.
    - Example: The payroll department ensures that salaries, taxes, and benefits are processed correctly according to company policies and regulations.

- **Payroll Processor**: An external payroll company acts as a data processor, processing payroll data according to the instructions given by the payroll controller. The processor stores and manages employee payroll information.
    - Example: A third-party payroll service provider that stores employee payment records and processes direct deposits.

# 5.2 Risk Management

Risk management is crucial for identifying, assessing, and mitigating potential risks within an organization. It helps prevent issues from becoming critical by understanding vulnerabilities and planning accordingly.

### Key Aspects of Risk Management
- **Managing Potential Risk**: Identifying and addressing risks before they escalate into serious problems.
- **Qualifying Internal and External Threats**: Analyzing potential threats from within the organization (internal) and from outside (external) to determine their impact on security and operations.
- **Risk Analysis**: Helps in planning for contingencies by understanding the potential consequences and likelihood of different risks.

### Types of Risk Assessments

- **Performing a Risk Assessment**:
    - **One-time Assessments**: These are conducted for a specific issue or event. The assessment is designed to address a single risk or vulnerability, and once it's completed, no further action is required unless the risk evolves.
    - **Continuous Assessments**: These are ongoing evaluations. For instance, every change made to a system, such as software or network adjustments, requires a risk assessment as part of the change control process.

- **Ad Hoc Assessments**: These are performed for a specific purpose, usually in response to a particular event or concern.
    - A **committee** is typically formed to carry out the assessment. Once the assessment is completed, the committee is disbanded. There may be no further need to investigate the same risk again unless it recurs.

- **Recurring Assessments**: These assessments occur on regular intervals to ensure that the organization’s security measures remain effective.
    - **Internal Assessments**: These assessments are performed internally every few months, with documentation maintained for each evaluation.
    - **Mandated Risk Assessments**: Some organizations are legally required to conduct regular risk assessments. For example, the **PCI DSS** (Payment Card Industry Data Security Standard) mandates annual risk assessments for companies handling payment card data.

# 5.2 Risk Analysis

Risk analysis helps organizations identify, assess, and prioritize risks based on their likelihood, impact, and the potential costs involved. It can be done qualitatively or quantitatively.

### Types of Risk Assessments

- **Qualitative Risk Assessment**: 
    - Involves identifying significant risk factors and assessing their potential impact using subjective methods. 
    - It is often visualized using tools like **traffic light grids** (red, amber, green) to categorize risks based on their severity and likelihood.

- **Quantitative Risk Assessment**: 
    - Focuses on assigning numerical values to risks to understand their potential impact more precisely.
    - Key metrics in quantitative analysis include:

    - **ARO (Annualized Rate of Occurrence)**: The likelihood that a risk will occur in a year.
    - **Exposure Factor (EF)**: The percentage of an asset’s value that is lost due to an incident. For example, losing 25% of the value of an asset would result in an EF of 0.25.

    **Quantitative Risk Metrics**:

    - **SLE (Single Loss Expectancy)**: The monetary loss if a single event occurs.
        - Formula: **SLE = Asset Value x Exposure Factor**
        - Example: If a laptop valued at $1,000 is stolen (EF = 1.0), the SLE is $1,000.
        
    - **ALE (Annualized Loss Expectancy)**: The expected annual monetary loss from a specific risk.
        - Formula: **ALE = ARO x SLE**
        - Example: If there are 7 laptop thefts a year (ARO = 7), the ALE is $7,000.

### Impact Considerations
Risk can have various impacts, not just financial:
- **Life**: The most critical factor—impacts on human safety and wellbeing.
- **Property**: Risk to buildings, equipment, or physical assets.
- **Safety**: The potential for unsafe work environments.
- **Finance**: The financial consequences of the event.

### Likelihood vs. Probability
- **Risk Likelihood** (Qualitative): A subjective measure of how likely a risk is to occur, such as "rare," "possible," or "almost certain."
- **Risk Probability** (Quantitative): A statistical measure based on historical performance or data.

### Risk Appetite and Tolerance
- **Risk Appetite**: The level of risk an organization is willing to accept in pursuit of its objectives.
    - Example: A highway speed limit set by authorities is an acceptable balance between safety and convenience.
    
- **Risk Tolerance**: The acceptable range of variation from the risk appetite. It represents the level of deviation the organization is willing to accept.
    - Example: A person might tolerate driving 10 mph over the speed limit in favorable conditions, but this tolerance may change under different circumstances (e.g., weather, traffic).

### Risk Register
A **Risk Register** is a tool used to document and manage risks associated with a project or activity.
- **Purpose**: 
    - Identifies and documents risks at each stage of a project.
    - Applies possible solutions and mitigation measures to each identified risk.
    - Monitors the results and effectiveness of risk management actions.
    
- **Key Risk Indicators (KRIs)**: These are metrics that help identify risks that could potentially impact the organization.

- **Risk Owners**: Assigning specific individuals or teams to manage and mitigate particular risks.

### Risk Threshold
The **Risk Threshold** is the point at which the cost of mitigation is at least equal to the value gained from mitigation efforts. It determines when the cost of further risk mitigation outweighs the benefits.

# 5.2 Risk Management Strategies

Risk management strategies are used to handle and mitigate the risks identified through the assessment process. These strategies help organizations make informed decisions on how to address various types of risks.

### Risk Management Strategies

1. **Transfer**: 
   - Move the risk to another party, typically through **cybersecurity insurance** or outsourcing. For example, if an organization faces the risk of a data breach, they may purchase insurance to cover the financial losses associated with the breach.
   
2. **Accept**: 
   - This strategy involves making a **business decision** to accept the risk without any mitigating actions. It's used when the cost of mitigation outweighs the potential impact of the risk.
   
3. **Accept with Exemption**:
   - In some cases, it may not be possible to fully comply with a security policy or regulation. This may be due to technical limitations, lack of resources, or other factors.
   - Exemptions may need to be formally approved by senior management or compliance officers. For example, an organization may accept not implementing a certain security control due to specific constraints.

4. **Accept with Exception**:
   - This is similar to the "accept" strategy, but with **temporary deviations** from internal security policies or procedures.
   - For example, **monthly security updates** must typically be applied within three days. However, a critical software package crashes after updates, requiring an exception to the policy for that particular update.
   
5. **Avoid**:
   - The **avoidance strategy** involves eliminating the risk by **stopping or avoiding a high-risk activity** entirely.
   - For example, if an organization identifies a specific vulnerability in a third-party software they use, they may choose to avoid using that software or switch to a safer alternative.
   
6. **Mitigate**:
   - **Mitigation** involves taking steps to **reduce** the likelihood or impact of a risk. This often includes investing in **security systems**, implementing policies, or enhancing existing defenses to lower the potential for a risk event.
   - For example, an organization may implement stronger firewalls, encryption, or intrusion detection systems to reduce the risk of a cyberattack.

### Risk Reporting
- **Risk Reporting** is the process of creating a formal document that outlines the identified risks and details associated with them.
    - This document is typically **created for senior management** to help them make decisions regarding resource allocation, budgeting, and further security tasks.
    - The risk report will usually include:
        - Identification of risks
        - Detailed information on each risk
        - Proposed strategies for managing or mitigating risks
        - An assessment of the potential impact of each risk

# 5.2 Business Impact Analysis (BIA)

A Business Impact Analysis (BIA) is a critical component in risk management, helping organizations assess the potential impacts of disruptions to their operations. It aims to identify and prioritize critical functions, allowing businesses to plan for recovery and ensure continuity.

### Key Metrics in Business Impact Analysis

- **Recovery Time Objective (RTO)**: 
    - Defines the maximum time allowed to restore a service after a disruption before the business is significantly impacted.
    - Example: If a company’s email server is down, the RTO might be set to 4 hours, meaning the email service should be restored within 4 hours of the incident.
  
- **Recovery Point Objective (RPO)**: 
    - Indicates the maximum amount of data loss an organization is willing to tolerate, measured in time.
    - Example: If the RPO is 1 hour, the organization can afford to lose no more than 1 hour of data in case of a disaster.

### Metrics for System Reliability and Performance

- **Mean Time to Repair (MTTR)**: 
    - The average time it takes to diagnose and resolve an issue, from detection to restoration of service. It reflects the efficiency of the IT response team.
    - Example: If a server crashes, the MTTR would be the average time it takes to get it back online.

- **Mean Time Between Failures (MTBF)**:
    - Represents the predicted time between system failures, calculated based on historical data.
    - Example: If a server experiences 5 failures over a total of 100,000 hours, the MTBF is 20,000 hours.
    - MTBF helps organizations plan for future maintenance and anticipate potential disruptions.

### Business Continuity Planning

The BIA feeds into broader **Business Continuity Planning (BCP)** by ensuring that the organization can resume its most important operations as quickly as possible with minimal data loss.

- **Impact on Critical Functions**: 
    - The BIA identifies key business functions that are essential for the organization’s survival and estimates the financial and operational consequences of a disruption to these functions.
    - Example: The loss of access to customer databases for an e-commerce business would have a major impact on operations and revenue.
  
- **Risk Prioritization**: 
    - Based on the BIA, risks are ranked according to their potential impact and likelihood, allowing organizations to focus on the most critical areas that need protection.

- **Resource Allocation**: 
    - Based on the results of the BIA, resources such as personnel, technology, and budget are allocated to ensure that recovery efforts are adequately supported.
    - Example: High-priority systems may receive additional resources to reduce the RTO and RPO.

# 5.3 Third-party Risk Assessment

Third-party risk assessment is essential for identifying and managing risks associated with vendors and service providers that have access to your organization’s data and systems. This process helps minimize potential security threats and ensures compliance with applicable regulations.

### Key Components of Third-party Risk Assessment

- **Third-party Risk**:
    - Vendors that provide services like payroll processing, customer relationship management (CRM), email marketing, and supply chain management are often given access to sensitive company data.
    - Data shared with cloud-based services or external contractors needs to be properly assessed for risk.
    - Risk assessments categorize each vendor's potential impact and manage the overall exposure through security controls and policies.
    - Contracts are used to define clear expectations between the organization and the third party to mitigate misunderstandings or disputes.

### Risk Management through Testing and Audits

- **Penetration Testing**:
    - Involves simulating an attack on systems to identify vulnerabilities that can be exploited.
    - Penetration testing is often a compliance requirement, ensuring the security of third-party systems and networks.
    - Regular penetration tests should be conducted by third-party specialists, as they bring expertise and an unbiased perspective.
  
- **Rules of Engagement**:
    - Establishes the scope of penetration tests, including IP address ranges, testing devices, emergency contacts, and handling of sensitive data.
    - Helps to avoid misunderstandings between the testing team and the vendor, ensuring the tests are carried out safely.

- **Right to Audit Clauses**:
    - Ensures that organizations can perform regular audits on their third-party vendors to evaluate their security posture.
    - Audits check for compliance with security controls, including access management, password security, VPN controls, and offboarding practices.

- **Evidence of Internal Audits**:
    - Regular internal audits assess the effectiveness of implemented security controls.
    - Involves reviewing security processes and controls to identify weaknesses, and may be required for regulatory compliance.
  
### Supply Chain and Vendor Relationship Management

- **Supply Chain Analysis**:
    - Involves evaluating the components, processes, and flow of goods within a supply chain.
    - Identifies risks and opportunities to enhance the supply chain's performance and reduce vulnerabilities that could impact business operations.
  
- **Independent Assessments**:
    - Engaging external specialists or teams to provide impartial evaluations of third-party risks.
    - These independent reviews help organizations identify potential gaps in vendor security measures.

- **Vendor Selection Process**:
    - Before bringing a third-party vendor on board, a thorough due diligence process is essential.
    - This includes verifying financial stability, checking for past or pending legal issues, conducting background checks, and ensuring there are no conflicts of interest.
  
- **Vendor Monitoring**:
    - Ongoing monitoring of vendor performance and security status is necessary to maintain an active understanding of potential risks.
    - Monitoring can include financial health checks, IT security reviews, and periodic assessments to ensure vendors comply with security requirements.
    - A designated vendor manager should oversee this monitoring process to ensure consistency and accountability.

- **Questionnaires**:
    - Used during due diligence and as part of ongoing vendor monitoring.
    - Organizations should request answers from vendors on their security practices, compliance status, and risk management strategies to evaluate their readiness and reliability.

# 5.3 Agreement Types

In business, different types of agreements govern the terms of service, confidentiality, and expectations between parties. These agreements help define roles, responsibilities, and dispute resolution methods, ensuring a clear understanding between parties.

### Common Agreement Types:

- **Service Level Agreement (SLA)**:
    - Specifies the minimum terms of services provided, including uptime, response time, and performance metrics.
    - Commonly used between customers and service providers to ensure agreed-upon service standards are met.
    - Example: An internet service provider (ISP) may have an SLA that guarantees no more than four hours of unscheduled downtime and promises technician dispatch for repairs. The customer may also be required to keep spare equipment on-site.

- **Memorandum of Understanding (MOU)**:
    - A less formal agreement where both parties agree on the general contents and intentions.
    - Often includes common goals, outlines of future cooperation, and may contain confidentiality clauses.
    - Typically used to establish preliminary agreements or intentions before more formal documents are drafted.

- **Memorandum of Agreement (MOA)**:
    - A more formalized version of an MOU, where both parties agree to the objectives of the agreement but it may not always include legally enforceable promises.
    - Serves as a bridge between informal understanding and formal contracts.

- **Master Service Agreement (MSA)**:
    - A broad, legal contract that outlines terms and conditions for future transactions and engagements.
    - Used to set the foundation for multiple projects, detailing key expectations, deliverables, and responsibilities.
    - Often supplemented by Work Orders (WO) or Statements of Work (SOW), which provide specific lists of tasks or deliverables tied to the broader MSA.

- **Non-Disclosure Agreement (NDA)**:
    - A legal contract that ensures confidentiality between parties. It prevents the disclosure of sensitive information, such as trade secrets or proprietary business data.
    - NDAs can be unilateral (one party discloses information) or mutual (both parties share sensitive information).
    - Requires formal signatures to be enforceable.

- **Business Partner Agreement (BPA)**:
    - Defines the terms of a business partnership, including ownership stakes, decision-making authority, and financial obligations.
    - It also prepares for contingencies such as financial issues, disaster recovery, and other unexpected events.
    - The agreement outlines roles and responsibilities for each party and provides a framework for business operations.

# 5.4 Compliance

Compliance refers to the process of adhering to a series of standards, laws, policies, and regulations that govern business practices. This encompasses a broad range of rules, covering everything from industry-specific standards to general legal obligations, with penalties for non-compliance.

### Key Points:

- **Compliance Overview**:
  - Compliance involves following a catalog of rules, which may vary depending on the industry and jurisdiction.
  - Penalties for non-compliance can include fines, loss of employment, and even incarceration.
  - Compliance requirements can be both **domestic** (within a specific country) and **international** (across borders), making it crucial for multinational organizations to understand global regulations.

### Types of Compliance Reporting:

- **Internal Compliance Reporting**:
  - Organizations monitor and report on their compliance efforts to ensure adherence to laws and internal policies.
  - Large organizations often have a **Central Compliance Officer (CCO)** to oversee these efforts.
  - Internal compliance reports are also provided to customers or potential investors as part of trust-building and transparency.

- **External Compliance Reporting**:
  - External compliance reporting involves providing documentation to regulatory bodies, industry regulators, or third parties.
  - This may involve annual or ongoing reporting, depending on the nature of the regulation.
  - Missing or invalid reports can lead to significant fines or sanctions.

### Regulatory Compliance Examples:

- **Sarbanes-Oxley Act (SOX)**: A U.S. law that mandates strict measures to prevent corporate fraud.
- **Health Insurance Portability and Accountability Act (HIPAA)**: A U.S. law protecting the privacy of health information.
- **Gramm-Leach-Bliley Act (GLBA)**: A U.S. law focused on protecting consumers' personal financial information.

### HIPAA Non-Compliance Penalties:

- **Fines**: 
  - Up to $50,000 for violations, with penalties increasing based on intent (e.g., false pretenses or intent to harm).
  - Maximum civil fines can reach up to $100 per violation, with an annual cap of $25,000 for the same violation.
  
- **Prison Sentences**:
  - Intentional violations can lead to imprisonment, ranging from 1 to 10 years, depending on the severity.

### Consequences of Non-Compliance:

- **Reputational Damage**: 
  - Failing to comply with regulations or experiencing data breaches can lead to significant financial losses, tarnish the organization’s reputation, and impact its stock price.
  
- **Loss of License**:
  - Non-compliance can result in the revocation of business licenses, meaning an organization may no longer be able to sell products or services until it is re-licensed, which can be costly.

### Compliance Monitoring:

- **Internal Monitoring**:
  - Organizations use internal tools to monitor compliance, ensuring that daily operations align with regulatory and internal standards.
  - Formal compliance documentation must be signed off, and individuals are responsible for its accuracy.

- **External Monitoring**:
  - For larger organizations, compliance monitoring may require the use of automation and third-party monitoring systems.
  - These tools collect data from internal systems and individuals, compile it, and report on compliance status, ensuring that both internal operations and third-party relationships remain in compliance.

# 5.4 Privacy

Privacy is a critical aspect of data protection, influenced by evolving legal frameworks that vary across local, national, and global levels. These guidelines govern the collection, storage, and use of personal data and are essential for compliance and safeguarding individuals' rights.

### Privacy Legal Implications:

- **Local/Regional Privacy**:
  - Privacy laws at the local or state level can govern various types of information, such as vehicle registrations, medical licenses, and more.
  
- **National Privacy**:
  - National laws establish privacy guidelines that apply to all citizens within a country, such as **HIPAA** for healthcare data in the U.S. or laws protecting online privacy for children under 13.

- **Global Privacy**:
  - **General Data Protection Regulation (GDPR)**: A European Union regulation focused on personal data protection. It applies to all organizations processing personal data of individuals in the EU and EU area.
    - **Rights under GDPR**:
      - **Right to Access**: Individuals can access their personal data held by organizations.
      - **Right to Rectification**: Individuals can request corrections to their personal data.
      - **Right to Erasure**: Individuals can request the deletion of their personal data (also known as the "right to be forgotten").
      - **Right to Data Portability**: Individuals can transfer their data from one service provider to another.
      - **Right to Object**: Individuals can object to the processing of their data in certain circumstances.

### Data Subject:

- A **data subject** refers to any individual whose personal data is being processed. This can include information such as:
  - **Personal Information**: Name, identification number, address, and more.
  - **Sensitive Information**: Genetic data, physical characteristics, or location data.
  
- Privacy is generally defined from the perspective of the **data subject**, ensuring their rights and protection are prioritized.

### Data Responsibilities:

- **Data Owner**: The individual or role accountable for specific sets of data within an organization.
  
- **Data Inventory and Retention**:
  - **Data Inventory**: A comprehensive list of all data managed by the organization, including its owner, update frequency, and format.
  - **Internal Use**: Data used for internal purposes such as project collaboration, IT security, or quality checks.
  - **External Use**: Data shared with third parties or the public, ensuring compliance with relevant laws and regulations.

# 5.5 Audits and Assessments

Audits and assessments are essential for evaluating the effectiveness of an organization’s cybersecurity posture, compliance with regulations, and identifying vulnerabilities. These evaluations help ensure that proper controls are in place to protect sensitive data and systems.

### Cybersecurity Audit:

A **cybersecurity audit** is a comprehensive review of an organization’s computing environment, which includes:
- **IT Infrastructure, Software, and Devices**: Audits examine hardware, software, and devices used within the organization to assess their security.
- **Policies and Procedures**: Evaluates the effectiveness of existing security policies and procedures in mitigating risks.
- **Vulnerability Identification**: Helps detect weaknesses or vulnerabilities before they are exploited by attackers.
- **Internal or Third-party Audits**: Audits can be conducted internally by the organization or externally by a third-party security expert.
- **Attestation**: An auditor may provide an attestation, which is a formal opinion on the accuracy and reliability of the organization’s security posture.

### Internal Audits:

Internal audits help organizations self-assess their security and compliance:
- **Audit Committee**: Often formed to manage risk and oversee internal audits within the organization.
- **Self-assessments**: The organization may conduct its own evaluations, consolidating results into ongoing reports for review and improvement.
- **Ongoing Monitoring**: Internal audits typically take place at regular intervals to ensure continuous compliance and effectiveness.

### External Audits:

External audits are often mandated by regulations and provide an independent review of an organization's compliance and cybersecurity practices:
- **Regulatory Requirements**: External audits are required by certain laws and regulations, and the frequency and type depend on the specific mandate.
- **Examinations**: Auditors conduct hands-on research, reviewing records and gathering data to assess security and compliance.
- **Assessments**: Auditors may assess the organization’s current activities and provide recommendations for future improvements.

# 5.5 Penetration Test

Penetration testing (pen testing) is a critical component of a proactive cybersecurity strategy, allowing organizations to identify and mitigate vulnerabilities before attackers can exploit them. It includes various perspectives and approaches, and it can be performed in different environments.

### Physical Penetration Testing:

Physical penetration testing assesses the physical security measures of an organization and its facilities:
- **Circumventing System Security**: Physical access to devices can easily bypass system security. A tester may attempt to modify the boot process, boot from alternative media, or replace OS files.
- **Physical Security Assessment**: Just as network security is important, physical security is also crucial. Testing might include attempting unauthorized access to the building, assessing the security of doors, windows, elevators, and the effectiveness of physical security measures (e.g., keycards, security personnel).
- **Key Question**: Can an attacker physically enter the building or server rooms without proper access?

### Penetration Testing Perspectives:

Penetration testing can be approached from several perspectives:

#### Offensive (Red Team):
- **Attack Systems**: The red team acts as attackers, seeking vulnerabilities in systems, networks, and applications.
- **Goal**: Exploit weaknesses to simulate a real-world attack.

#### Defensive (Blue Team):
- **Defend and Detect**: The blue team identifies attacks as they occur, focusing on real-time detection and prevention of unauthorized access.
- **Goal**: Respond to simulated attacks and improve security measures to minimize risks.

#### Integrated:
- **Ongoing Process**: Combining offensive and defensive perspectives in an ongoing cycle. Systems are continuously tested, patched, and re-evaluated for vulnerabilities.
- **Goal**: Establish a proactive, continuous improvement loop for security.

### Working Knowledge:

The level of knowledge a pentester has about the environment impacts the penetration test:

- **Known Environment**: Full disclosure, meaning the tester knows everything about the environment and systems they are testing.
- **Partially Known Environment**: A mix of known and unknown systems, where the tester is provided with certain systems or areas of focus.
- **Unknown Environment**: A "blind" test, where the tester has no prior knowledge about the systems and performs the test without any inside information.

### Reconnaissance:

Reconnaissance is the information-gathering phase, crucial to understanding the target environment before exploiting any vulnerabilities.

#### Passive Reconnaissance:
- **Open-Source Intelligence (OSINT)**: Gathering information from publicly available sources without interacting directly with the target system.
  - Examples include social media, corporate websites, online forums, Reddit, social engineering, or even dumpster diving for physical information.
  - **Goal**: Understand the security posture of the target without revealing your presence.

#### Active Reconnaissance:
- **Direct Interaction**: Actively interacting with the target system or network to gather detailed information.
  - This can include:
    - **Ping Scans**: Identifying active hosts on the network.
    - **Port Scans**: Identifying open ports and services running on the system.
    - **DNS Queries**: Extracting information from the Domain Name System.
    - **OS Scans and Fingerprinting**: Identifying the operating system and version running on a device.
    - **Service and Version Scans**: Identifying running services and their versions to discover potential vulnerabilities.
  - **Goal**: Identify systems' configurations, vulnerabilities, and defensive measures. 
  - **Visibility**: Active reconnaissance will likely be visible in network traffic and system logs.

# 5.6 Security Awareness

Security awareness is a critical element in fostering a security-conscious culture within an organization. It involves training and educating users to recognize risks and avoid security incidents. Here's a breakdown of key components in building an effective security awareness program:

### Phishing Campaigns:

Simulating phishing campaigns helps train users to recognize and avoid phishing attempts.
- **Automated Reporting**: Track and report on incorrect clicks or actions by users, and provide feedback and training tools.
- **Key Phishing Indicators**:
  - **Spelling and Grammatical Errors**: Phishing emails often contain mistakes in spelling and grammar.
  - **Domain Name and Email Inconsistencies**: Look for slight differences in domain names or suspicious email addresses.
  - **Unusual Attachments**: Be wary of unexpected attachments, especially if they prompt you to run or open them.
  - **Requests for Personal Information**: Phishing emails often request sensitive information such as passwords or social security numbers.
  - **General Advice**: **Never click a link** or **run an attachment** unless you're certain it's legitimate.

### Anomalous Behaviour Recognition:

Recognizing risky or unusual behavior can help prevent security incidents.
- **Types of Risky Behavior**:
  - **Modifying Hosts Files**: Altering configuration files that control how a system communicates with other devices or networks.
  - **Replacing Core OS Files**: This could indicate malicious activity or tampering.
  - **Uploading Sensitive Files**: Unauthorized uploading of sensitive information to external sites or services.
  - **Unexpected Logins**: Logins from unexpected locations (e.g., a different country) could indicate unauthorized access.
  - **Increased Data Transfers**: Unusual spikes in data transfer may indicate data exfiltration attempts.
  - **Unintentional Behaviors**: Actions like typing incorrect domain names, losing USB drives, or misconfiguring security settings can also pose risks.

### Reporting and Monitoring:

Tracking and analyzing security awareness metrics is essential for improving the program.
- **Automated Monitoring**: Automate tracking of metrics like phishing click rates, password manager adoption, multi-factor authentication (MFA) usage, and password sharing.
- **Incident Types**:
  - **Initial Incidents**: The first occurrence of risky behavior is an opportunity for immediate user training to prevent future incidents.
  - **Recurring Incidents**: Long-term monitoring helps identify frequent issues and provides targeted assistance to users who repeatedly fall into the same traps.

### Development of the Security Awareness Program:

Building an effective security awareness program involves planning, training, and monitoring.
- **Establish Roles**: Create a security awareness team responsible for roles in training, monitoring, policy creation, and ongoing improvement.
- **Minimum Awareness Level**: Set a baseline level of awareness for all employees and ensure training is aligned with job functions.
- **Integrate Compliance Mandates**: Include relevant regulatory requirements, such as PCI DSS, HIPAA, and GDPR, into the awareness program.
- **Define Metrics**: Establish clear metrics to measure the effectiveness of the training program and assess performance. Continuously improve areas with lower performance.
  
### Execution of the Awareness Program:

The execution phase involves developing and delivering training to employees.
- **Training Materials**: Develop training materials that are accessible to users in various formats (e.g., workshops, videos, quizzes, written guides).
- **Document Success Metrics**: Clearly define how success will be measured (e.g., reduced phishing click rates, higher MFA adoption).
- **Stakeholder Identification**: Identify key stakeholders (e.g., IT department, security team, HR) who will support and advocate for the program.
- **Deployment**: Roll out the training materials across the organization and monitor effectiveness over time.

# 5.6 Security Training

Security training is an essential component in protecting an organization's sensitive data and ensuring that all users understand their responsibilities and best practices for security. This involves not only educating employees but also contractors, third parties, and other stakeholders who interact with the organization's systems.

### Key Training Aspects:

#### **Training Before Providing Access:**
- Before granting system access, it’s crucial to train users on detailed security requirements.
- Training should be tailored to each user's specific role and responsibilities, addressing their unique security needs.

#### **Specialized Training:**
- Each user, depending on their role, should undergo specialized training to meet specific security responsibilities.
- **Third-Parties and Contractors**: Training applies not only to internal users but also to external entities such as contractors, suppliers, and partners who interact with the organization's systems.

#### **Documentation and Records:**
- Keep detailed records of who has been trained and who hasn't to ensure compliance and identify gaps in training.

### **User Guidance and Training:**

#### **Policy and Handbooks:**
- **Document Security Requirements**: All security requirements should be clearly documented and provided to users.
  - Access to policy guidelines should be readily available, preferably online.
  - Ensure policies are referenced in the employee handbook for easy access and reminders.
  
#### **Situational Awareness:**
- Users should always be on the lookout for potential threats. This includes:
  - **Software Attacks**: Identifying phishing emails, malicious links, or suspicious attachments.
  - **Physical Attacks**: Being vigilant about unauthorized access through unlocked building doors or malicious USB drives.
  
#### **Insider Threats:**
- Insider threats can be difficult to guard against, but several strategies can help mitigate risks:
  - **Multiple Approvals**: For critical processes, ensure that multiple approvals are required to reduce the likelihood of malicious actions.
  - **Monitoring**: Continuously monitor files and systems for any suspicious activity.

#### **Password Management:**
- Guide users on best practices for password management:
  - Establish standards for creating strong passwords.
  - Encourage the use of password managers to store and generate complex passwords.

#### **Removable Media and Cables:**
- **USB Drives and Cables**: Educate users on the risks posed by unknown USB drives and cables, which could potentially carry malware.

#### **Social Engineering Awareness:**
- Social engineering attacks are common and sophisticated, requiring ongoing training to ensure users can identify and avoid them.
- **User Defense**: Users are the front line of defense, and training should emphasize how to handle social engineering attacks effectively.

#### **Operational Security:**
- Teach users to think from an attacker’s perspective:
  - **Sensitive Data Identification**: Users must understand what constitutes sensitive data and how to keep it secure.
  - **Privacy**: Encourage practices that prioritize keeping sensitive information confidential.

#### **Hybrid/Remote Work Environments:**
- Remote work introduces unique security risks that need to be addressed:
  - **Home Security**: Employees working from home may be vulnerable to social engineering or physical threats if they don't have the same level of security as in-office setups.
  - **VPN and Endpoint Security**: Emphasize the use of secure VPN connections and additional endpoint security for remote workers.
  
#### **Additional Endpoint Security:**
- **VPN Access Policies**: Establish and enforce security policies for accessing the network remotely, including the use of multi-factor authentication (MFA) and secure VPNs.


</details>
