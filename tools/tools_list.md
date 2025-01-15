# 🛠️ CTF Tools List

This document provides a curated list of tools that were instrumental in solving CTF challenges during the Yeshiva University CTF event and other related CTFs. These tools range from packet analyzers to exploit frameworks, providing an essential toolkit for cybersecurity professionals.

---

## 1. **Wireshark**  
   - **Category**: Network Analysis, Forensics  
   - **Description**: A powerful network protocol analyzer used for capturing and analyzing packets in real time. Ideal for tasks like packet sniffing, network traffic analysis, and identifying vulnerabilities in network traffic.  
   - **Key Features**:
     - Real-time traffic capture
     - Protocol decoding
     - Deep packet inspection  
   - **Usage**: Used extensively in CTF challenges to identify DDoS attacks, MITM attacks, and analyze network traffic.
   - **Link**: [Wireshark Official Site](https://www.wireshark.org/)

---

## 2. **Burp Suite**  
   - **Category**: Web Exploitation, Security Testing  
   - **Description**: A comprehensive suite for web application security testing. It helps identify vulnerabilities in web applications, such as SQL Injection, XSS, and more.  
   - **Key Features**:
     - Intercepting Proxy
     - Web Scanning and Crawling
     - Intruder (for automated attacks)  
   - **Usage**: Used for exploiting web vulnerabilities, crawling web applications, and testing security flaws in web-based services.
   - **Link**: [Burp Suite Official Site](https://portswigger.net/burp)

---

## 3. **Ghidra**  
   - **Category**: Reverse Engineering, Binary Exploitation  
   - **Description**: A software reverse engineering framework developed by the NSA. It is used to analyze binaries and reverse-engineer compiled applications.  
   - **Key Features**:
     - Static analysis of binaries
     - Disassembly and decompilation
     - Supports multiple architectures  
   - **Usage**: Used to reverse-engineer binaries in CTF challenges, find vulnerabilities like buffer overflows, and understand application logic.
   - **Link**: [Ghidra Official Site](https://ghidra-sre.org/)

---

## 4. **Metasploit Framework**  
   - **Category**: Exploitation, Penetration Testing  
   - **Description**: An open-source framework for developing and executing exploit code against remote targets. It's used for penetration testing, exploiting vulnerabilities, and learning security exploits.  
   - **Key Features**:
     - Exploit development
     - Payload creation
     - Post-exploitation capabilities  
   - **Usage**: Used in CTF to automate exploit development, generate payloads, and test system defenses.
   - **Link**: [Metasploit Official Site](https://www.metasploit.com/)

---

## 5. **John the Ripper**  
   - **Category**: Cryptography, Password Cracking  
   - **Description**: A powerful password cracking tool that is primarily used to test the strength of passwords by attempting to decrypt them through dictionary and brute force attacks.  
   - **Key Features**:
     - Cracks various cryptographic hashes
     - Supports many password hash algorithms  
   - **Usage**: Used in CTF challenges to crack password hashes or decrypt encrypted passwords.
   - **Link**: [John the Ripper Official Site](https://www.openwall.com/john/)

---

## 6. **Hydra**  
   - **Category**: Password Cracking, Brute Forcing  
   - **Description**: A fast and flexible password-cracking tool that supports multiple protocols, including HTTP, FTP, and SSH. It is often used to perform brute-force attacks.  
   - **Key Features**:
     - Supports numerous protocols
     - Parallelized attack methods  
   - **Usage**: Used to crack login forms and perform brute-force attacks on network services in CTF challenges.
   - **Link**: [Hydra GitHub Repo](https://github.com/vanhauser-thc/thc-hydra)

---

## 7. **Netcat (nc)**  
   - **Category**: Networking, Pwn  
   - **Description**: Known as the "Swiss Army knife" of networking, Netcat is a versatile tool for reading from and writing to network connections. It is used for creating backdoors, port scanning, and even file transfers.  
   - **Key Features**:
     - Simple and lightweight
     - Can be used to create a remote shell
     - Supports both TCP and UDP  
   - **Usage**: Used in CTF for creating reverse shells, port scanning, and establishing connections between attack and target machines.
   - **Link**: [Netcat GitHub Repo](https://github.com/diegocr/netcat)

---

## 8. **Radare2**  
   - **Category**: Reverse Engineering  
   - **Description**: An open-source framework for reverse engineering and analyzing binaries. It provides a wide range of tools for disassembling, debugging, and exploiting vulnerabilities in executables.  
   - **Key Features**:
     - Disassembler and debugger
     - Support for various file formats
     - Scripting capabilities  
   - **Usage**: Used to dissect binaries and identify vulnerabilities in compiled applications during CTF reverse engineering challenges.
   - **Link**: [Radare2 Official Site](https://rada.re/n/)

---

## 9. **Steghide**  
   - **Category**: Steganography  
   - **Description**: A command-line tool used for hiding data in various kinds of files, such as BMP, WAV, and JPEG. Steghide can extract hidden information from such files.  
   - **Key Features**:
     - Supports multiple file formats
     - Password protection for hidden files  
   - **Usage**: Used in CTF for uncovering hidden messages or flags in image and audio files through steganography.
   - **Link**: [Steghide GitHub Repo](https://github.com/StefanoDeVuono/steghide)

---

## 10. **Nikto**  
   - **Category**: Web Application Security  
   - **Description**: A web server scanner used to identify vulnerabilities, such as outdated server software, insecure files, and configuration issues.  
   - **Key Features**:
     - Comprehensive vulnerability scanning
     - Detects potential server misconfigurations
     - Reports detailed findings  
   - **Usage**: Used in CTF to scan and identify vulnerable web servers that can be exploited through various attack vectors.
   - **Link**: [Nikto GitHub Repo](https://github.com/sullo/nikto)

---

## 11. **Sleuth Kit**  
   - **Category**: Digital Forensics  
   - **Description**: A collection of command-line tools used for digital forensics, allowing the analysis of disk images and recovering deleted files.  
   - **Key Features**:
     - Disk image analysis
     - File recovery
     - Metadata extraction  
   - **Usage**: Used in CTF for performing disk forensics to retrieve deleted files and analyze file systems.
   - **Link**: [Sleuth Kit Official Site](http://sleuthkit.org/)

---

Feel free to contribute any tools you find useful for CTF challenges and cybersecurity in general. I welcome your suggestions and additions to enhance this list!