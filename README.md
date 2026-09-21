# NETWORKWALKS-GIDEON-B083-WK3-PM1-2-CYBERSECURITY-PASSWORD-CRACKING-WITH-JTR-AND-NW TOOLS
###
## 👤 Lab Information

| **Field** | **Details** |
|---|---|
| **Pentester Name**<br>*(Cybersecurity Professional)* | **OYEWALE OLAOLUWA GIDEON** |
| **Program/Batch** | B082-Networkwalks |
| **Date** | 21 SEPTEMBER 2026 |
| **Modules Completed** | W3-PM1 (Password Cracking With JTR)<br>W3-PM2 (Password Cracking With NW Online Tools) |
| **Client/Target** | 1. Networkwalks Locked PDF Files (secured written permission already)|
| **Permission secured from client?** | **Yes** |
| **Phases Covered** | **Phase 1:** Using Of John The Ripper to Crack The Password<br>**Phase 2:** Using Of NetworkWalks Tools to Crack The Password<br>|
###

##1. Introduction
This report documents to Week 3 cybersecurity activities completed as part of my ongoing internship at Networkwalks. The first module focuses on **Locked Networkwalks PDF File to be password crack by John The Ripper Tool  (W3-PM1)**, while the second covers **Locked Networkwalks PDF File to be password crack by Networkwalks online  Tools (W3-PM2)**.
Together, these exercises demonstrate the progression from **breaking the password of a passworded Networkwalks PDF files and accessing the information on it network**.
All activities were performed using **John The Ripper tools  to crack the password of the PDF file cracking password exercise** and a **Networkwalks Tools  to crack the password of the PDF file cracking password exercise**. Each section documents the command or procedure used, the observed output, supporting screenshot evidence, and a brief explanation of the security relevance of each finding.

##2🛠️ Tools Used

The table below lists the tools used in this report and their respective purposes.

| **Tool** | **Purpose** |
|---|---|
| **John The Ripper ** | password-cracking and password-auditing tool . It tests password hashes to determine whether passwords are weak or susceptible to guessing attacks.|
| **onlinehashcrack.** | PDF hash Extractor - IT will extract the information needed from your PDF to convert it to hash, also known as pdf2john or pdf2hashcat. |
| ** Networkwalks password cracker Online Tools** | password-cracking and password-auditing tool . It tests password hashes to determine whether passwords are weak or susceptible to guessing attacks.|
| ** Networkwalks Online Hash Calculaor Tools** | Generate MD5, SHA-1, SHA-256, SHA-384, SHA-512, or extract a crackable hash from a password-protected PDF.|



####
# 3. Activities Performed

## 3.1 Password Cracking Using JTK (John The Ripper ) tool

For the password-cracking phase of the assessment, John the Ripper (JTR) was downloaded, installed, and configured to perform a controlled password recovery test on the protected PDF file. The tool was used to assess the strength of the PDF password by systematically testing potential password combinations against the file’s password hash. This process demonstrated how password cracking tools can be used during authorized security assessments to identify weak or easily guessable passwords.
<img width="1237" height="571" alt="image" src="https://github.com/user-attachments/assets/9632387d-1b70-4211-830f-b5408b807862" />
<img width="672" height="358" alt="john the ripper app" src="https://github.com/user-attachments/assets/177101f4-e2a7-4d05-b556-3c0e40270037" />
<img width="912" height="510" alt="image" src="https://github.com/user-attachments/assets/72f5b5c5-f599-4aad-888b-fe1601c9c513" />

Before attempting to crack the password using John the Ripper (JTR), the password-protected PDF first had to be converted into a crackable hash format. An online tool, OnlineHashCrack, was used to extract the necessary password-hash information from the locked PDF. The PDF file was uploaded to the tool, which processed the file and generated the corresponding hash value required for the password cracking stage.
The extracted hash was then used as input for John the Ripper, allowing the tool to perform a controlled passwordrecovery test against the protected PDF.

<img width="859" height="610" alt="Screenshot 2026-09-20 202622" src="https://github.com/user-attachments/assets/aa80710b-24e1-4e13-80e1-53458a77c975" />
<img width="1235" height="693" alt="Screenshot 2026-09-20 202922" src="https://github.com/user-attachments/assets/5caaf8a7-8638-4b32-8bd2-7a3e83ccb9ba" />
<img width="1312" height="571" alt="Screenshot 2026-09-20 203058" src="https://github.com/user-attachments/assets/31d50d1c-377f-4d35-90aa-f75293f42e06" />

The Hash value was saved in a text file to upload to john the ripper so as to crack the password and after uploading the hash value it generated the password for the locked app and used to unlock the PDF file and likewise process was done to the other two fil
<img width="1364" height="610" alt="password " src="https://github.com/user-attachments/assets/b7714541-b243-470a-87d2-3d9563a64942" />
<img width="1306" height="574" alt="password2" src="https://github.com/user-attachments/assets/ac8d4f8b-1376-4d71-9c30-8722f7b38ce2" />
<img width="1247" height="698" alt="job done" src="https://github.com/user-attachments/assets/6049b980-4881-4cb6-b360-c998b1e246be" />
<img width="1095" height="563" alt="break" src="https://github.com/user-attachments/assets/2ee09e61-4d46-470f-a385-7048d0c55646" />
<img width="1068" height="643" alt="break3" src="https://github.com/user-attachments/assets/7d08c598-ce71-4d25-a1bb-97926c8e80ac" />

These findings provided additional visibility into the target's **web-server configuration, security controls, and DNS infrastructure**, contributing to the overall reconnaissance profile.

###
## 3.2 Network Scanning with Zenmap

The second practical activity focused on **network discovery and host identification using Zenmap** within my local network. The objective was to determine the local IP address and subnet, identify active devices, obtain their IP and MAC addresses, and visualize the discovered hosts using Zenmap's network topology feature.



I began by running the `ipconfig` command on Windows cmd to obtain the computer's local IP address and determine the applicable LAN subnet.

<img width="971" height="500" alt="image" src="https://github.com/user-attachments/assets/fd6aecb4-dd65-480b-975d-9e388532452e" />




 I then configured Zenmap with the identified subnet which is **192.168.56.1** and performed a **Ping Scan** to detect devices that were actively responding on the network. The command nmap -sn -PR 192.168.1.0/24

The practical exercise identified the following live hosts:

- `192.168.1.1`
- `192.168.1.193`
- `192.168.1.56`
-

The scan also returned corresponding **MAC address information** for the discovered devices.
<img width="1356" height="498" alt="image" src="https://github.com/user-attachments/assets/313a9b4c-f327-4eb7-8c41-9fac69d01213" />


After completing the host discovery scan, I accessed the **Topology** tab in Zenmap to visualize the network structure. I enabled the topology legend and exported the resulting network map as a **PDF**, as required by the practical exercise.
<img width="1353" height="588" alt="image" src="https://github.com/user-attachments/assets/d3f91b2d-f5ad-4260-b6fd-0473bec554d6" />


###



## 4. Risk Analysis / Impact

The reconnaissance and network-scanning exercises produced several findings that may have security implications. The observations below summarize the identified exposures and their potential impact.

| # | Risk / Finding | Evidence / Observation | Potential Impact | Risk Level |
|---|---|---|---|---|
| 1 | **Web technology details exposed** | WhatWeb detected **WordPress** and **WP Download Manager** on the website. | Technology and version details could help an attacker identify components that may require additional security assessment. | 🟠 **Medium** |
| 2 | **Web server IP address exposed** | Nslookup mapped the domain to **192.232.216.135**. | The information provides visibility into the network location associated with the web service. | 🟡 **Low** |
| 3 | **HTTP response information disclosed** | cURL returned HTTP headers and revealed the `/wp-json/` endpoint. | The exposed information may support application fingerprinting and additional reconnaissance. | 🟡 **Low** |
| 4 | **WAF technology detected** | Wafw00f identified **ModSecurity (SpiderLabs)** as the deployed WAF. | Identifying the security technology provides information about the web application's defensive infrastructure. | 🟡 **Low** |
| 5 | **DNS infrastructure exposed** | DNSRecon returned DNS, mail-server, and service-related records. | The information could be combined with other findings to develop a broader picture of the target infrastructure. | 🟠 **Medium** |
| 6 | **Multiple active hosts discovered** | Zenmap detected multiple responsive devices on the local network. | Unidentified or unauthorized devices could increase the potential attack surface of the local network. | 🟠 **Medium** |

### Risk Level Classification

- 🟡 **Low:** Limited exposure with relatively low immediate security impact.
- 🟠 **Medium:** Information that could contribute to further reconnaissance or increase exposure.
- 🔴 **High:** Findings that could present a significant security risk and require prompt attention.

###

## 5. Security Recommendations

- Keep WordPress, plugins, themes, and other web technologies regularly updated.
- Minimize unnecessary technical information exposed through HTTP headers and public endpoints.
- Review and secure DNS records and remove outdated or unnecessary entries.
- Maintain and regularly update WAF security rules and configurations.
- Monitor the local network for unknown or unauthorized devices.
- Conduct periodic vulnerability assessments and network security scans.
- Apply strong access controls to administrative and sensitive services.
- Enable security logging and monitor for suspicious network activity.
- Protect sensitive configuration and system information from public exposure.
- Document findings and verify that identified security issues are properly addressed.


## 6. Conclusion


This practical exercise provided valuable hands-on experience in the **reconnaissance, footprinting, network discovery, and initial security assessment phases of penetration testing**. The activities demonstrated how security professionals can systematically gather information about a target and use the collected data to develop an initial understanding of its digital infrastructure.

During the **footprinting and reconnaissance phase**, I used several Kali Linux tools, including **WHOIS, WhatWeb, Nslookup, cURL, Wafw00f, and DNSRecon**. Each tool provided a different perspective of the target environment. The assessment revealed information relating to domain registration, DNS infrastructure, the associated IP address, web technologies, HTTP response headers, publicly accessible endpoints, and the presence of a Web Application Firewall. Combining these results demonstrated how individual pieces of publicly available information can contribute to a broader understanding of a target's infrastructure.

The **network-scanning exercise** provided practical experience using **Zenmap** to identify active hosts within an authorized local network. By first determining the local IP address and subnet using Windows networking commands, I was able to configure Zenmap and perform host discovery. The scan demonstrated how network-scanning tools can identify responsive devices and provide information such as IP and MAC addresses. The Zenmap topology feature also provided a visual representation of the discovered network environment.

The exercises highlighted the importance of conducting reconnaissance and scanning in a **structured, controlled, and authorized manner**. Information gathered during these stages can help security professionals understand the attack surface, identify areas requiring further investigation, and prioritize appropriate security controls. At the same time, the findings demonstrate why organizations should minimize unnecessary information exposure and maintain visibility over devices and services operating within their networks.

From a learning perspective, this practical strengthened my ability to work with **Kali Linux, Windows networking tools, Zenmap, Nmap-based scanning, DNS enumeration, web technology fingerprinting, and basic security analysis**. It also improved my understanding of how reconnaissance findings can be documented, interpreted, and translated into potential security risks and recommendations.

Overall, the project provided a practical foundation for progressing into more advanced stages of security assessment, including **service enumeration, vulnerability identification, exploitation testing, and security validation**. All activities documented in this report were conducted within controlled environments and against systems for which appropriate authorization was available.


###
**👤 Author**

**Oyewale Olaoluwa Gideon**  
Cybersecurity Intern | B083
LinkedIn: www.linkedin.com/in/oyewale-olaouwa-60b252bb

---

**📌 Project Information**

**Program Name:** Cybersecurity Internship Program at Networkwalks | **Week:** 02 | **Project:** Footprinting & Network Scanning Phases  | **Repository:** GitHub

