# Yeshiva University CTF 2025  

- **Event Overview**:
  - **Date**: December 4–6, 2025  
  - **Duration**: 3 days of 24/7 challenges.  
  - **Format**: Individual challenges.  
  - **Categories**: Web Exploitation, Cryptography, Forensics, Reverse Engineering, Pwn, Wireshark, and more.  

- **Key Contributions**:
  - Solved 5 advanced Web Exploitation challenges with full points, including SQL Injection, XSS, and Command Injection.
  - Decrypted a complex **512-bit RSA ciphertext** in the Cryptography section using brute-force techniques.
  - Solved a high-value **Forensics** challenge, identifying a **Man-in-the-Middle (MITM)** attack from a packet capture using Wireshark.
  
#### **Categories Tackled**:
- **Web Exploitation**:
  - Full points on 5 advanced challenges, including **SQL Injection**, **Cross-Site Scripting (XSS)**, and **Command Injection**.
  - Exploited a complex **Blind SQL Injection** vulnerability on a login page, bypassing authentication and extracting user credentials from the database.
  - Found and exploited a **Stored XSS** vulnerability in an online forum, executing arbitrary JavaScript on the victim's browser to steal session cookies.
- **Forensics**:
  - Solved a high-value **Wireshark** challenge by analyzing packet captures (pcap files) to identify a **MITM (Man-in-the-Middle) attack**.
  - Recovered **steganographic files** hidden within image data and extracted encrypted information that led to the next challenge.
  - Decrypted network traffic using **SSL stripping** techniques to reveal sensitive credentials in plain text.
- **Cryptography**:
  - Decrypted a **512-bit RSA ciphertext** using **Brute-Force** and **Weak Key Attack** techniques, breaking the encryption within the time limit.
  - Exploited a **hash collision vulnerability** in SHA-1 to create a forged signature for a document, passing the integrity check.
  - Successfully cracked a **ROT13 + XOR** encrypted string in a challenge designed to simulate outdated cipher techniques.
  - Used **Elliptic Curve Cryptography (ECC)** to break an encrypted message and extract the original text.
- **Reverse Engineering**:
  - Disassembled a **buffer overflow challenge** using **Ghidra** and **IDA Pro**, then successfully injected shellcode to gain remote code execution.
  - Solved a **CRYPTO1** (low-level cryptography) puzzle, reverse-engineering a simple algorithm used to encrypt a file, and later exploited the weak implementation to retrieve the original key.
- **Pwn Challenges**:
  - Exploited a **Buffer Overflow** vulnerability in a **32-bit ELF executable** to execute arbitrary code, gaining control of the program's execution.
  - Leveraged **ROP chains** to bypass stack protection mechanisms such as **NX** and **ASLR**, gaining shell access on a remote system.
  - Completed a **format string vulnerability** challenge by manipulating printf-style functions to read memory contents, leading to shellcode execution.
  - Identified a **use-after-free** vulnerability in a given program, leading to arbitrary memory access and privilege escalation.
- **Wireshark**:
  - Analyzed a **pcap file** to identify a **DDoS attack** source, isolating malicious packets and tracing the attack to a compromised botnet.
  - Decoded encrypted **TLS/SSL traffic** from a pcap capture and extracted session keys to gain access to sensitive plaintext data.
  - Analyzed **DNS** and **HTTP** traffic in Wireshark to identify suspicious activity, pinpointing a **data exfiltration** operation through DNS tunneling.

#### **Challenges Solved**:
- **SQL Injection Attack**:
  - Bypassed login authentication using `' OR 1=1 --`, then extracted admin credentials and session tokens.
  - Leveraged **Time-based Blind SQL Injection** to retrieve sensitive database entries by measuring server response times.
  - Exploited **Union-based SQL Injection** to retrieve data from multiple tables, including user profiles and password hashes.
- **Cross-Site Scripting (XSS)**:
  - Exploited a **DOM-based XSS** vulnerability to steal and forward session cookies from logged-in users.
  - Executed a **Reflected XSS** attack, injecting malicious JavaScript to perform a **keylogger** attack, capturing typed credentials.
- **Buffer Overflow**:
  - Reverse-engineered a vulnerable application to locate a buffer overflow vulnerability, then successfully executed shellcode to gain control of the system.
  - Used **Return-Oriented Programming (ROP)** to bypass stack protections and execute arbitrary commands.
- **Packet Analysis**:
  - Identified the **source IP of a DDoS attack** by analyzing pcap files in Wireshark, isolating the attack from legitimate traffic.
  - Used **TCP sequence analysis** to determine the location of a man-in-the-middle (MITM) attack that intercepted and altered communications between clients.
  - Dissected **encrypted traffic** and extracted login credentials passed through a vulnerable website, thanks to weak SSL/TLS implementation.
- **Steganography**:
  - Identified and extracted hidden data from a **JPEG image** using **steganographic** tools like **StegSolve**, then decoded the data to reveal a flag hidden in an image's least significant bits (LSB).
  - Used a **PDF steganography** technique to extract a hidden flag embedded within a suspicious PDF file.
- **Reverse Engineering and Binary Exploitation**:
  - Successfully reverse-engineered a **patched binary** to retrieve an earlier version of the application’s source code and exploit vulnerabilities in its older codebase.

---

## 📚 Skills Demonstrated
- **Web Exploitation**: SQL Injection, XSS, Command Injection.
- **Cryptography**: RSA, ECC, SHA-1 collisions, ROT13 + XOR.
- **Forensics**: Packet Analysis, SSL Stripping, Steganography.
- **Reverse Engineering**: Buffer Overflow, ROP, Binary Exploitation.
- **Steganography**: Image Steganography, PDF Analysis, LSB extraction.
- **Pwn**: Buffer Overflow, ROP Chains, Format String Vulnerability, Use-After-Free, Privilege Escalation.
- **Wireshark**: Packet Capture Analysis, DDoS Source Identification, SSL Decryption, DNS Tunneling.

---

## 📖 Lessons Learned
- Collaboration in high-pressure environments.
- Efficient time management for prioritizing challenges.
- Deepened understanding of common vulnerabilities and exploitation techniques.
