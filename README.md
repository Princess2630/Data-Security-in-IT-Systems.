# Data Security in IT Systems - Labs Portfolio 

This repository documents my technical journey through the MSc Cybersecurity program.

---

## Lab 01: Social Engineering Attack Lifecycle & Remote Access
*Tools: Kali Linux, MSFVenom, Metasploit (msfconsole), G++, Python HTTP Server*

<details>
<summary><b>📂 View Full Project Walkthrough (Manual Payload Prep to Exploitation)</b></summary>

### **Phase 1: Weaponization**
| Step 1: Nano Source Editing | Step 2: MSFVenom Generation | Step 3: Shellcode Embedding |
| :---: | :---: | :---: |
| <img src="./images/lab1_1.png" width="250"> | <img src="./images/lab1_2.png" width="250"> | <img src="./images/lab1_3.png" width="250"> |
| *Defining the C++ buffer* | *Generating Reverse TCP payload* | *Pasting hex into main.cpp* |

### **Phase 2: Delivery & Phishing**
| Step 4: G++ Compilation | Step 5: Python HTTP Server | Step 6: Roundcube Webmail Setup |
| :---: | :---: | :---: |
| <img src="./images/lab1_4.png" width="250"> | <img src="./images/lab1_4.png" width="250"> | <img src="./images/lab1_5.png" width="250"> |
| *Creating update.exe* | *Hosting the delivery vector* | *Fake login portal creation* |

### **Phase 3: Exploitation**
| Step 7: Metasploit Handler | Step 8: Target Execution | Step 9: Reverse Shell Success |
| :---: | :---: | :---: |
| <img src="./images/lab1_7.png" width="250"> | <img src="./images/lab1_10.png" width="250"> | <img src="./images/lab1_8.png" width="250"> |
| *Configuring LHOST/LPORT* | *User runs update.exe on Win* | *Full CLI access granted* |

**Conclusion:** This lab demonstrated the end-to-end attack chain, proving that user interaction is a critical vulnerability that can be exploited to bypass technical perimeters.

</details>

---

##  Lab 02: Host-Based Intrusion Prevention (SSHGuard)
*Tools: Ubuntu Server, SSHGuard, Iptables, Python Attack Scripts*

<details>
<summary><b>📂 View Full Project Walkthrough (Automated Brute-Force Mitigation)</b></summary>

### **Phase 1: Defensive Hardening**
| Step 1: Service Verification | Step 2: Systemctl Monitoring |
| :---: | :---: |
| <img src="./images/lab2_1.png" width="400"> | <img src="./images/lab2_1.png" width="400"> |
| *Verifying SSHGuard is active* | *Checking iptables integration* |

### **Phase 2: Attack Simulation**
| Step 3: Python Brute-Force | Step 4: Auth.log Detection |
| :---: | :---: |
| <img src="./images/lab2_2.png" width="400"> | <img src="./images/lab2_3.png" width="400"> |
| *Simulating rapid SSH attempts* | *SSHGuard identifying the pattern* |

### **Phase 3: Mitigation & Resource Analysis**
| Step 5: Iptables Drop Rules | Step 6: System Stability (Htop) | Step 7: Log Correlation |
| :---: | :---: | :---: |
| <img src="./images/lab2_10.png" width="250"> | <img src="./images/lab2_13.png" width="250"> | <img src="./images/lab2_12.png" width="250"> |
| *Malicious IP blocked in firewall* | *Analyzing CPU/RAM under load* | *Matching logs with mitigations* |

**Conclusion:** The lab confirmed that combining real-time log analysis with automated firewall updates successfully neutralizes high-frequency brute-force attacks without impacting system performance.

</details>

---

<p align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png" width="100%">
</p>

<p align="center">
  <b>  Stay tuned! More labs on Data Security are on the way.</b><br>
  <i>Current Status: MSc Cybersecurity Student | Actively Building & Documenting</i>
</p>

<p align="center">
  <a href="https://github.com/Princess2630">
    <img src="https://img.shields.io/badge/Follow-Princess2630-blue?style=for-the-badge&logo=github" alt="Follow on GitHub">
  </a>
</p>
