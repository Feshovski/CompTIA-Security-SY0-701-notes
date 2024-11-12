# CompTia-Security-SY0-701-notes

Hi All, I completed my exam on the 16th of August 2024 after roughly a month of self study. I used a range of resources found on [O'Reilly ](https://www.oreilly.com/), ranging from the [certification guide](https://www.oreilly.com/library/view/comptia-security-sy0-701/9781835461532/), a video course by [Sari Green](https://www.oreilly.com/library/view/comptia-security-sy0-701/9780138251062/) and [practice exams.](https://www.oreilly.com/library/view/comptia-security-sy0-701/9780138225568/) 

ProfesserMesser's [YouTube Playlist, CompTIA SY0-701 Security+ Training Course ](https://www.youtube.com/playlist?list=PLG49S3nxzAnl4QDVqK-hOnoqcSKEIDDuv) was my main study resource where most of my notes were derived from, I used other tools to help me better understand concepts I was struggling to understand. 

[Free labs](https://www.101labs.net/comptia-security/) I used to help wrap my head around some concepts**note that you will need your own VM with a Linux distro installed to complete these.**

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

#### Preventive: Blocks access to a resource
**Prevent access:**
- Firewall rules
- Follow security policy
- Guard shack checks all identification
- Enable door locks

#### Deterrent: Discourages an intrusion attempt, does not directly prevent access
**Makes an attacker think twice:**
- Application splash screens
- Threat of demotion
- Front reception desk
- Posted warning signs

#### Detective: Identify and log an intrusion attempt, may not prevent access
**Find the issue:**
- Collect and review system logs
- Review login reports
- Regularly patrol the property
- Enable motion detectors

#### Corrective: Apply a control after an event has been detected, reverse the impact of an event, and continue operating with minimal downtime
**Correct the problem:**
- Restoring from backups can mitigate a ransomware infection
- Create policies for reporting security issues
- Contact law enforcement to manage criminal activity
- Use a fire extinguisher

#### Compensating: Control using other means, existing controls aren't sufficient, may be temporary
**Prevent the exploitation of a weakness:**
- Firewall blocks a specific application instead of patching the app
- Implement a separation of duties
- Require simultaneous guard duties
- Generator used after power outage

#### Directive: Direct a subject towards security compliance, a relatively weak security control
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

#### Policy Decision Point (PDP):
- There's a process for making an authentication decision.

#### Policy Engine:
- Evaluates each access decision based on policy and other information sources.
- Grant, deny, or revoke access.

#### Policy Administrator:
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

#### Allow List:
- Nothing runs unless it's approved.
- Very restrictive.

#### Deny List:
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

#### Out-of-band key exchange: Don't send the symmetric key over the net:
- Telephone
- Courier
- In-person, etc.

#### In-band key exchange: On the network:
- Protect the key with additional encryption.
- Use asymmetric encryption to deliver a symmetric key.

#### Real-time encryption/decryption: Share a symmetric session key using asymmetric encryption:
- Client encrypts a random (symmetric) key with a server's public key.
- The server decrypts this shared key and uses it to encrypt data.
- This is the session key.

#### Symmetric key from asymmetric keys:
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

#### Common Steganography Techniques:
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

#### The Hash Should Be Unique
- Different inputs should never create the same hash.
- If they do, it's a **collision**.
![image](https://github.com/user-attachments/assets/ed896ca3-efdd-4e4a-a64d-2fab905b7c4e)

#### MD5 Has a Collision Problem
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

#### Sign with the Private Key
- The message doesn't need to be encrypted.
- **Nobody else can sign this**.

#### Verify with the Public Key
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

#### Message-Based Vectors
- **Overview**: A major vector, often through phishing.
- **Methods**:
  - **Email**: Malicious links, phishing sites.
  - **SMS (Smishing)**: Phishing attacks via text messages.

#### Phishing Attacks
- **Common Forms**: Links in emails, texts, or IMs.
- **Intent**: Often to deliver malware or engage in social engineering scams like invoice or cryptocurrency scams.

#### Image-Based Vectors
- **Difficulty**: Harder to identify threats embedded in images.
- **Methods**:
  - **SVG Files**: Can contain HTML injections or JavaScript.
  - **XSS (Cross-Site Scripting)**: Injects malicious scripts into trusted applications.

#### File-Based Vectors
- **Overview**: Malicious code hidden in files.
- **File Types**: PDF, ZIP/RAR, and other compressed formats.

#### Voice Call Vectors (Vishing)
- **Methods**:
  - **Spam over IP**: High-volume automated calls.
  - **War Dialing**: Attempting to connect to multiple phone numbers.
  - **Call Tampering**: Disrupting voice calls, often as a form of DoS.

#### Removable Device Vectors
- **Device Types**: USB flash drives, among others.
- **Risks**:
  - **Air-gapped Networks**: Can introduce malware even in isolated systems.
  - **Data Exfiltration**: Massive data extraction with zero network bandwidth.

#### Vulnerable Software Vectors
- **Overview**: Security flaws in software require frequent updates.
- **Categories**:
  - **Client-Based**: Vulnerabilities in user-installed applications.
  - **Agentless**: Compromised server software affecting all clients.

#### Unsupported Systems Vector
- **Risk**: Unpatched, outdated systems pose significant vulnerabilities.
- **Solution**: Maintain an inventory and ensure all systems are up-to-date.

#### Unsecure Network Vectors
- **Types**:
  - **Wireless**: Outdated protocols (e.g., WEP, WPA), unsecured networks.
  - **Wired**: Lack of security measures like 802.1X.
  - **Bluetooth**: Vulnerable to reconnaissance and exploitation.

#### Open Service Ports
- **Risk**: Open TCP/UDP ports increase attack surface.
- **Challenge**: Each open port presents a potential entry point.

#### Default Credentials
- **Issue**: Default usernames and passwords can provide attackers with administrator access.

#### Supply Chain Vectors
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

#### Vishing
- **Definition**: Voice phishing conducted over the phone or voicemail.
- **Common Tactics**:
  - **Caller ID Spoofing**: Making the call appear from a trusted source.
  - **Fake Security Checks**: Posing as bank or tech support representatives.

#### Smishing
- **Definition**: SMS phishing done via text message.
- **Common Tactics**:
  - **Spoofed Sender ID**: Messages appear to be from a trusted source.
  - **Link Forwarding**: Requests to click links or provide personal details.

#### Phishing with Different Bait
- **Definition**: Combines phishing with other social engineering tactics.
- **Goal**: Broaden the approach to increase the chances of success.

# 2.2 Impersonation

**Definition**  
Impersonation occurs when an attacker pretends to be someone they are not in order to trick individuals into revealing personal information.

---

### Tactics in Impersonation

#### Eliciting Information
- **Technique**: Extracting information from a target without them realizing it.
- **Common Scenarios**: Often used in vishing, where attackers find it easier to extract information over the phone.
- **Psychology**: Relies on well-documented psychological techniques to manipulate the victim.

#### Identity Fraud
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

#### How TOCTOU Works:
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

#### Non-persistent (Reflected) XSS Attack
- In a reflected XSS attack, the website allows scripts to run in user inputs, such as search boxes or form fields.
- The attacker sends a malicious link to the victim, which, when clicked, runs a script that can send the victim's credentials, session IDs, or cookies to the attacker.
- The script is embedded in the URL and executes in the victim's browser, often without the victim knowing.
  
#### Persistent (Stored) XSS Attack
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

#### Firmware
- Firmware is the software that resides inside hardware devices, often referred to as the operating system of the device.
- Vendors are typically the only ones who can fix hardware vulnerabilities, provided they are aware of the issue.

#### End-of-Life (EOL)
- **End-of-life (EOL)** refers to when a manufacturer stops selling a product.
- Even after EOL, the manufacturer may continue supporting the product for a period.
- **End-of-service life (EOSL)** occurs when the manufacturer stops selling a product, and support is no longer available.
- No security patches or updates are issued once EOSL is reached, which increases the security risks associated with using that device.
- Some manufacturers may offer a premium support option, but ongoing security updates are not guaranteed.

### End-of-Service Life (EOSL) Concerns
- **EOSL** is a significant security concern, especially for legacy platforms. Without continued support or security patches, devices become vulnerable to new exploits.
- Manufacturers typically release security patches as part of normal operations, but this ends once the device reaches EOSL.

#### Legacy Platforms
- A legacy platform is a device running an older operating system, outdated applications, or old middleware without current updates.
- These devices may be at risk due to their use of outdated systems, often at EOL or EOSL.
- Devices running legacy platforms require additional security protections, such as more stringent firewall rules and updated intrusion prevention signatures, to mitigate the risks associated with outdated software.

# 2.3 Virtualization Vulnerabilities

Virtualization vulnerabilities share similarities with physical machine vulnerabilities, but they introduce unique risks due to the nature of virtual environments. These vulnerabilities can include issues like local privilege escalations, command injection, and others specific to virtualized systems.

### Key Concepts

#### Virtual Machine Escape Protection
- **Virtual machine escape** occurs when an attacker breaks out of the virtual machine (VM) and interacts with the host operating system or hardware.
- If an attacker successfully escapes the VM, they gain significant control over the host system, which represents a huge security exploit.
- Protecting against VM escape is critical to maintaining the security of both the virtual and host environments.

#### Resource Reuse
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

#### Attack Process:
1. **Interception of Data**: The attacker captures the original data transmission.
2. **Modification and Retransmission**: The attacker may alter the data before sending it again.
3. **Authentication Bypass**: If the data contains authentication information, the attacker can bypass security measures.

To carry out this attack, the attacker needs access to raw network data, which could be obtained through methods like **network taps**, **ARP poisoning**, or **malware on the victim’s system**.

#### Pass the Hash (PtH) Attack:
In a **Pass the Hash** attack, an attacker captures the hashed version of a password and uses it to authenticate to a remote server or service.

**Steps involved**:
1. **Hash Capture**: The attacker obtains a hashed password (e.g., from network transmission or memory).
2. **Hash Usage**: The attacker uses the captured hash to authenticate to systems like **NTLM**.
3. **Authentication**: The attacker gains access without needing to know the original password.

**Mitigation**:
- **Salting passwords**: Adding a unique value to the password before hashing can make hash values more secure.
- **Encryption**: Protecting the transmission of passwords with encryption can prevent hash capture.
- **Session IDs**: Using session identifiers for authentication reduces reliance on password hashes.

#### Browser Cookies:
Cookies store information on your browser for tracking, session management, and personalization. While not inherently executable, they present a **privacy risk** if stolen by attackers. They are typically not a direct security threat unless the attacker can access them.

#### Session Hijacking (Sidejacking):
Session hijacking, or **sidejacking**, occurs when an attacker intercepts a session ID to impersonate the user. This can happen if the session ID is not properly encrypted or protected.

#### Header Manipulation:
Attackers may manipulate HTTP headers to modify or hijack sessions.

**Preventing Session Hijacking**:
- **Encrypt end-to-end**: Ensure session IDs are encrypted to prevent interception.
- **Use HTTPS**: Websites should enforce HTTPS to secure communication.
- **Additional security**: Tools like the **HTTPS Everywhere** browser extension or enforcing **Force-TLS** can enhance session security.
- **VPN**: Encrypting sessions to a VPN concentrator further secures the connection.

# 2.4 Malicious Code

Malicious code refers to software or scripts used by attackers to exploit vulnerabilities, gain unauthorized access, or cause damage to systems. This can include techniques such as **social engineering**, **default credentials**, or exploiting **misconfigurations**, which may not require advanced technical skills but still pose serious risks to even well-secured systems.

#### What is Malicious Code?
Malicious code is any software or code that an attacker uses to gain access to a system or exploit its vulnerabilities. This can include:
- **Executable files**
- **Scripts**
- **Macro viruses**
- **Worms**
- **Trojan horses**

#### Protection Against Malicious Code:
Defense against malicious code requires multiple layers of security, including:
- **Anti-malware software**
- **Firewalls**
- **Continuous software updates and patches**
- **Secure computing habits**

#### Example: WannaCry Ransomware
One notable example is **WannaCry**, a ransomware attack that exploited a vulnerability in **Windows SMBv1**. The malicious executable allowed arbitrary code execution, enabling the malware to spread rapidly across networks, encrypting files and demanding ransom.

Malicious code is often opportunistic, and while systems may be well-secured, it's essential to maintain proactive security measures and vigilance.

# 2.4 Application Attacks

Application attacks target vulnerabilities in software programs and web applications, exploiting weaknesses in the code or design. These attacks can lead to serious security breaches, allowing attackers to gain unauthorized access, execute arbitrary code, or manipulate data.

#### Code Injection
Code injection occurs when attackers add malicious code into an application's input fields, which the program then processes. This is often enabled by poor programming practices that fail to properly handle input and output.

- **Common injection types**: HTML, SQL, XML, LDAP, etc.
- **Risk**: Allows attackers to execute unintended commands or alter the application's behavior.

#### Buffer Overflow
A buffer overflow happens when a program writes more data to a buffer than it can handle. Buffers are temporary storage areas for data, and when data exceeds the buffer's size, it can overwrite adjacent memory, leading to crashes or exploitable conditions.

- **Consequences**: Crashes, arbitrary code execution, data corruption, and security bypass.
- **Mitigation**: 
  - **Bounds checking**: Ensure data fits within buffer limits.
  - **Safe functions**: Use functions with built-in checks like `strncpy` instead of `strcpy`.
  - **Address Space Layout Randomization (ASLR)**: Randomize memory addresses to make exploitation harder.
  - **Data Execution Prevention (DEP)**: Mark certain memory areas as non-executable to block injected code.
  - **Static and Dynamic Analysis**: Use tools to detect and fix vulnerabilities in code.

#### Privilege Escalation
Privilege escalation occurs when attackers gain higher levels of access to a system by exploiting bugs, design flaws, or vulnerabilities, allowing them to perform actions normally restricted to privileged users.

- **Mitigation**: 
  - **Patch vulnerabilities**: Keep software up to date.
  - **Anti-virus/Anti-malware**: Ensure software is current and capable of detecting known threats.
  - **Block known exploits**: Prevent known vulnerabilities from being exploited.
  - **DEP & ASLR**: Protect memory and prevent unauthorized code execution.

#### Cross-Site Request Forgery (CSRF)
Cross-Site Request Forgery (CSRF) tricks a user’s browser into executing unwanted actions on a different website where the user is authenticated. The attacker exploits the trusted relationship between the user’s browser and the website.

- **Risk**: Unauthorized actions, such as transferring funds or posting content, on behalf of the user.
- **Mitigation**: 
  - **Anti-forgery tokens**: Use cryptographic tokens to ensure requests come from trusted sources.
  - **User validation**: Check that each request is valid and originates from a legitimate source.

#### Directory Traversal / Path Traversal
Directory traversal, or path traversal, allows attackers to access files and directories on a server that are outside the scope of the website’s directory. This could give them access to sensitive files, such as configuration files.

- **Risk**: Attackers can browse directories beyond the web server's root, potentially accessing critical system files.
- **Mitigation**: 
  - Ensure proper directory access controls are in place.
  - Avoid using unsafe file paths like `../` in web application code.

# 2.4 Cryptographic Attacks

Cryptographic attacks aim to break the security of encrypted data, often exploiting weaknesses in how cryptographic algorithms or protocols are implemented. While encryption itself is a powerful tool for securing data, poor implementation or outdated protocols can make it vulnerable.

#### Birthday Attack
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

#### Collisions
A **collision** occurs when two different pieces of data produce the same hash. Since hash functions are meant to be unique, a collision undermines the integrity of the hash and potentially the security of the data.

#### Downgrade Attack
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

### 2.5 Segmentation and Access Control

**Segmentation** is a technique used to isolate and secure different parts of a network or system. It is done for several reasons, including improving performance for high-bandwidth applications, enhancing security, and ensuring compliance with regulations.

#### Physical Segmentation
This involves using separate physical devices and infrastructure to create isolated segments within a network or system.
- **Dedicated Hardware**: Different segments are maintained on separate physical hardware such as routers, switches, and cables.
- **Complete Isolation**: Physical separation ensures that segments are entirely isolated, without shared components.
- **High Security**: Because there’s no direct way to traverse between segments without physical access, this method offers a high level of security.
  
**Example**: A corporate network where the finance department has its own dedicated server, switch, and cabling, separate from the other departments.

#### Logical Segmentation
Logical segmentation divides a network into smaller segments using software and network configurations.
- **VLANs**: This is often achieved by using Virtual Local Area Networks (VLANs), which partition a single physical network into multiple logical networks.
- **Access Control**: Traffic between segments is controlled by network devices such as switches and routers that manage traffic based on defined policies.
- **Flexible Configuration**: Logical segmentation is more flexible and easier to reconfigure than physical segmentation, enabling dynamic network management.
  
**Example**: A university network that separates student, faculty, and administrative traffic using VLANs on the same physical network infrastructure.

#### Virtual Segmentation
Virtual segmentation creates isolated virtual environments within a single physical host, typically through virtualization technologies.
- **Virtual Machines (VMs)**: Multiple VMs can run on a single physical server, each with its own operating system and applications, isolated from each other.
- **Hypervisors**: A hypervisor manages the creation and operation of VMs, ensuring proper isolation and resource allocation.
- **Network Virtualization**: Virtual switches and routers can be used to segment network traffic within virtualized environments.
  
**Example**: A cloud service provider hosts multiple virtual servers for different customers on the same physical hardware, using VMs and virtual networks to ensure data and application isolation.

#### Access Control Lists (ACLs)
ACLs are used to control traffic by specifying which users or devices can access specific resources and under which conditions.
- **Restrictions**: ACLs allow traffic based on criteria like source IP, destination IP, port numbers, application types, and even time of day.
- **Risk**: Careful planning is needed when creating ACLs, as improper configuration can lock users or administrators out of critical systems.
  
**Examples of ACL Permissions**:
- **Bob** can read files.
- **Fred** can access the network.
- **James** can access network 192.157.1.0/24 using TCP ports 80, 443, and 8088.

Many operating systems use ACLs to manage access to files, directories, and network resources.

#### Application Allow/Deny Lists
Security policies can use allow and deny lists to control application execution.

- **Allow List**: Only applications that are explicitly approved can run. This method is very restrictive but offers high security.
- **Deny List**: Only applications on the "bad list" are blocked from execution, typically used by anti-virus and anti-malware software.

**Examples of Allow and Deny Lists**:
- **Application Hash**: Only applications with a specific, approved hash value can run.
- **Certificate**: Only applications signed with a valid certificate are allowed to execute.
- **Path**: Only applications located in designated folders can be executed.
- **Network Zone**: Applications can only run if they are located within a specific network zone.

### 2.5 Mitigation Techniques

Mitigation techniques refer to the strategies and processes used to reduce the impact of security events or potential security breaches.

#### Patching
Patching is crucial for maintaining system stability and applying security fixes to vulnerabilities.
- **Monthly Updates**: Regular, incremental updates that address known security issues.
- **Third-Party Updates**: Updates for third-party applications, device drivers, and software components.
- **Auto-Update**: While convenient, it is not always the best option due to potential compatibility issues or unexpected outcomes.
- **Emergency Out-of-Band Updates**: Critical security patches that are applied outside of the regular update schedule, often to address zero-day vulnerabilities or high-severity threats.

#### Encryption
Encryption ensures that unauthorized parties cannot access application data or files.
- **File-Level Encryption**: Encrypts specific files using technologies like EFS (Encrypted File System).
- **Full Disk Encryption (FDE)**: Encrypts the entire contents of a disk, such as using BitLocker (Windows) or FileVault (macOS).
- **Application Data Encryption**: Managed by the application itself, this protects stored data from unauthorized access.

#### Monitoring
Monitoring involves collecting data from various devices and systems to detect potential security events.
- **Built-In Technology**: Many devices come with built-in logging and monitoring capabilities.
- **Integrated Into Servers**: Servers often include sensors, IPS (Intrusion Prevention Systems), firewall logs, authentication logs, and more.
- **Collectors and Consoles**: Data aggregation tools such as SIEM (Security Information and Event Management) consoles, syslog servers, and proprietary tools help consolidate and analyze logs.
- **Correlation Engines**: Many SIEM systems include correlation engines that compare data from diverse sensors to identify unusual patterns.

#### Least Privilege
The principle of least privilege dictates that users should only have the minimum permissions necessary to perform their tasks.
- **Minimal User Rights**: User accounts should be restricted to only the permissions required for their role.
- **Application Privileges**: Applications should run with the least privileges, and administrative rights should be granted sparingly.
- **Limiting Malicious Behaviour**: Restricting administrative privileges limits the scope of any potential damage caused by malicious actions.

#### Configuration Enforcement
Ensures that devices meet security requirements before being allowed access to the network.
- **Posture Assessment**: Devices are assessed for compliance each time they connect to the network, checking factors like OS patch levels, EDR (Endpoint Detection and Response) versions, and firewall status.
- **Compliance Checks**: Systems that do not meet the required configuration are quarantined, often in a private VLAN with limited access.
- **Recheck After Corrections**: Devices that were initially out of compliance are rechecked after corrections have been made to ensure they meet the security standards.

#### Decommissioning
Proper decommissioning is critical to prevent data leakage or unauthorized access to sensitive information.
- **Data Removal**: Sensitive data should be completely removed from devices before decommissioning, especially from storage devices like HDDs, SSDs, and USB drives.
- **Device Reuse**: If devices are recycled for use in other systems, all data must be wiped or destroyed to ensure confidentiality.
- **Device Disposal**: Devices should be securely wiped and destroyed to prevent unauthorized recovery of any data.

### 2.5 Hardening Techniques

Hardening techniques involve strengthening systems to minimize vulnerabilities and reduce the likelihood of successful attacks.

#### System Hardening: Server
To secure a server, various hardening practices should be followed:
- **Updates**: Regularly apply operating system updates, service packs, and security patches to fix known vulnerabilities.
- **User Accounts**: Enforce policies for minimum password lengths and complexity, as well as restrictions on account usage and login attempts.
- **Network Access**: Limit network access to only necessary services, reducing the attack surface.
- **Monitoring and Security**: Deploy anti-virus, anti-malware tools, and continuously monitor system activity for potential threats.

#### Encryption
Encryption helps prevent unauthorized access to data and communication:
- **File System Encryption**: Encrypt sensitive files using built-in tools like EFS (Encrypting File System) on Windows.
- **Full Disk Encryption (FDE)**: Tools like BitLocker (Windows) and FileVault (macOS) encrypt entire disk drives, securing data even if the device is lost or stolen.
- **Network Communication Encryption**: Encrypt all network traffic with a VPN and encrypt application data to ensure confidentiality during transmission.

#### The Endpoint
The endpoint is the user’s access point to systems, applications, and data. Protecting endpoints is crucial for a layered security approach:
- **Defense in Depth**: Implement multiple layers of security, from hardware to software, to protect the endpoint from various threats.

#### Endpoint Detection and Response (EDR)
EDR provides advanced protection to endpoints by detecting, investigating, and responding to security incidents:
- **Threat Detection**: EDR systems use signatures, behavioral analysis, and machine learning to detect threats. They go beyond traditional signature-based detection.
- **Root Cause Analysis**: Investigate incidents to determine how an attack occurred and its impact.
- **Automated Response**: EDR systems can automatically isolate affected systems, quarantine threats, and roll back changes without user or technician intervention.

#### Host-Based Firewall
A host-based firewall runs on individual endpoints and controls application-level traffic:
- **Traffic Control**: It allows or denies incoming and outgoing traffic based on application processes.
- **Malware Prevention**: It can identify and block unknown processes, potentially stopping malware before it can execute.
- **Centralized Management**: These firewalls can be managed centrally to enforce consistent security policies across endpoints.

#### Host-Based Intrusion Prevention System (HIPS)
HIPS helps detect and block known attacks by securing the OS and application configurations:
- **Signature-Based Detection**: Uses predefined signatures to identify and block known threats.
- **Heuristic and Behavioral Analysis**: Identifies abnormal behavior and potential attacks based on patterns rather than known signatures.
- **Protection**: Can detect buffer overflows, unauthorized registry updates, and file modifications to sensitive areas of the OS.

#### Open Ports and Services
Every open port is a potential entry point for an attacker:
- **Limit Open Ports**: Only keep necessary ports open and control access to them using firewalls, including Next-Generation Firewalls (NGFWs).
- **Service Management**: Disable unused or unnecessary services, which may come pre-installed with the OS or third-party applications.
- **Port Scanning**: Use tools like Nmap to identify open ports and services, ensuring no unnecessary services are exposed.

#### Default Password Changes
Many devices come with default management interfaces and passwords:
- **Change Default Credentials**: Always change default passwords for network devices, critical systems, and applications.
- **Add Extra Security**: Implement additional authentication measures and strong passwords to increase security.

#### Removal of Unnecessary Software
Removing unneeded software reduces the attack surface:
- **Software Management**: Unused software can introduce security vulnerabilities through bugs and unpatched exploits.
- **Risk Reduction**: By removing unnecessary software, you reduce the number of vulnerabilities and simplify patch management.
</details>

<details>
<summary>3.0 Security Architecture</summary>
 
</details>

<details>
<summary>4.0 Security Operations</summary>
 
</details>

<details>
<summary>5.0 Security Program Management Oversight</summary>
 
</details>

