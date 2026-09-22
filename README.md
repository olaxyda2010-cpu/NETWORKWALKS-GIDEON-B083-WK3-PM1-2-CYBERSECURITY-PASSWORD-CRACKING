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
|**John The Ripper**| password-cracking and password-auditing tool . It tests password hashes to determine whether passwords are weak or susceptible to guessing attacks.|
|**onlinehashcrack.**| PDF hash Extractor - IT will extract the information needed from your PDF to convert it to hash, also known as pdf2john or pdf2hashcat. |
|**Networkwalks password cracker Online Tools**| password-cracking and password-auditing tool . It tests password hashes to determine whether passwords are weak or susceptible to guessing attacks.|
|**Networkwalks Online Hash Calculaor Tools**| Generate MD5, SHA-1, SHA-256, SHA-384, SHA-512, or extract a crackable hash from a password-protected PDF.|



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


The extracted hash value was saved in a text file and subsequently provided as input to John the Ripper (JTR) for password-cracking analysis. JTR systematically tested potential password combinations against the extracted hash until the correct password was identified.

Once the password was successfully recovered, it was used to unlock and access the protected PDF file. The same procedure was then repeated for the remaining two password-protected PDF files, including extracting their hash values, processing them with John the Ripper, recovering the corresponding passwords, and using the recovered credentials to unlock the files.



<img width="1364" height="610" alt="password " src="https://github.com/user-attachments/assets/b7714541-b243-470a-87d2-3d9563a64942" />
<img width="1306" height="574" alt="password2" src="https://github.com/user-attachments/assets/ac8d4f8b-1376-4d71-9c30-8722f7b38ce2" />
<img width="1247" height="698" alt="job done" src="https://github.com/user-attachments/assets/6049b980-4881-4cb6-b360-c998b1e246be" />
<img width="1095" height="563" alt="break" src="https://github.com/user-attachments/assets/2ee09e61-4d46-470f-a385-7048d0c55646" />
<img width="1068" height="643" alt="break3" src="https://github.com/user-attachments/assets/7d08c598-ce71-4d25-a1bb-97926c8e80ac" />


This exercise demonstrated the practical application of password-cracking techniques in an authorized security-testing environment and highlighted the importance of using strong, complex passwords to protect sensitive documents.

###
## 3.2 Password Cracking Using Networkwalks online  tool

The second practical activity focused on using NetworkWalks online tools to achieve the same password-recovery objective demonstrated with John the Ripper (JTR).

As part of the exercise, the NetworkWalks Hash Calculator was used to process the password-protected PDF and extract the hash information required for password-cracking analysis. Similar to the previous practical, where OnlineHashCrack was used to obtain the hash for JTR, the NetworkWalks tool provided the hash value needed for the subsequent password-recovery process.

This practical provided an opportunity to compare an online-based approach with the password cracking approach using John the Ripper, demonstrating how different tools can be used to perform similar password security assessments.
<img width="911" height="477" alt="image" src="https://github.com/user-attachments/assets/8af95d9e-e299-4c52-beea-b3d91509efae" />
<img width="1078" height="661" alt="image" src="https://github.com/user-attachments/assets/01bb794f-b868-4f07-8341-f62a498d715f" />


After the hash value was created from the uploaded PDF file Networkwalks Password Cracker was used to crack the hash value to generate the real password and used to unlock the PDF file
<img width="1124" height="546" alt="image" src="https://github.com/user-attachments/assets/4b1ab4ac-eac6-4461-8e27-0ffde23972ff" />
<img width="989" height="621" alt="image" src="https://github.com/user-attachments/assets/d8e5ab4f-8d8f-4d30-95be-338a0d4bac20" />
<img width="1247" height="698" alt="job done" src="https://github.com/user-attachments/assets/60f9ff76-89a5-40b8-a9a0-c6797a846486" />








###





## 6. Conclusion

### Conclusion

The practical activities provided valuable hands-on experience in **password security assessment and password recovery techniques** using both GUI and online tools. **John the Ripper (JTR)** was used to analyze extracted PDF password hashes and recover the passwords through systematic password-cracking techniques. The same objective was subsequently achieved using **NetworkWalks online tools**, providing a practical comparison between different approaches to password recovery.

The exercise demonstrated the importance of understanding how password-protected files can be assessed when the necessary authorization and hash information are available. It also highlighted the security risks associated with **weak or easily guessable passwords**, as such passwords can potentially be recovered using automated cracking techniques.

Overall, the practical strengthened my understanding of **password hashing, hash extraction, passwordcracking methodologies, and security assessment tools**. It also reinforced the importance of implementing strong, unique passwords and appropriate security controls when protecting sensitive information.

###

## 🔭 Tools and Resources ##

To install JTR CLI AND GUI : [https://7-zip.org/download.html.](https://drive.usercontent.google.com/download?id=1YeyV7pwN6gRyKGUKqwyhGv0DKf_vFf8j&export=download&authuser=0&confirm=t&uuid=4c9b5f3b-3360-4039-bc23-2ccec70591a9&at=AMrWOn2lg6GmeJ2__xZ1Hm6WEUdN:1790056324880)

[https://7-zip.org/download.html.](https://drive.usercontent.google.com/download?id=1ecZTIyGrmAIy07phmZO_rm9Ps1y0aHUs&export=download&authuser=0&confirm=t&uuid=4c4320bf-4bdf-4198-97e1-7a3f782b424f&at=AMrWOn0WmMAw0jGgqkQ5w-AJ3G7f:1790069703772)

The Locked PDF files and the Networkwalks online tools:
https://networkwalks.com/wp-content/uploads/2026/08/Password-Cracking-with-NW-Tools-v1.pdf
https://networkwalks.com/wp-content/uploads/2026/08/My-Locked-PDF1.pdf
https://networkwalks.com/wp-content/uploads/2026/08/My-Locked-PDF2.pdf
https://networkwalks.com/wp-content/uploads/2026/08/My-Locked-PDF3.pdf


---
**👤 Author**

**Oyewale Olaoluwa Gideon**  
Cybersecurity Intern | B083
LinkedIn: www.linkedin.com/in/oyewale-olaouwa-60b252bb

---

**📌 Project Information**

**Program Name:** Cybersecurity Internship Program at Networkwalks | **Week:** 03 | **Project:** PASSWORD CRACKING WITH JTR AND NW TOOLS  | **Repository:** GitHub

