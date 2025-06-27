# 🔥 Cyber Security Internship – Task 4

## ✅ Task Title:
**Setup and Use a Firewall on Windows**

---

## 🎯 Objective:
To configure and test basic firewall rules using Windows Defender Firewall by blocking Telnet traffic on port 23, validating the rule, and restoring the firewall to its original state.

---

## 🛠 Tools & Technologies Used:
- **Operating System:** Windows 10/11
- **Firewall Tool:** Windows Defender Firewall with Advanced Security
- **Command Line Tool:** Command Prompt
- **Telnet Client:** Installed via Windows Features

---

## 📌 Steps Performed:

1. **Opened Firewall Settings**  
   - Launched "Windows Defender Firewall with Advanced Security".

2. **Created Inbound Rule to Block Port 23 (Telnet)**  
   - Selected "Port" > TCP > Port 23  
   - Chose "Block the connection"  
   - Applied to all profiles (Domain, Private, Public)  
   - Named the rule: `Block Telnet Port 23`  
   📸 Screenshot: `1_rule_created.png`

3. **Installed Telnet Client**  
   - Enabled Telnet Client from "Turn Windows features on or off"  
   📸 Screenshot: `2_telnet_installed.png` (optional)

4. **Tested the Rule**  
   - Ran `telnet localhost 23` in Command Prompt  
   - Confirmed connection was blocked  
   📸 Screenshot: `3_telnet_test_blocked.png`

5. **Deleted the Custom Rule**  
   - Removed `Block Telnet Port 23` rule  
   📸 Screenshot: `4_rule_deleted.png`

---

## 📉 Limitations:
- Telnet test may silently fail if no Telnet service is running, which can be misinterpreted as a firewall block.
- Requires admin privileges to modify firewall settings.
- GUI-based rules are less scriptable than Linux/UFW alternatives.

---

## 📚 Concepts Learned:

- What a firewall is and how it filters traffic.
- Difference between **inbound** and **outbound** firewall rules.
- How to **block a specific port** using Windows Firewall.
- How to install and use the **Telnet Client** to test open/blocked ports.
- Importance of **removing temporary security rules** to avoid misconfigurations.

---

## ✅ Conclusion:

Successfully configured Windows Defender Firewall to block Telnet traffic on port 23. Verified that the rule was effective by using the Telnet client, and then removed the rule to restore the default configuration. This task demonstrated hands-on knowledge of basic firewall management and network security principles.

---

