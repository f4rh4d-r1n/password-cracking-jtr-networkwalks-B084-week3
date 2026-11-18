# 🔐 Password Cracking Labs — John the Ripper & Hash Analysis Tools

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Ethical%20Hacking-red?style=for-the-badge&logo=hackaday&logoColor=white)
![John the Ripper](https://img.shields.io/badge/Tool-John%20the%20Ripper-black?style=for-the-badge&logo=linux&logoColor=white)
![Johnny GUI](https://img.shields.io/badge/Tool-Johnny%20GUI-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Kali%20Linux-informational?style=for-the-badge&logo=kalilinux&logoColor=white)

## 📖 Overview

This repository documents two hands-on password cracking labs completed as part of a Cybersecurity & Ethical Hacking training program. The labs explore how password-protected PDF files can be analyzed and cracked using hash extraction and dictionary attacks — a core technique in offensive security and penetration testing.

> ⚠️ **Educational purpose only.** All work was performed on sample files provided by the course for learning purposes. These techniques should only ever be used on systems and files you own or have explicit written authorization to test.

## 🧪 Labs Included

| Module | Topic | Tools Used |
|---|---|---|
| **Module 1** | Password Cracking with JTR | John the Ripper, Johnny (GUI), Online Hash Extractor |
| **Module 2** | Password Cracking with NW Tools | Hash Calculator, Password Cracker (dictionary attack) |

### Module 1 — John the Ripper (JTR) & Johnny
- Extracted a crackable hash (`$pdf$...`) from a password-protected PDF using `pdf2john`
- Loaded the hash into **Johnny**, the GUI front-end for John the Ripper
- Ran a dictionary/brute-force attack to recover the original password
- Verified the recovered password by unlocking the PDF

### Module 2 — Networkwalks Hash Calculator & Password Cracker
- Used the **Hash Calculator** tool to extract a hashcat/pdf2john-compatible hash directly in-browser
- Fed the hash into the **Password Cracker** tool for a dictionary attack
- Recovered the password and unlocked the file

## 🧠 Key Concepts Learned

- **Encryption vs. Hashing** — encryption is reversible with the correct key; hashing is a one-way function used to verify, not reveal, data
- How password hashes are extracted from protected file formats (PDF, ZIP, Office)
- How dictionary attacks work: testing wordlist candidates against a hash until a match is found
- Why password length and complexity directly affect crack time
- The real-world risk of weak/reused passwords (breach statistics referenced in the course material)

## 📂 Repository Structure

```
password-cracking-labs/
├── docs/
│   ├── Module1_Password_Cracking_with_JTR.pdf
│   └── Module2_Password_Cracking_with_NW_Tools.pdf
├── screenshots/
│   ├── 01_johnny_cracked_hash.png
│   ├── 02_hash_calculator_output.png
│   ├── 03_onlinehashcrack_extractor.png
│   └── 04_pdf_password_prompt.png
├── LICENSE
└── README.md
```

## 🛠️ Tools Referenced

- [John the Ripper](https://www.openwall.com/john/) — password cracking tool
- [Johnny](https://openwall.info/wiki/john/johnny) — GUI for John the Ripper
- [Online Hash Crack — PDF Hash Extractor](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php)
- Networkwalks Hash Calculator & Password Cracker (training tools)

## 📌 Note on Flags/Answers

Lab completion flags and the specific cracked password used in these training exercises have intentionally **not** been published in this README out of respect for other students still working through the same coursework. Screenshots and documentation here focus on methodology, not answers.

## 📜 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details. Course material PDFs remain the property of Networkwalks and are included here for personal learning-record purposes only.

---

*Part of a Cybersecurity & Ethical Hacking training journey — Week 3 Project Modules.*
