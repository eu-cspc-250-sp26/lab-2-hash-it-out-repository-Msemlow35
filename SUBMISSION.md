# Hash It Out Lab - Submission

**Student Name:**  Mia Semlow 
**Date:** 2/10/2026  
**CSPC 250: Computer Systems Security**

---

## Part 1: Understanding Hashes (10 points)

### Exercise 1.1: Create Your First Hash

**1. What is the MD5 hash of your name?**

f520518d6a33de4116504f9a26a429d3

**2. Run the command again with the exact same name. Did the hash change? Why or why not?**

No it did not change because my name has already been hashed once

**3. Change one letter of your name (like capitalizing it) and run again. How different is the hash?**

Everything is different about the hash. Different letters and numbers in different orders.

---

### Exercise 1.2: Hash Collisions

**4. What is the md5sum of the file you created?**

[Your answer here]

**5. In your own words, explain what a hash collision is and why it's a security concern.**

A hash collision is when two different codes have the same hash, and its a concern because it can let people cheat or hack in very easily.

---

## Part 2: Password Storage (10 points)

### Exercise 2.1: Examine the Shadow File

**6. Why would a system have users with `*` instead of password hashes?**

Users with * instead of password hashes cannot log in with a password; these accounts exist only for system tasks or security purposes.

**7. What do the different parts of karl's password line mean? (Hint: Research the format of `/etc/shadow` entries)**

    7. $y$ → Which hashing algorithm (Yescrypt)
    j9T → Salt (random value)
    oR2Z… → Hashed password
    19255 → Last password change
    0 → Minimum days before next change
    99999 → Max days before change
    7 → Warning period before expiry
    ::: → Extra info (usually empty)

---

### Exercise 2.2: Understanding Password Hashing

**8. Why don't systems store passwords in plaintext?**

Systems don’t store plaintext passwords to protect user security and privacy. They store hashed versions instead.

**9. What is a "salt" in password hashing and why is it used?**

Salt is a radomized value added to a password before getting hashed to make it more secure.

**10. Research the `yescrypt` algorithm (the `$y$` prefix). Why is it considered secure?**

It is secure because it is a salted, slow hashing algorithm designed to resist brute. force and GPU based password attacks.

---

## Part 3: Password Cracking (15 points)

### Exercise 3.1: Crack Karl's Password

**11. What was karl's password?**

karl:test:19255:0:99999:7:::

**12. How long did it take John to crack it?**

It took John a couple seconds to crack it.

**13. Why was this password easy to crack?**



---

### Exercise 3.2: Verify the Password

**14. Does the hash match? (Yes/No)**

[Your answer here]

**15. What does this tell you about how Linux verifies passwords during login?**

[Your answer here]

---

## Part 4: Security Analysis (5 points)

**16. Based on this lab, what makes a password "strong"?**

[Your answer here]

**17. Why do websites now require passwords with numbers, symbols, and mixed case?**

[Your answer here]

**18. If you were designing a password policy for a company, what rules would you set? (At least 3 specific rules)**

[Your answer here]

---

## Screenshots Checklist

Include three screenshots in the `screenshots/` folder:

- [ ] `screenshot1.png` - Your name being hashed (Exercise 1.1)
- [ ] `screenshot2.png` - md5sum of your file (Exercise 1.2)
- [ ] `screenshot3.png` - John the Ripper cracking karl's password (Exercise 3.1)

---

## Reflection (Optional but Recommended)

What was the most interesting thing you learned in this lab?

[Your answer here]

---

## Academic Integrity Statement

By submitting this lab, I affirm that:
- I completed this work independently
- I did not copy answers from other students
- I did not use AI tools to generate my responses
- I understand the concepts and can explain them in my own words

**Signature (type your name):** [Your Name]  
**Date:** [Date]
