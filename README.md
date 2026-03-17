# Data Security in IT Systems - Lab Portfolio 

This repository documents my technical journey through the MSc Cybersecurity program. Each project is contained within a collapsible section—click **"View Project Details"** to see the full technical walkthrough.
----

##  Lab 01: Social Engineering Attack Lifecycle
*Focus: Malware Development, Phishing, and Remote Access*

<details>
<summary><b>📂 View Full Technical Walkthrough (9+ Screenshots)</b></summary>

### **Phase 1: Weaponization & Coding**
**1. Source Code Prep:** Editing `main.cpp` in Kali Linux to prepare the malicious character buffer.
![Step 1](./images/lab1_1.png)

**2. Shellcode Generation:** Using `msfvenom` to generate the reverse TCP payload.
![Step 2](./images/lab1_2.png)

**3. Embedding:** Pasting the hex shellcode into the C++ source before compilation.
![Step 3](./images/lab1_3.png)

### **Phase 2: Delivery & Social Engineering**
**4. Compilation & Hosting:** Compiling the exploit into `update.exe` and launching a Python HTTP server to host the file.
![Step 4](./images/lab1_4.png)

**5. Fake Login Portal:** Setting up the Roundcube webmail clone to capture user interest.
![Step 5](./images/lab1_5.png)

**6. The Phishing Email:** Crafting the deceptive message to trigger the download.
![Step 6](./images/lab1_9.png)

### **Phase 3: Exploitation & Control**
**7. Listener Configuration:** Setting up the Metasploit `multi/handler` to wait for the callback.
![Step 7](./images/lab1_7.png)

**8. Target Execution:** The moment the user runs the "update" on the Windows machine.
![Step 8](./images/lab1_10.png)

**9. Remote Access Granted:** Success! Full command-line access established via the reverse shell.
![Step 9](./images/lab1_8.png)

</details>

---

##  Lab 02: Host-Based Intrusion Prevention (SSHGuard)
*Focus: Brute-Force Mitigation and Linux Hardening*

<details>
<summary><b>📂 View Full Technical Walkthrough (12+ Screenshots)</b></summary>

### **Phase 1: Defensive Setup**
**1. Service Verification:** Confirming **SSHGuard** is active and integrated with `iptables` on the Ubuntu Server.
![Step 1](./images/lab2_1.png)

### **Phase 2: Attack Simulation**
**2. Automated Brute-Force:** Running a Python script from Kali Linux to hammer the SSH port with connection attempts.
![Step 2](./images/lab2_2.png)

**3. Real-Time Detection:** Monitoring the server logs as SSHGuard identifies the rapid-fire authentication failures.
![Step 3](./images/lab2_3.png)

### **Phase 3: Mitigation & Monitoring**
**4. Blocking the Attacker:** Viewing the `iptables` rules automatically generated to drop the attacker's IP.
![Step 4](./images/lab2_10.png)

**5. System Stability:** Monitoring CPU and resource usage to ensure the server remains stable under attack.
![Step 5](./images/lab2_11.png)

**6. Correlation:** Analyzing the logs to correlate the attack timestamps with the defensive actions taken.
![Step 6](./images/lab2_12.png)

</details>
*Future documentation for Cloud Security or IoT Labs.*
