# Week 03 – Password Cracking & Security Auditing

## Overview

Week 03 of my Networkwalks Cybersecurity Internship focused on understanding password security, password hashing, and password-cracking techniques.

This week's practical exercises introduced password auditing using John the Ripper and Networkwalks online security tools.

All practical activities were performed in a controlled learning environment using Kali Linux.

## Objectives

- Understand password hashing and password security.
- Learn how password-protected PDF files store password hashes.
- Extract password hashes from encrypted PDF files.
- Perform password auditing using John the Ripper.
- Explore Networkwalks Hash Calculator and Password Cracker.
- Understand the importance of strong and complex passwords.

## Tasks Completed

### 1. Password Cracking with John the Ripper (JTR)

**Objective:** Recover the password of a provided password-protected PDF file using John the Ripper.

**Tools Used:**
- Kali Linux
- John the Ripper
- PDF Hash Extractor
- RockYou Wordlist
- Terminal

**Practical Workflow:**

1. Obtained the password-protected PDF provided for the lab.
2. Extracted the PDF password hash using an online PDF hash extractor.
3. Saved the extracted hash in a text file named `hash1.txt`.
4. Prepared the RockYou wordlist.
5. Used John the Ripper to perform a dictionary-based password audit.
6. Checked the results using John's show command.
7. Verified the recovered password by opening the protected PDF.

**Commands Used:**

```bash
john --version
```

```bash
cd ~/Downloads
```

```bash
nano hash1.txt
```

```bash
john --wordlist=/usr/share/wordlists/rockyou.txt hash1.txt
```

```bash
john --show hash1.txt
```

### 2. Password Cracking with Networkwalks Tools

**Objective:** Extract and recover the password of the provided protected PDF using Networkwalks online tools.

**Tools Used:**
- Kali Linux
- Firefox Browser
- Networkwalks Hash Calculator
- Networkwalks Password Cracker

**Practical Workflow:**

1. Downloaded the provided password-protected PDF.
2. Opened the Networkwalks Hash Calculator.
3. Uploaded the protected PDF to extract its password hash.
4. Copied the complete extracted hash.
5. Opened the Networkwalks Password Cracker.
6. Submitted the extracted hash for password recovery.
7. Obtained the recovered password from the tool.
8. Verified the password by opening the original PDF.

**Online Tools:**

- [Networkwalks Hash Calculator](https://networkwalks.com/hash-calculator/)
- [Networkwalks Password Cracker](https://networkwalks.com/password-cracker/)

## Key Learnings

- Difference between encryption and hashing.
- How password-protected PDF files can be audited.
- How John the Ripper performs dictionary-based password attacks.
- How wordlists are used in password auditing.
- How to extract and process password hashes.
- Why strong, unique passwords are important for cybersecurity.

## Evidence & Screenshots

Practical screenshots are organized into their respective module folders:

- PM1 – John the Ripper
- PM2 – Networkwalks Tools

## Security & Ethical Considerations

All activities were performed for educational purposes using the files and tools specified in the internship lab instructions.

Password auditing should only be performed on files and systems for which permission has been granted.

Sensitive information, recovered passwords, and confidential files are not included in this public repository.

## Conclusion

Week 03 provided practical exposure to password auditing techniques using John the Ripper and Networkwalks security tools.

These exercises improved my understanding of password hashes, dictionary-based attacks, and the importance of implementing strong password security practices.

---

**Internship:** Networkwalks Cybersecurity Internship  
**Week:** 03  
**Focus Area:** Password Cracking & Security Auditing  
**Environment:** Kali Linux
