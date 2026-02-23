# Uryyb, Greb!  

### x) € Schneier 2015 — Applied Cryptography: Chapter 1: Foundations  
- Cryptography is about keeping information safe: making sure only the right people can read it and that it hasn’t been changed.
- Encryption turns readable text into unreadable form, and keys are what make it secure, instead of hiding the method.
- There are two main types: shared secret keys and public/private key pairs.
- Attackers are assumed to know how the system works, so security must rely on strong design.
- Even good algorithms can fail if the protocol or implementation is bad.

### Karvinen 2023: PGP - Send Encrypted and Signed Message - gpg  
- PGP ,with GnuPG, is used to encrypt messages and prove who sent them.
- You create a key pair: a public key to share and a private key to keep secret.
- To send a secure message, you encrypt it with the recipient’s public key so only they can read it.
- You can also sign messages with your private key so others know it really came from you.
- Keys can be exported and shared, and fingerprints help verify they’re correct.

### a) install OpenSSH server
Installed OpenSSH server  
<img width="734" height="189" alt="Screenshot From 2026-02-23 12-26-25" src="https://github.com/user-attachments/assets/33929db4-aa10-4749-b31a-1b16bc8828cf" />

Started the service  
<img width="639" height="480" alt="Screenshot From 2026-02-23 12-33-23" src="https://github.com/user-attachments/assets/2b59f759-0bda-4ea2-9c94-f5008c7acee7" />

Connected with ssh username@localhost  
<img width="639" height="480" alt="Screenshot From 2026-02-23 12-35-11" src="https://github.com/user-attachments/assets/e9740eeb-60a1-448d-abdc-ade85be68b8b" />  

### b) Automate SSH   
First I generated SSH key with ssh-keygen  
<img width="1920" height="921" alt="Screenshot From 2026-02-23 13-37-28" src="https://github.com/user-attachments/assets/2cf09b5b-65f9-4071-be36-32f0b05f85af" />  
I then copied public key using ssh-copy-id 
<img width="1920" height="921" alt="Screenshot From 2026-02-23 13-39-07" src="https://github.com/user-attachments/assets/37562bc1-719b-4c9b-b3c2-3bf9233b2ec5" />  
Then I verified login works without password, it asked for the passphrase I created, so it was succesful.  
<img width="1920" height="921" alt="Screenshot From 2026-02-23 13-39-54" src="https://github.com/user-attachments/assets/5a749fb8-c5fb-499e-a796-6e247a17b764" />  

### c) Password manager
I installed keepassxc. 
<img width="1920" height="921" alt="Screenshot From 2026-02-23 13-48-42" src="https://github.com/user-attachments/assets/572be202-b3b2-4d75-9dbc-cd924d7af02a" />  
On KeePassxc, I created a new database named Passwords. When creating it, it asked me for a strong master password. After saving the file, I was able to add a new entry. I clicked the dice icon and was able to generate  a new password.  
<img width="1920" height="921" alt="Screenshot From 2026-02-23 13-52-46" src="https://github.com/user-attachments/assets/7a25135c-a2be-47fe-a1f9-d8a84f6e2a57" />
<img width="1920" height="921" alt="Screenshot From 2026-02-23 13-52-56" src="https://github.com/user-attachments/assets/1cc14fc7-2d63-468b-8c97-31af136176ee" />   
WHy a Password manager is needed?  
- People often reuse passwords across sites.  
- Password managers generate strong and unique passwords.  
- They store passwords securely so you don’t have to remember them.  
- Using one reduces risk if a site is breached.
  
Some of the threats it protects against are:  
Password reuse attacks, where an attacker tries using a leaked password on other sites.  
Phishing attacks, because a manager helps avoid typing passwords manually.  
Weak passwords, because a manager creates stong ones.  
Force guessing, because generated passwords are long and hard to guess.  

### s) ETAION  
At first look it looked very confusing, but then I saw a ffew things I was able to start with. DHHP:// most likely stands for HTTPS:// , and .OWG for .COM. I laso saw 'YI, and I could only think of 're as the replacement  
in english language. So I started with replacing all the corresponding letters with the one I figured out.  
![cipher](https://github.com/user-attachments/assets/c0de4a73-814f-4b37-8fd0-56067a3cc63c)  
I then figured out that the website was terokarvinen.com. Figuring this out helped me change some corresponding letters in the encrypted message again, and I started looking at the shortest words, because they are the easiest to figure out, for example: see, at, can, be etc. I was then able to replca some letters again and some words started to form, where I was able to guess the remaining letter of that word.  
![CIPHER1](https://github.com/user-attachments/assets/c816569b-ea6d-445d-8238-f7edcb91e6eb)  
![CIPHER3](https://github.com/user-attachments/assets/cefb0388-4962-40ea-bb76-e4a85b59dd9e)  
Unfortunately this was the furthest I got, and I was not able to crack the whole code after trying for a long time.








