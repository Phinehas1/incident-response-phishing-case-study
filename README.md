# Incident Response Case Study: Phishing Email with Malware Attachment (Simulated)

**Disclaimer:**  
This incident response case study is a simulated scenario created for educational and portfolio purposes.

---

## Incident Overview
A medium-severity phishing alert was generated after an employee received an email containing a suspicious attachment posing as a job application. The attachment was identified as a malicious executable file.

---

<details>
<summary>Screenshot of Phishing Email</summary>

![Phishing Email Example](screenshots/Phishing-email-example.png)

</details>

---
## SOC Ticket Details
- **Ticket ID:** A-2703  
- **Alert:** SERVER-MAIL Phishing attempt – possible malware delivery  
- **Severity:** Medium  
- **Status:** Escalated  

---

<details>
<summary><strong>Detection</strong></summary>

- SOC received an alert indicating a potential phishing attempt on the corporate email server  
- Email contained an executable attachment disguised as a resume  
- Alert escalated due to potential malware delivery  

</details>

---

<details>
<summary><strong>Analysis and Indicators of Compromise (IoCs)</strong></summary>

- Sender domain did not match a legitimate corporate or recruitment domain  
- Email originated from an external IP address  
- Attachment identified as an executable file (`bfsvc.exe`) masquerading as a resume  
- Password-protected attachment used to evade automated email scanning  
- Known malicious file hash identified:


</details>

---

<details>
<summary><strong>Impact Assessment</strong></summary>

- No evidence the attachment was executed  
- No endpoint compromise detected  
- Incident classified as medium severity based on potential malware exposure  

</details>

---

<details>
<summary><strong>Response and Mitigation</strong></summary>

- Blocked sender IP address and domain  
- Quarantined the email and malicious attachment  
- Added malicious file hash to security blocklists  
- Notified HR department of phishing attempt  

</details>

---

<details>
<summary><strong>Prevention Recommendations</strong></summary>

- Block executable attachments at the email gateway  
- Implement sandboxing for email attachments  
- Provide phishing awareness training to HR staff  
- Enforce least-privilege access controls  

</details>

---

<details>
<summary><strong>Incident Summary</strong></summary>

- Investigated a phishing email delivering a malicious executable attachment  
- Identified indicators of compromise including sender IP and file hash  
- Incident successfully contained with no confirmed system compromise  

</details>
