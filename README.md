# Cyber Security Internship - Task 6
## Topic: Password Strength Evaluation and Security Best Practices

---

## 1. Introduction
The primary objective of this task is to understand the core principles of password security, evaluate passwords of varying complexities using strength assessment tools, and analyze common password-based attacks. Below is a detailed comparative analysis and documentation based on the task guidelines.

---

## 2. Password Strength Evaluation Table
Three distinct passwords with varying complexity levels were generated and tested using **PasswordMeter** and standard computational estimation tools to analyze their strength and predictability:

| Password Type | Example Password | Strength Score | Estimated Time to Crack | Feedback / Weakness |
| :--- | :--- | :--- | :--- | :--- |
| **Weak (Low)** | `password123` | 10% (Very Weak) | Instantly | Contains only lowercase letters and sequential numbers. Uses a common dictionary word. |
| **Medium** | `Secure#2026` | 60% (Medium) | A few days / months | Includes uppercase, lowercase, symbols, and numbers, but the length is short (11 characters) and follows a predictable pattern. |
| **Strong (High)** | `Tr0p$c4L!W4t3r#99` | 100% (Very Strong) | Centuries | Outstanding length (16+ characters). Features an excellent random mix of cases, symbols, and numbers with no dictionary words. |

---

## 3. Common Password Attacks
*   **Brute Force Attack:** In this attack, threat actors use automated software to systematically try every possible combination of characters (letters, numbers, and symbols) until the correct password is found. Shorter passwords are highly vulnerable to this method.
*   **Dictionary Attack:** An automated technique where the attacker attempts to gain authentication by stepping through a predefined list of words (wordlists), such as standard dictionary terms, common names, or leaked credentials (e.g., `admin`, `password`, `qwerty`).

---

## 4. Key Takeaways & Best Practices
*   **Length over Complexity:** Password length is mathematically superior to complexity alone. A 12-to-16-character password drastically expands the search space ($$Entropy$$), making it exponentially harder to crack.
*   **Avoid Predictable Patterns:** Capitalizing only the first letter or appending predictable sequences like `123`, `2026`, or `!` at the end creates distinct patterns that modern password crackers prioritize.
*   **Use Passphrases:** Instead of a single complex word, combining 3 to 4 random, unrelated words (e.g., `Blue#Elephant$Running%Tree`) results in a highly secure and long credential that is easy for humans to remember but incredibly hard for machines to guess.

---

## 5. Interview Questions & Answers

### Q1. What makes a password strong?
**Ans:** A password is considered strong when it is at least 12–16 characters long and contains a randomized mixture of uppercase letters (A-Z), lowercase letters (a-z), numbers (0-9), and special symbols ($, #, @, !). Crucially, it must not contain any personal information or dictionary words.

### Q2. What are common password attacks?
**Ans:** The most prevalent password attacks include:
1. **Brute Force Attack:** Testing all character combinations.
2. **Dictionary Attack:** Using a precompiled list of common words/passwords.
3. **Credential Stuffing:** Automated testing of leaked username/password pairs across different sites.
4. **Phishing:** Tricking users into revealing their credentials via fraudulent pages or emails.

### Q3. Why is password length important?
**Ans:** As the length of a password increases, the number of potential combinations expands exponentially. This geometric escalation drastically multiplies the time and computational power required for an attacker to execute a successful brute-force crack.

### Q4. What is a dictionary attack?
**Ans:** A dictionary attack is a targeted authentication bypass method where an attacker runs a program that tries thousands of words from a pre-arranged list (wordlist). It is significantly faster than a pure brute-force attack because it avoids testing random character strings and focuses on high-probability words.

### Q5. What is multi-factor authentication (MFA)?
**Ans:** MFA is an identity verification mechanism that requires a user to supply at least two different verification factors before gaining access. This typically combines something you know (password) with something you have (an OTP on a phone, or a token from Google Authenticator) or something you are (biometrics like fingerprints).

### Q6. How do password managers help?
**Ans:** Password managers generate, store, and encrypt highly complex, unique passwords for every single account a user owns. By keeping everything securely stored under one master password, it eliminates the habit of reusing passwords across multiple platforms.

### Q7. What are passphrases?
**Ans:** A passphrase is a sequence of random words joined together to form a long password (e.g., `correcthorsebatterystaple`). They offer premium security because their immense length makes them computationally unfeasible to crack, yet they remain highly memorable for the user.

### Q8. What are common mistakes in password creation?
**Ans:** The most widespread mistakes are:
1. Reusing the exact same password across multiple websites.
2. Using easily predictable patterns, dictionary terms, or personal info (names, birth years).
3. Keeping passwords short (under 8 characters).
4. Storing credentials as unencrypted plain text in notes files or web browsers.
