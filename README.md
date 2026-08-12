# Akanksha — SECURE STATIC MASTER

Password: **1914**

This version uses a client-side encrypted birthday payload:
- Before the correct password, the birthday HTML, CSS, JavaScript, photos, and decorations are ciphertext.
- The password is not stored in the page source.
- The browser decrypts the birthday only after the correct password is entered.
- The password gate uses PBKDF2-SHA256 + AES-256-GCM.

Important limitation:
This is the strongest practical **free/static** approach for GitHub Pages, but it is not equivalent to server-side authentication. A 4-digit password such as 1914 can be brute-forced by someone determined enough, and anything displayed after unlocking can always be inspected by that browser. For a 10–15 day personal surprise, this is much stronger than a normal JavaScript password gate.
