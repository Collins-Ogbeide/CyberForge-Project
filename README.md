# CyberForge-Project
Linux Security Hardening &amp; Audit Report
<img width="960" height="505" alt="image" src="https://github.com/user-attachments/assets/52993004-7bfa-42d6-9bfe-70d49bef39b2" />


<img width="960" height="505" alt="image" src="https://github.com/user-attachments/assets/105fbdde-a713-4b48-9eb3-5744f13ffc48" />
Analyst: Collins Ogbeide  
Date: October 18, 2026  
System: Ubuntu 26.04.1 LTS (VMware Workstation)

 Project Overview
This repository documents my 5-day intensive Linux security hardening and auditing project. It covers file permissions, service management, firewall inspection, log analysis, and forensic verification of security controls.

 Evidence & Screenshots
This repository contains the terminal output and verification screenshots for:
- Day 2: File Permission Auditing (chmod 600)
- Day 3: Service & SSH Status Checks
- Day 4: Firewall (ufw) & Log Analysis (journalctl, auth.log)
- Day 5: Advanced Hardening (chmod 400) & Forensic Verification (stat)

 Key Commands Used
| Command | Purpose |
| :--- | :--- |
| chmod 400 [file] | Restricts file to Read-Only for owner (Maximum security) |
| sudo ufw status verbose | Checks the state of the Uncomplicated Firewall |
| sudo journalctl -p warning -n 20 | Filters system logs for critical warnings |
| sudo tail -n 30 /var/log/auth.log | Reviews authentication logs for intrusions |
| stat -c '%A %a %n' [file] | Forensically verifies exact file permissions |

 Lessons Learned
- *Adaptability is key:* When tools fail, knowing native alternatives saves the day.
- *Audit before you act:* Always check the baseline state of a system before applying changes.
- *Documentation is proof:* A security action is only as good as the verification that it worked.

 ⚠️ Security Note
All screenshots have been reviewed. No real passwords, private keys, or sensitive personal information (PII) are present in this repository. Mock data was used for testing.

