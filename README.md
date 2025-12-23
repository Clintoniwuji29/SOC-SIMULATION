# SOC-SIMULATION
This alert was triggered when a user attempted to access an external URL that is listed in the organization's blacklist or threat intelligence feeds. The firewall or proxy successfully blocked the outbound request, preventing the connection. 

This alert was triggered when a user attempted to access an external URL that is listed in the organization's blacklist or threat intelligence feeds. The firewall or proxy successfully blocked the outbound request, preventing the connection. Note: The blacklist only covers known threats. It does not guarantee protection against new or unknown malicious domains.
<img width="3140" height="1427" alt="Screenshot 2025-12-23 011857" src="https://github.com/user-attachments/assets/32720b66-9a17-4365-8826-4f9fc1759151" />


Using TryHackMe SOC simulator to triage Suspicious Outbound Connection
The objective of this lab is to show use of a real SOC environment. Using the SOC dashboard, I will take ownership of alerts based on their severity, triage the alert, assign whether the alert is True positive or False positive, write a case report, and finally designate whether the alert needs escalation.
Skills Acquired

**Email Security**: Identify and respond to phishing attempts and malicious attachments.

**Incident Response**: Quickly address and escalate security incidents.

**Log Analysis**: Use Splunk to investigate and interpret security events.

**Threat Intelligence**: Correlate and validate threats using multiple intelligence sources.

**Network Analysis**: Monitor and examine network traffic with Wireshark.

**File Analysis**: Evaluate suspicious files using PowerShell and sandbox environments.

**Documentation**: Produce clear, concise incident reports.

**Problem-Solving**: Apply strong critical thinking and troubleshooting skills.

**Collaboration:** Work efficiently with SOC and security teams.

**Continuous Learning**: Keep current with evolving security threats and best practices.


**Tools Utilized
**
: Monitored and managed security alerts and incidents.

**Splunk Enterprise**: Performed log analysis and event searches.

**Virtual Machines for Sandboxing**: Safely analyzed suspicious files in isolated environments.

**VirusTotal**: Verified files and URLs against threat intelligence.

**Wireshark**: Analyzed network traffic for anomalies or malicious activity.

**PowerShell**: Conducted file analysis and automated repetitive security tasks.


**Steps**

Take ownership of an alert.
<img width="3095" height="1406" alt="Screenshot 2025-12-22 234953" src="https://github.com/user-attachments/assets/3e852abc-96d3-4e82-88f8-885bd4ce81c6" />

After taking ownership of the alert, I reviewed its description and proceeded with a detailed investigation using Splunk Enterprise.
<img width="3111" height="1441" alt="Screenshot 2025-12-23 000917" src="https://github.com/user-attachments/assets/7ee10554-8df9-484e-946a-a5f879857275" />

I continued triaging incoming alerts, several of which contained malicious URL/IP Address. These files were safely analyzed within a provided virtual machine sandbox. Using the PowerShell more command, I examined the contents of the attachments to gather additional details. Further research confirmed that wireshark can be used to capture remote access, enabling command-and-control activity, data exfiltration, persistence, and potential lateral movement within the environment.
<img width="3150" height="1440" alt="Screenshot 2025-12-23 014624" src="https://github.com/user-attachments/assets/09eeb03e-954d-4596-9911-c1b5d8a14128" />

**Documentation and result:**
Estsblished a True Positive. 
<img width="3125" height="1420" alt="Screenshot 2025-12-23 012814" src="https://github.com/user-attachments/assets/e82874e7-19ee-472c-8f33-58193299fed6" />

