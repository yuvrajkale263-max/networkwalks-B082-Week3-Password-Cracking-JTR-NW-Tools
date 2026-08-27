# Networkwalks-B082-Week3-Password-Cracking-JTR-NW-Tools
## Password cracking with John the Ripper (JTR), Johnny GUI, and Network walks password-cracking tools.

## 📌 Overview

During **Week 3 of my Cybersecurity Internship**, I completed two practical modules focused on **password cracking and password security**.

The labs demonstrated how a password-protected PDF can be analyzed by extracting its password hash and attempting to recover the original password using different password-cracking tools.

The two modules completed were:

1. **Module 1 – Password Cracking with John the Ripper (JTR)**
2. **Module 2 – Password Cracking with Networkwalks Tools**

> **Note:** These activities were performed as part of an authorized cybersecurity training lab using the provided password-protected PDF.

---

# 🔐 Module 1 – Password Cracking with JTR

## Objective

The objective of this module was to recover the password of a provided protected PDF using:

* **John the Ripper (JTR)**
* **Johnny GUI**, the graphical interface for John the Ripper
* A PDF hash extraction process

John the Ripper is a password-cracking tool used by security professionals to test password strength. Johnny provides a graphical interface that makes JTR easier to use for beginners.

## 🛠️ Tools Used

* John the Ripper
* Johnny GUI
* Windows PC
* PDF hash extraction tool
* Notepad

## 🔎 Procedure

### 1. Installed John the Ripper and Johnny

I downloaded and configured **John the Ripper** and **Johnny GUI** on my Windows system.

Johnny was configured to use the `john.exe` executable located in the JTR `run` directory.

### 2. Obtained the PDF Hash

I used a PDF hash extraction tool to extract the hash from the provided encrypted PDF.

The extracted value was stored in the format beginning with:

```text
$pdf$
```

The complete hash was then saved into a text file named:

```text
hash1.txt
```

### 3. Loaded the Hash into Johnny

I opened Johnny and used **Open password file** to load the `hash1.txt` file containing the extracted PDF hash.

### 4. Started the Password Attack

I started a new attack in Johnny. The tool attempted different password candidates until a matching password was found.

The time required for the attack depends on factors such as system performance and password complexity.

### 5. Verified the Password

After the password was recovered, I used it to open the encrypted PDF and successfully verified that the password worked.

## 🎯 Result

The protected PDF was successfully unlocked after recovering its password.

---

# 🌐 Module 2 – Password Cracking with Networkwalks Tools

## Objective

The second module demonstrated the same general password-recovery workflow using **Networkwalks' browser-based tools** instead of locally installed JTR software.

The two tools used were:

* **Networkwalks Hash Calculator**
* **Networkwalks Password Cracker**

Both tools operate through a web browser, so no local installation was required.

## 🛠️ Tools Used

* Networkwalks Hash Calculator
* Networkwalks Password Cracker

## 🔎 Procedure

### 1. Opened the Hash Calculator

I opened the Networkwalks **Hash Calculator** in a web browser and uploaded the provided locked PDF.

The tool extracted a PDF password hash beginning with `$pdf$`.

### 2. Copied the Complete Hash

I copied the complete extracted hash, ensuring that no portion of the `$pdf$` hash was missing.

### 3. Used the Password Cracker

I opened the Networkwalks **Password Cracker** and pasted the extracted hash into the appropriate field.

The tool then attempted different password candidates to find a matching password.

### 4. Waited for the Attack to Complete

The tool tested password candidates until it found a match.

The module demonstrated that the time required to recover a password depends on the complexity of the password.

### 5. Verified the Recovered Password

I entered the recovered password into the protected PDF and successfully opened the file, completing the lab.

---

# 🧠 Key Concepts Learned

## 1. Password Hashing

A password can be represented by a hash value rather than being stored directly. In the lab, the password hash was extracted from the protected PDF and used as the input for password recovery.

## 2. Password Cracking

Password cracking involves attempting different password candidates until one produces a matching result.

This demonstrated why weak or commonly used passwords can be vulnerable to password-cracking attacks.

## 3. Dictionary-Based Attacks

The Networkwalks Password Cracker demonstrated a **dictionary attack**, where password candidates are tested against the extracted hash until a match is found.

## 4. Password Complexity

The exercises demonstrated that password complexity affects the time required for password recovery. Simple passwords can be recovered more easily than stronger passwords.

## 5. Hashing vs Encryption

The module also highlighted the difference between encryption and hashing:

* **Encryption** is reversible when the appropriate key is available.
* **Hashing** is designed as a one-way transformation that produces a message digest.

---

# 📚 Skills Gained

Through these two practical labs, I gained hands-on experience with:

* Understanding password hashes
* Extracting hashes from password-protected PDFs
* Using **John the Ripper**
* Using the **Johnny GUI**
* Performing password-cracking attacks in a controlled lab
* Understanding dictionary-based password attacks
* Using browser-based password-cracking tools
* Understanding the relationship between password complexity and cracking time
* Understanding the security importance of strong passwords

---

# 📝 Week 3 Summary

Week 3 provided practical exposure to **password security and password-cracking techniques**.

I completed the same password-recovery objective using two different approaches: first with **John the Ripper and Johnny GUI**, and then with **Networkwalks' web-based Hash Calculator and Password Cracker**.

The labs helped me understand the complete workflow of a password-cracking exercise:

```text
Protected PDF
      ↓
Extract Password Hash
      ↓
Prepare Hash
      ↓
Password-Cracking Attack
      ↓
Recover Password
      ↓
Verify by Opening PDF
```

Overall, the exercises improved my understanding of how password attacks work and why strong, complex passwords are an important part of cybersecurity.

---

## ⚠️ Ethical Use

Password-cracking techniques should only be used on systems, files, accounts, or data for which you have explicit authorization.

This Week 3 work was performed as part of an authorized cybersecurity internship training lab.
