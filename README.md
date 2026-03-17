# Data Security in IT Systems - Lab Portfolio 🔒

This repository documents my technical journey through the MSc Cybersecurity program. Each project is contained within a collapsible section—click **"View Project Details"** to see the full technical walkthrough.

---

## 🧪 Lab 01: Social Engineering Attack Lifecycle
*Focus: Malware Development, Phishing, and Remote Access*

<details>
<summary><b>📂 View Project Details & Screenshots</b></summary>

### **Technical Walkthrough**

**1. Weaponization & Payload Prep** I edited the `main.cpp` source file in a Kali Linux environment and used `msfvenom` to generate a reverse TCP shellcode. This shellcode was embedded directly into the C++ character buffer.
![Payload Prep](./images/lab1_1.png)

**2. Delivery & Phishing Execution** After compiling the code into `update.exe`, I hosted it on a Python HTTP server. I crafted a targeted phishing email and a fake Roundcube webmail login page to trick the user into downloading and running the file.
![Phishing Setup](./images/lab1_7.png)

**3. Exploitation & Remote Shell** With the Metasploit `multi/handler` active, the moment the user executed the file on the Windows target, a reverse connection was established. I successfully gained full command-line access to the target system.
![Remote Access](./images/lab1_9.png)

**Key Takeaway:** This lab demonstrates how attackers combine technical tools with psychological deception to bypass traditional security perimeters.

</details>

---

## 🧪 Lab 02: Linux Hardening & SSH Brute-Force Mitigation
*Focus: Intrusion Prevention, SSHGuard, and System Monitoring*

<details>
<summary><b>📂 View Project Details & Screenshots</b></summary>

### **Technical Walkthrough**

**1. Securing the SSH Service** I deployed **SSHGuard** on an Ubuntu Server to monitor authentication logs. This service is designed to automatically detect and block IP addresses that exhibit suspicious brute-force behavior.
![Service Status](./images/lab2_1.png)

**2. Attack Simulation** Using a Python script in Kali Linux, I generated repeated, rapid-fire network requests to simulate an automated brute-force attack against the server's SSH port.
![Attack Script](./images/lab2_2.png)

**3. Automated Mitigation** The system detected the abnormal traffic patterns in real-time. **SSHGuard** triggered `iptables` rules to drop all traffic from the attacker's IP, effectively neutralizing the threat while maintaining system stability.
![Mitigation Active](./images/lab2_3.png)

**Key Takeaway:** Proactive host-based intrusion prevention (HIPS) is critical for protecting exposed services from automated credential-stuffing attacks.

</details>

---

## 🧪 Lab 03: [Upcoming Lab]
*Future documentation for Cloud Security or IoT Labs.*
