# Password Cracking and Hashing Algorithms

### Project Overview

This project was developed to demonstrate a practical understanding of cryptographic hashing and its vulnerabilities. The goal is to show how a simple dictionary attack can be used to "crack" passwords that have been secured with an outdated and insecure hashing algorithm.

**Disclaimer:** This project is for educational and ethical purposes only. The techniques and code provided should only be used in a legal and authorized environment.

### Project Files

-   `password_cracker.py`: The main Python script that performs the dictionary attack. It reads a list of target hashes and a wordlist, then attempts to match them.
-   `hashed_passwords.txt`: A file containing MD5 hashes of known, simple passwords. This represents a "leaked" password file.
-   `wordlist.txt`: A simple dictionary of common passwords used to attempt to crack the hashes.

### Methodology

The `password_cracker.py` script follows a simple logic:
1.  It reads the hashes from `hashed_passwords.txt`.
2.  It iterates through each word in the `wordlist.txt`.
3.  For each word, it generates an MD5 hash.
4.  It compares the generated hash to the target hashes.
5.  If a match is found, it reports the plaintext password and the corresponding hash.

This method, known as a **dictionary attack**, highlights why using simple, common passwords and weak hashing algorithms (like MD5) is a major security risk.

### How to Run the Project

#### Prerequisites
-   Python 3 (The `hashlib` library is built-in).

#### Steps
1.  Place all three project files (`password_cracker.py`, `hashed_passwords.txt`, `wordlist.txt`) in the same directory.
2.  Open a terminal or command prompt and navigate to the project directory.
3.  Execute the Python script with the following command:
    ```sh
    python password_cracker.py
    ```
4.  The script will print the results to the console, showing which hashes were successfully cracked.

### Skills Demonstrated

-   **Cryptography Fundamentals:** Understanding hashing, salting, and the difference between secure and insecure algorithms.
-   **Ethical Hacking:** Understanding attack methodologies like dictionary attacks.
-   **Python Programming:** File I/O, string manipulation, and using the `hashlib` library.
-   **Security Best Practices:** The importance of using strong, salted hashes for password storage.

---
*Project completed by Aditya Sudhakar Mundhe  as part of my internship.*