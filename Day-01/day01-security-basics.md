1. What is Cybersecurity?

Cybersecurity is the practice of protecting systems, networks, applications, devices, and data from unauthorized access, misuse, disruption, modification, or destruction.

2. CIA Triad

The three fundamental goals of security:

Principle	Meaning	Example
Confidentiality	Only authorized people can access data	Passwords, encryption
Integrity	Data isn't improperly modified	Hashes, digital signatures
Availability	Systems/data remain accessible	Backups, redundancy, DDoS protection

Easy memory:

C = Can I see it?
I = Is it correct?
A = Is it available?

3. Threat vs Vulnerability vs Risk

Threat → Something that could cause harm.

Example: An attacker.

Vulnerability → A weakness that can be exploited.

Example: SQL injection vulnerability.

Risk → The potential impact of a threat exploiting a vulnerability.

Threat
   ↓
Vulnerability
   ↓
Exploitation
   ↓
Impact
   ↓
Risk
4. Authentication vs Authorization

Authentication = Who are you?

Examples:

Password
OTP
Fingerprint
MFA

Authorization = What are you allowed to do?

Example:

User → View own profile
Admin → View/delete users

Remember:

AuthN = Identity
AuthZ = Permissions

5. Hashing vs Encryption

Hashing

One-way transformation:

Password
   ↓
Hash

Used for things such as password verification and integrity checking.

Encryption

Reversible with the appropriate key:

Plaintext
   ↓
Encryption + Key
   ↓
Ciphertext
   ↓
Decryption + Key
   ↓
Plaintext

Never confuse the two.

6. Common Attacks

Know what these mean:

Phishing
Tricking users into revealing information or performing an unsafe action.

Malware
Malicious software.

Examples:

Virus
Worm
Trojan
Ransomware
Spyware

Brute force
Trying many possible credentials until one works.

DDoS
Overwhelming a service with traffic/requests so legitimate users cannot access it.

SQL Injection
Manipulating an application's database query through unsafe input.

XSS
Injecting malicious client-side script into a web application.

You'll study SQLi and XSS much more deeply later.

7. Security Controls

Security controls are measures used to reduce security risk.

Examples:

MFA
Firewalls
Encryption
Backups
Access control
Antivirus/EDR
Logging
Security monitoring
Patching
Input validation

They can be:

Preventive — stop an attack
Detective — identify an attack
Corrective — recover/respond after an incident
🔥 Most important takeaway for you

Since you're coming from MERN development, start thinking like a security engineer:

Instead of only asking:

"How do I build this API?"

also ask:

"How could someone abuse this API, and how do I prevent it?"

For example:

POST /api/login

A developer thinks:

Does login work?

A security-minded developer asks:

Can I brute-force it?
Can I bypass authentication?
Are passwords securely hashed?
Can I manipulate the request?
Is rate limiting implemented?
Can I enumerate users?
Are errors leaking information?
Are tokens handled securely?

That's the mindset we want to build over these 30 days.

Day 1 checkpoint

You should now be able to explain these without notes:

CIA → Threat → Vulnerability → Risk → Authentication → Authorization → Hashing → Encryption → Malware → Phishing → DDoS