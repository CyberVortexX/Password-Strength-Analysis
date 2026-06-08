# 🔐 Password Strength Analysis

A hands-on security assessment evaluating how password composition affects resistance against real-world cracking techniques. Passwords of varying complexity were tested using an online strength checker, and results were documented to demonstrate the measurable impact of length, character diversity, and randomness.

---

## 📁 Repository Structure

```
Password-Strength-Analysis/
├── README.md                   ← Project overview (you are here)
├── analysis_report.md          ← Full evaluation findings and recommendations
├── password_samples.txt        ← Sample passwords used during testing
└── screenshots/
    ├── weak_password.png
    ├── medium_password.png
    ├── strong_password.png
    └── veryStrong_password.png
```

---

## 🎯 Objective

Evaluate passwords of varying complexity using a password strength checker and understand how different composition factors affect resistance against common password attacks.

---

## 🛠️ Tools Used

- **Password Strength Checker** — online tool for estimating password entropy and crack time
- **Web Browser** — for testing and capturing screenshots

---

## 🔑 Passwords Evaluated

| Password | Length | Character Types |
|---|---|---|
| `password123` | 11 | Lowercase + Numbers |
| `Cyber@123` | 9 | Upper + Lower + Numbers + Symbols |
| `P@ssw0rd2026!` | 13 | Upper + Lower + Numbers + Symbols |
| `Cyb3r$ecur1ty!2` | 15 | Upper + Lower + Numbers + Symbols |
| `CyberSecurity@2026` | 18 | Upper + Lower + Numbers + Symbols |
| `Cyb3r$ecur1ty!2026#Safe` | 23 | Upper + Lower + Numbers + Symbols |

---

## 📊 Evaluation Results

| Password | Rating | Estimated Crack Time |
|---|---|---|
| `password123` | 🔴 Very Weak | 0 seconds |
| `Cyb3r$ecur1ty!2` | 🟡 Medium | 46 hours |
| `CyberSecurity@2026` | 🟢 Strong | 7 months |
| `Cyb3r$ecur1ty!2026#Safe` | 🔵 Very Strong | 4 thousand years |

> Full breakdown with per-password observations is available in [`analysis_report.md`](./analysis_report.md).

---

## 🔬 Password Strength Factors

The following factors directly influence how long a password takes to crack:

| Factor | Impact |
|---|---|
| **Length** | Most impactful — each added character multiplies the key space |
| **Uppercase letters** | Expands character set from 26 to 52 |
| **Lowercase letters** | Baseline character category |
| **Numbers** | Adds 10 additional characters to the pool |
| **Special characters** | Adds 30+ characters; significantly raises entropy |
| **Randomness** | Unpredictable sequences resist dictionary and hybrid attacks |

---

## ⚔️ Common Password Attack Techniques

### Brute Force
Tries every possible character combination systematically. Defeated by **length and complexity**.

### Dictionary Attack
Uses precompiled lists of common words and leaked passwords. Defeated by **avoiding real words and predictable patterns**.

### Credential Stuffing
Replays username/password pairs from previous data breaches across other services. Defeated by **using unique passwords per account**.

### Password Spraying
Tests a few common passwords against many accounts to avoid lockout triggers. Defeated by **strong password policies and MFA**.

---

## ✅ Best Practices

1. Use a **minimum of 12–16 characters** — longer is always better.
2. Mix **uppercase, lowercase, numbers, and symbols** throughout.
3. Avoid **dictionary words**, names, or predictable substitutions (`@` for `a`, `3` for `e`).
4. Never **reuse passwords** across different accounts or services.
5. Do not include **personal information** such as birthdays or usernames.
6. Enable **Multi-Factor Authentication (MFA)** wherever available.
7. Use a **password manager** to generate and store strong, unique passwords.

---

## 📌 Conclusion

Password length and character diversity have an exponential — not linear — effect on security. A weak, predictable password is cracked in seconds; a long, complex password can withstand thousands of years of sustained attack. Adopting strong password habits is one of the most effective and low-cost security measures available.

---

## 📄 License

This project is for educational and research purposes only.
