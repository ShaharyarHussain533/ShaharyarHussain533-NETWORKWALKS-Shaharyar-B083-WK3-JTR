# 🔐 Password Cracking — John the Ripper & Networkwalks Tools

## 👤 Student Information

**Name:** Syed Shaharyar Hussain
**Batch:** B083

## 📌 Overview

This repository documents **Week 3 of my Cybersecurity & Ethical Hacking training**, focusing on password-cracking techniques using:

* **John the Ripper (JTR)**
* **Johnny — JTR Graphical Interface**
* **Networkwalks Hash Calculator**
* **Networkwalks Password Cracker**

The labs demonstrate how password-protected PDF files can be analyzed by extracting their password hash and attempting to recover the original password.

The exercises were performed in an **authorized cybersecurity learning environment** for educational and security-awareness purposes.

---

## 🎯 Learning Objectives

Through these labs, I practiced:

* Understanding password hashing and password protection
* Extracting hashes from password-protected PDF files
* Preparing extracted hashes for password-cracking tools
* Using John the Ripper from a Windows environment
* Using the Johnny graphical interface
* Using browser-based Networkwalks security tools
* Understanding how password complexity affects cracking time
* Demonstrating the importance of strong passwords

---

# 🧪 Project Module 1 — Password Cracking with JTR

## 🔎 Introduction

**John the Ripper (JTR)** is a password-cracking tool used by security professionals to test password strength. It supports multiple operating systems and password/hash formats, including password-protected files such as PDFs, ZIP archives, and Office documents.

The lab also introduces **Johnny**, the graphical interface for John the Ripper, which provides a simpler point-and-click workflow.

### Tools Used

* John the Ripper
* Johnny GUI
* PDF Hash Extractor
* Notepad
* Windows PC / Kali Linux

---

## ⚙️ JTR Workflow

### 1. Install John the Ripper

John the Ripper can be downloaded from the official Openwall website:

https://www.openwall.com/john/

### 2. Configure Johnny

After installing Johnny:

1. Open Johnny.
2. Open **Settings**.
3. Browse to the `john.exe` executable.
4. Select the `john.exe` file from the JTR `run` directory.

### 3. Extract the PDF Hash

The encrypted PDF is uploaded to a PDF hash extraction tool.

The extracted hash begins with:

```text
$pdf$...
```

### 4. Create the Hash File

The extracted hash is placed into:

```text
hash1.txt
```

### 5. Start the Attack

In Johnny:

1. Select **Open password file**.
2. Open `hash1.txt`.
3. Select **Start new attack**.
4. Wait for the password-cracking process to complete.

The required time depends on computer performance and password complexity.

### 6. Verify the Password

Once the password has been recovered, it can be used to open the encrypted PDF.

For the provided lab exercise:

```text
password1
```

---

# 🧪 Project Module 2 — Password Cracking with Networkwalks Tools

## 🔎 Introduction

The second lab demonstrates a browser-based password-cracking workflow using two Networkwalks tools:

1. **Hash Calculator**
2. **Password Cracker**

### Tools Used

* Networkwalks Hash Calculator
* Networkwalks Password Cracker
* Web Browser
* Windows PC / Kali Linux

---

## ⚙️ Networkwalks Workflow

### 1. Obtain the Encrypted PDF

Download:

```text
My Locked PDF1.pdf
```

### 2. Extract the Hash

Open the Networkwalks Hash Calculator:

https://networkwalks.com/hash-calculator/

Upload the encrypted PDF.

The generated PDF hash begins with:

```text
$pdf$...
```

Copy the complete hash.

### 3. Open the Password Cracker

Open:

https://networkwalks.com/password-cracker/

Paste the extracted hash into the Password Cracker and start the attack.

### 4. Recover the Password

The tool attempts different passwords until it finds a matching password.

### 5. Verify the Result

Open the encrypted PDF and enter the recovered password.

For the provided lab:

```text
password1
```

---

# 🔄 Comparison of the Two Approaches

| Feature         | John the Ripper                     | Networkwalks Tools                |
| --------------- | ----------------------------------- | --------------------------------- |
| Environment     | Windows / Kali Linux                | Web browser                       |
| Main Tool       | John the Ripper                     | Networkwalks Password Cracker     |
| GUI             | Johnny available                    | Web interface                     |
| Hash Extraction | External PDF hash extractor         | Networkwalks Hash Calculator      |
| Installation    | Required for JTR                    | No installation required          |
| Hash File       | `hash1.txt`                         | Not required                      |
| Main Purpose    | Hands-on password-cracking practice | Simplified browser-based workflow |

---

# 🧠 Key Concepts Learned

### Hashing

Hashing converts plaintext data into a digest. The lab describes hashing as a **one-way function**, unlike encryption, which is described as reversible when the appropriate key is available.

### Password Cracking

Password cracking attempts to recover the original password by testing possible passwords against the stored hash.

```text
Password-Protected PDF
          ↓
     Hash Extraction
          ↓
       PDF Hash
          ↓
   Password Cracking
          ↓
   Recovered Password
          ↓
     Open PDF
```

### Password Complexity

Cracking time can vary depending on password complexity and available computing resources.

---

# 🛡️ Security Takeaways

From these exercises, I learned that:

* Weak passwords can be vulnerable to password-cracking attempts.
* Password hashes should be properly protected.
* Password complexity affects the difficulty of recovery.
* Security professionals can use password-cracking tools to evaluate password security.
* Password-cracking techniques should only be used against systems and files where authorization has been given.

---

# 📸 Evidence

Screenshots from the completed exercises can be added to this repository.

Suggested structure:

```text
Password-Cracking/
│
├── README.md
│
├── JTR/
│   ├── 01-jtr-installation.png
│   ├── 02-hash-extraction.png
│   ├── 03-hash-file.png
│   ├── 04-johnny-setup.png
│   ├── 05-cracking-process.png
│   └── 06-password-recovered.png
│
└── Networkwalks/
    ├── 01-hash-calculator.png
    ├── 02-extracted-hash.png
    ├── 03-password-cracker.png
    ├── 04-cracking-process.png
    └── 05-password-recovered.png
```

To display a screenshot:

```markdown
![JTR Password Cracking](JTR/05-cracking-process.png)
```

---

# 🧰 Tools & Technologies

* **John the Ripper**
* **Johnny**
* **Networkwalks Hash Calculator**
* **Networkwalks Password Cracker**
* **Windows**
* **Kali Linux**
* **PDF Hash Extraction**
* **Password Hashing**
* **Password Cracking**

---

# 📚 References

* John the Ripper — Openwall:
  https://www.openwall.com/john/

* Johnny GUI — Openwall:
  https://openwall.info/wiki/john/johnny

* Networkwalks Hash Calculator:
  https://networkwalks.com/hash-calculator/

* Networkwalks Password Cracker:
  https://networkwalks.com/password-cracker/

---

## ⚠️ Ethical Use

All password-cracking activities documented in this repository are intended for **authorized cybersecurity training, educational labs, and security testing**.

Do not use these techniques against systems, accounts, files, or networks without explicit authorization.

---

## 👨‍💻 Project Status

**Week 3 — Completed**

**Student:** Syed Shaharyar Hussain
**Batch:** B083

### Modules Completed

* [x] Password Cracking with John the Ripper
* [x] Password Cracking with Johnny
* [x] PDF Hash Extraction
* [x] Password Cracking with Networkwalks Tools
* [x] Password Recovery Verification

---

**Cybersecurity & Ethical Hacking — Week 3**
