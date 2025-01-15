# CTF Writeups

This section contains detailed writeups of the challenges solved during the Yeshiva University CTF event and other CTFs. Each writeup provides step-by-step solutions, explanations of the methods used, and insights into the tools and techniques employed to solve each challenge. These writeups are designed to help others learn and apply similar tactics in future CTFs.

---

## 1. **SQL Injection Challenge**  
   - **Category**: Web Exploitation  
   - **Difficulty**: Medium  
   - **Challenge Description**:  
     We were given a vulnerable login page and tasked with bypassing authentication using SQL Injection.
     
   - **Steps to Solve**:  
     1. **Identify the Vulnerability**:  
        - Observed the login page’s request URL and input fields. Tested with a simple SQL Injection payload: `' OR 1=1 --`.
     2. **Bypass Authentication**:  
        - The payload `' OR 1=1 --` bypassed the login page’s authentication check, logging us into the application.
     3. **Capture the Flag**:  
        - Once logged in, we accessed the flag hidden in the user’s profile page.
     
   - **Tools Used**:  
     - Burp Suite: Intercepted HTTP requests and modified inputs to test SQL Injection.
     - Firefox Developer Tools: Inspected the login form’s HTTP requests and responses.

---

## 2. **Wireshark Packet Analysis Challenge**  
   - **Category**: Forensics  
   - **Difficulty**: High  
   - **Challenge Description**:  
     We were provided with a pcap file containing network traffic and asked to identify the source of a DDoS attack.
     
   - **Steps to Solve**:  
     1. **Open the pcap File**:  
        - Opened the provided pcap file in Wireshark for inspection.
     2. **Filter Traffic**:  
        - Applied filters to focus on suspicious traffic, including `ip.src` and `ip.dst`.
     3. **Identify DDoS Traffic**:  
        - Noticed multiple SYN packets from a single IP address targeting a specific server, indicating a SYN Flood attack.
     4. **Block the Attacker**:  
        - Once identified, we noted the attacker’s IP and recommended that the server’s firewall block the source IP.
     
   - **Tools Used**:  
     - Wireshark: For packet capture and analysis.
     - tcpdump: Used for advanced traffic analysis.

---

## 3. **RSA Encryption Challenge**  
   - **Category**: Cryptography  
   - **Difficulty**: High  
   - **Challenge Description**:  
     We were given a 512-bit RSA ciphertext and tasked with decrypting it.
     
   - **Steps to Solve**:  
     1. **Inspect the Ciphertext**:  
        - The given ciphertext was in hexadecimal format.
     2. **Factor the Modulus**:  
        - Used the `RSA` modulus and public exponent to factor the large number. We used online tools such as `factordb.com` for factoring.
     3. **Decrypt the Ciphertext**:  
        - Once we factored the modulus, we used the private key to decrypt the ciphertext and reveal the plaintext.
     
   - **Tools Used**:  
     - Python (RSA module): For decryption and key generation.
     - OpenSSL: For verifying the private key and decryption process.

---

## 4. **Buffer Overflow Challenge**  
   - **Category**: Pwn  
   - **Difficulty**: Very High  
   - **Challenge Description**:  
     The challenge was a vulnerable C program susceptible to a buffer overflow. Our goal was to overflow the buffer and execute code to gain control of the system.
     
   - **Steps to Solve**:  
     1. **Analyze the Source Code**:  
        - The program accepted user input without bounds checking, making it vulnerable to buffer overflow.
     2. **Find the Offset**:  
        - Used pattern generation to identify the exact byte offset at which the return address was overwritten.
     3. **Exploit the Vulnerability**:  
        - Crafted an input payload with shellcode to overwrite the return address and gain access to a shell.
     4. **Gain Shell Access**:  
        - Used `nc` (Netcat) to create a reverse shell and interact with the system.
     
   - **Tools Used**:  
     - GDB: For debugging and finding the buffer overflow.
     - Python: For crafting the payload.
     - Netcat: For establishing a reverse shell.

---

## 5. **Steganography Challenge**  
   - **Category**: Steganography  
   - **Difficulty**: Medium  
   - **Challenge Description**:  
     We were given an image file and tasked with extracting a hidden message (flag) embedded in the image.
     
   - **Steps to Solve**:  
     1. **Analyze the Image**:  
        - Used `Steghide` to check if the image contained hidden data.
     2. **Extract the Data**:  
        - Found the hidden flag by extracting it using the correct password.
     3. **Capture the Flag**:  
        - The hidden message revealed the flag.
     
   - **Tools Used**:  
     - Steghide: For extracting hidden data from the image.
     - Binwalk: For inspecting hidden files within the image.

---

Feel free to check out the other writeups as we continue to add new solutions from future CTF events. Contribute your writeups or suggestions to improve this collection!