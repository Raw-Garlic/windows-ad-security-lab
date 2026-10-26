Windows Active Directory + PowerShell Security Lab

A hands-on Windows Server 2022 Active Directory environment built in Azure, then secured, monitored, and audited the way a SOC or GRC team would in a real enterprise domain. Every lab uses PowerShell, and every control is mapped to CIS and NIST 800-53.

Status: In progress (started October 2026). Each lab's folder is added as it's completed, with its README, scripts, and evidence.

Labs
#	Lab	Focus	Status
1	Domain Build	Windows Server 2022 DC + member server in Azure, static IP/DNS, RDP restricted by NSG	In progress
2	Identity & Least Privilege	OU design, CSV-driven user provisioning, role-based groups, tiered admin accounts, delegated help desk rights	Planned
3	Group Policy Hardening	Password/lockout policy, fine-grained admin policy, LLMNR disabled, script block logging, advanced audit policy	Planned
4	Windows Event Detection	Simulated password spray, lockout, and privilege escalation; hunting with PowerShell and Microsoft Sentinel KQL; MITRE ATT&CK mapping	Planned
5	PowerShell AD Audit Tool	Script that flags stale accounts, weak password settings, Kerberoastable SPNs, and privileged access outside the tiering model	Planned
Environment
Platform: Microsoft Azure (westus2)
Domain: lab.local
Servers: dc01 (domain controller + DNS), srv01 (member server)
Tools: Azure CLI, PowerShell, ActiveDirectory and GroupPolicy modules, Group Policy Management Console, Microsoft Sentinel
Skills Demonstrated
Active Directory deployment and administration
Identity and access management: least privilege, admin tiering, delegation
Secure configuration through Group Policy
Windows security event analysis and detection engineering
PowerShell scripting and automation
Control mapping to CIS Benchmarks, CIS Controls v8, NIST 800-53, and MITRE ATT&CK
Security Practices
No credentials are stored in this repository. All scripts prompt for passwords at runtime with Read-Host -AsSecureString.
Remote access to lab servers is restricted to a single trusted source IP. IP addresses are redacted from screenshots.
Attack simulations run only against this isolated lab domain.
Cloud resources are deallocated between sessions and deleted when the project is complete.
Related Projects
cysa-lab-portfolio: 12-lab CySA+ capstone ("Operation BlueShield")
azure-security-mini-lab: Azure network security, monitoring, and Sentinel detection
Author

Alejandro W. Orellana: CompTIA Security+, Network+, CySA+ · Google Cybersecurity Certificate
