# Data Security in IT Systems - Lab Portfolio 🔒

This repository documents my technical journey through the MSc Cybersecurity program. Each project is contained within a collapsible section—click **"View Project Details"** to see the full technical walkthrough and screenshots.

---

## 🧪 Lab 01: Social Engineering Attack Lifecycle
*Focus: Malware Development, Phishing, and Remote Access*

<details>
<summary><b>📂 Click to View Project Details & Screenshots</b></summary>

### **Technical Walkthrough**

**1. [cite_start]Weaponization & Payload Prep** Edited the `main.cpp` source file [cite: 1, 3] [cite_start]and generated a reverse TCP shellcode using `msfvenom`[cite: 5, 6]. [cite_start]This demonstrated how attackers embed malicious code into legitimate-looking programs[cite: 4].
![Payload Prep](./images/lab1_1.png)

**2. [cite_start]Delivery Mechanism** Compiled the payload into `update.exe` [cite: 14] [cite_start]and hosted it via a Python HTTP server[cite: 15]. [cite_start]I then crafted a phishing email and a fake Roundcube login page [cite: 22, 26] [cite_start]to trick the target into downloading the "update"[cite: 27].
![Phishing Email](./images/lab1_7.png)

**3. [cite_start]Exploitation & Remote Shell** Once the user executed the file on the Windows target [cite: 37, 38][cite_start], my Metasploit listener received a reverse connection [cite: 31][cite_start], granting full CLI access to the system[cite: 32].
![Reverse Shell Success](./images/lab1_9.png)

> [cite_start]**Key Learning:** This lab emphasizes that social engineering exploits human trust rather than just technical flaws[cite: 42].

</details>

---

## 🧪 Lab 02: Data Integrity & Digital Signatures
*Focus: Hashing Algorithms (MD5/SHA-256) and RSA Signing*

<details>
<summary><b>📂 Click to View Project Details & Screenshots</b></summary>

### **Technical Walkthrough**

**1. Hashing for Integrity** Generated MD5 and SHA-256 hashes of a source file to establish a digital fingerprint.
![Hash Generation](./images/lab2_1.png)

**2. Detecting Unauthorized Changes** Modified the file content and re-verified the hash. The mismatched results proved that the file's integrity had been compromised.
![Hash Mismatch](./images/lab2_2.png)

**3. Digital Signatures** Utilized a Private Key to sign the file hash and a Public Key to verify it, ensuring authenticity and non-repudiation.
![Verification Success](./images/lab2_3.png)

</details>

---

## 🧪 Lab 03: [Upcoming Lab]
*Future documentation for Cloud Security or IoT Labs.*
