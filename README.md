<div align="center">🔐 PENETRATION TESTING REPORT

FOOTPRINTING & NETWORK SCANNING PHASES

W2-PM-FINAL | CYBERSECURITY | NETWORKWALKS

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1000&color=00F7FF&center=true&vCenter=true&width=650&lines=Cybersecurity+%26+Ethical+Hacking;Reconnaissance+%7C+Footprinting;Network+Discovery+%7C+Scanning;Learning+by+Doing+%F0%9F%94%90" />"Cybersecurity" (https://img.shields.io/badge/Domain-Cybersecurity-blue?style=for-the-badge)
"Kali Linux" (https://img.shields.io/badge/OS-Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
"Nmap" (https://img.shields.io/badge/Tool-Nmap%2FZenmap-4682B4?style=for-the-badge)
"Status" (https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

Author: ODESANMI OLUMIDE

Cybersecurity Professional | Networkwalks | Batch B084

</div>---

📌 1. PROJECT OVERVIEW

This repository documents my Week 2 practical activities during the Cybersecurity & Ethical Hacking internship program at Networkwalks.

The project focuses on two fundamental penetration testing activities:

1. Footprinting & Reconnaissance: Gathering publicly available information about a target domain using multiple Kali Linux tools.
2. Network Scanning & Discovery: Identifying active hosts and network information within my authorized local network using Zenmap.

These exercises demonstrate how cybersecurity professionals gather intelligence, identify exposed information, map network environments, and document potential security risks.

Project Information| Details
Pentester| Odesanmi Olumide
Program| Networkwalks Cybersecurity Program
Batch| B084
Project Code| W2-PM-FINAL
Date| 14 November 2026
Module 1| W2-PM1 – Multiple Kali Tools
Module 2| W2-PM5 – Zenmap Scanning
Target 1| networkwalks.com
Target 2| My Own Local LAN
Authorization| Written permission secured for assigned target
Phases Covered| Reconnaissance, Footprinting & Scanning
Project Status| Phases 1–2 completed; Phases 3–5 in progress

---

⚖️ 2. AUTHORIZATION & LIABILITY DISCLAIMER

All activities documented in this repository were conducted within an authorized educational environment or on systems and devices owned by me.

Written permission was secured for the assigned target.

This repository is intended strictly for educational, research, and professional development purposes.

The tools and techniques documented here must not be used against systems, networks, or devices without appropriate authorization.

Unauthorized access to computer systems may constitute a criminal offense and can result in legal consequences, financial penalties, and other liabilities.

The author, instructors, and Networkwalks are not responsible for any misuse of the information contained in this repository.

Ethical hacking requires authorization, accountability, and responsible disclosure.

---

🎯 3. PROJECT OBJECTIVES

The primary objectives of this practical exercise were to:

- Understand the fundamentals of reconnaissance and footprinting.
- Identify publicly available domain registration information.
- Discover website technologies and server information.
- Examine DNS records and infrastructure information.
- Identify potential security information exposed through HTTP headers.
- Determine whether a Web Application Firewall (WAF) is present.
- Identify active devices within an authorized local network.
- Discover IP and MAC addresses.
- Generate and document a network topology.
- Develop professional cybersecurity reporting skills.

---

🛠️ 4. TOOLS & TECHNOLOGIES USED

The following tools were used throughout the practical exercises.

Tool| Purpose| Environment
Kali Linux| Reconnaissance and security testing| Linux
WHOIS| Domain registration information| Kali Linux
WhatWeb| Website technology fingerprinting| Kali Linux
Nslookup| DNS resolution| Kali Linux
cURL| HTTP response header inspection| Kali Linux
Wafw00f| Web Application Firewall detection| Kali Linux
DNSRecon| DNS record enumeration| Kali Linux
Zenmap| Network discovery and scanning| Windows
Nmap| Network scanning engine| Windows
Windows CMD| Local IP and MAC identification| Windows

---

🔍 5. METHODOLOGY & ACTIVITIES PERFORMED

PHASE 1: RECONNAISSANCE & FOOTPRINTING

Target: "networkwalks.com"

Operating System: Kali Linux

I performed reconnaissance against the assigned domain using six Kali Linux tools.

Each tool provided a different perspective of the target's publicly accessible infrastructure.

5.1 WHOIS – Domain Information Gathering

Objective: Obtain publicly available domain registration information.

WHOIS was used to gather information relating to:

- Domain registration.
- Registration dates.
- Name servers.
- Domain ownership information where publicly available.

Security relevance:

Domain registration information can help security professionals understand the infrastructure associated with a target and identify publicly exposed administrative information.

5.2 WhatWeb – Technology Fingerprinting

Objective: Identify technologies used by the target website.

The results identified:

- WordPress 7.0.4.
- WP Download Manager 3.3.58.
- Additional publicly identifiable web technologies.

Security relevance:

Technology fingerprinting helps identify software components that may require further security review against relevant vulnerability advisories.

5.3 Nslookup – DNS Resolution

Objective: Resolve the domain name to its corresponding IP address.

Observed result:

"192.232.216.135"

Security relevance:

DNS resolution helps establish the network address associated with a domain and provides useful information for infrastructure mapping.

5.4 cURL – HTTP Header Analysis

Objective: Inspect the HTTP response headers returned by the website.

The "curl -I" command was used to retrieve HTTP response headers.

Observation:

The response exposed technical information about the web application, including the WordPress REST API endpoint:

"/wp-json/"

Security relevance:

HTTP response headers can reveal information about web server configurations and application technologies.

5.5 Wafw00f – Web Application Firewall Detection

Objective: Identify whether a Web Application Firewall protects the website.

Observed result:

ModSecurity (SpiderLabs).

Security relevance:

Identifying a WAF provides insight into the defensive technologies protecting a web application.

5.6 DNSRecon – DNS Enumeration

Objective: Enumerate publicly accessible DNS records.

The exercise identified information relating to:

- NS records.
- MX records.
- SPF records.
- TXT records.
- SRV records.
- DNS infrastructure information.

Security relevance:

DNS enumeration helps security professionals understand an organization's publicly exposed domain infrastructure and identify records requiring configuration review.

---

PHASE 2: NETWORK SCANNING & DISCOVERY

Tool: Zenmap (Nmap GUI)

Operating System: Windows

Target: My own local LAN network.

The second practical activity focused on identifying active hosts within my local network.

5.7 Local Network Identification

I initially used the Windows Command Prompt to identify my local IP address and subnet.

Command used:

ipconfig

This provided information about my local network configuration.

5.8 Host Discovery with Zenmap

I launched Zenmap and entered the identified local subnet.

I selected the Ping Scan option to discover active hosts within the authorized network.

Observed example result:

Parameter| Observation
Live Host| 10.52.39.3
IP Address| 10.52.39.3
MAC Address| Recorded during the practical
Scanning Tool| Zenmap
Scan Type| Ping Scan

Note: The above address represents the example result provided in the practical. Replace it with your verified local scan results before final submission.

5.9 Network Topology Generation

After completing the network scan, I:

1. Opened the Topology section in Zenmap.
2. Enabled the topology legend.
3. Reviewed the discovered network devices.
4. Generated the network topology.
5. Saved the topology in PDF format.

Security relevance:

Network topology visualization helps administrators understand network structure, identify connected devices, and investigate unexpected hosts.

---

📊 6. RISK ANALYSIS & SECURITY IMPACT

Based on the observations collected during the footprinting and scanning activities, I identified the following potential security risks.

#| Finding| Evidence| Potential Impact| Risk
1| Web technology information exposed| WhatWeb identified WordPress and WP Download Manager| May assist attackers in identifying software requiring security review| Medium
2| Server IP identifiable| Nslookup resolved the domain to 192.232.216.135| Provides information about the web infrastructure| Low
3| HTTP technical information exposed| cURL identified response headers and "/wp-json/"| May assist further technology fingerprinting| Low
4| WAF technology identifiable| Wafw00f identified ModSecurity| Reveals information about defensive architecture| Low
5| DNS infrastructure information exposed| DNSRecon identified DNS and mail records| Helps build an infrastructure profile| Medium
6| Multiple live hosts visible| Zenmap identified active hosts in the example network| Unknown devices may require investigation| Medium

Risk Classification

- 🔴 Critical
- 🟠 High
- 🟡 Medium
- 🟢 Low

Important Security Note:

The findings documented above represent observations from reconnaissance and network discovery exercises. They are not confirmed vulnerabilities.

No exploitation or vulnerability validation was performed during these two modules.

The presence of an identifiable software version, IP address, DNS record, or WAF does not automatically indicate that a system is vulnerable.

Additional authorized security testing would be required to validate any suspected vulnerability.

---

🛡️ 7. SECURITY RECOMMENDATIONS

Based on the observations, I recommend the following security improvements:

#| Recommendation| Security Benefit
1| Review publicly exposed technology information| Reduces unnecessary technology disclosure
2| Keep CMS platforms and plugins updated| Reduces exposure to known vulnerabilities
3| Review HTTP security headers| Helps identify unnecessary technical disclosures and missing security controls
4| Regularly audit DNS records| Ensures only necessary DNS information is publicly exposed
5| Properly configure and monitor ModSecurity| Strengthens web application protection
6| Perform regular internal network discovery| Improves visibility of connected devices
7| Investigate unknown network devices| Helps detect unauthorized connections
8| Maintain updated network documentation| Improves infrastructure visibility and incident response
9| Conduct authorized security assessments| Helps identify and validate security weaknesses

---

📸 8. EVIDENCE & SCREENSHOTS

This section contains evidence collected during the practical activities.

Screenshots should be uploaded into an "evidence/" folder in this repository.

Phase 1: Footprinting & Reconnaissance

#| Evidence| Description
1| WHOIS Screenshot| Domain registration information
2| WhatWeb Screenshot| Website technology fingerprinting
3| Nslookup Screenshot| Domain-to-IP resolution
4| cURL Screenshot| HTTP response headers
5| Wafw00f Screenshot| WAF detection
6| DNSRecon Screenshot| DNS enumeration results

Phase 2: Network Scanning

#| Evidence| Description
1| Windows CMD Screenshot| Local IP and network configuration
2| Zenmap Scan Screenshot| Active host discovery
3| Host Information| IP and MAC address identification
4| Network Topology| Visual representation of discovered hosts
5| Topology PDF| Exported network topology report

Adding Screenshots to GitHub

Create a folder named:

evidence/

Upload your screenshots into that folder.

To display a screenshot in your README, use:

![WHOIS Results](evidence/whois.png)

For multiple screenshots:

## WHOIS Results
![WHOIS](<div align="center">🔐 PENETRATION TESTING REPORT

FOOTPRINTING & NETWORK SCANNING PHASES

W2-PM-FINAL | CYBERSECURITY | NETWORKWALKS

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1000&color=00F7FF&center=true&vCenter=true&width=650&lines=Cybersecurity+%26+Ethical+Hacking;Reconnaissance+%7C+Footprinting;Network+Discovery+%7C+Scanning;Learning+by+Doing+%F0%9F%94%90" />"Cybersecurity" (https://img.shields.io/badge/Domain-Cybersecurity-blue?style=for-the-badge)
"Kali Linux" (https://img.shields.io/badge/OS-Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
"Nmap" (https://img.shields.io/badge/Tool-Nmap%2FZenmap-4682B4?style=for-the-badge)
"Status" (https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

Author: ODESANMI OLUMIDE

Cybersecurity Professional | Networkwalks | Batch B084



