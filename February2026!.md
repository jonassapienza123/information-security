# February2026!  

## X) 
### € Schneier 2015: Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions.  
- one-way functions are fundamental building blocks in various protocols
- easy to compute, significantly harder to reverse
- Not useful alone for encryption because no one could reverse them
- Trapdoor one-way function:  
Easy forward.  
Hard backward.  
Easy backward if you know a secret (trapdoor).  
- Foundation of public-key cryptography.
### € Schneier 2015: Applied Cryptography: 2.4 One-Way Hash Functions.  
Take input of any length and produce fixed-length output (hash).  
Used as a “fingerprint” of data.  
Easy to compute hash, hard to reverse it.    
Hard to find two different inputs with the same hash (collision).  

## b)  
First I updated packages.  
<img width="732" height="333" alt="Screenshot From 2026-03-01 14-21-14" src="https://github.com/user-attachments/assets/8f5d96ca-4107-450f-86c2-9a2e655b94fb" />   
I then installed hashcat.   
<img width="732" height="142" alt="Screenshot From 2026-03-01 14-28-01" src="https://github.com/user-attachments/assets/2bbb889c-abbc-44d7-9427-bbcb7c46b8ef" />  
I used the command given by the teahce, and added the hash which we are cracking. Also saved the solution as plain text to a new file called "solved".    
<img width="730" height="458" alt="Screenshot From 2026-03-01 14-41-44" src="https://github.com/user-attachments/assets/7ab6e084-fa54-48f1-8b17-627b1b174495" />  
Using comand "cat solved" I could see the hash and the solution in plain text, which was disobey:  
<img width="733" height="76" alt="Screenshot From 2026-03-01 14-45-13" src="https://github.com/user-attachments/assets/f0c699ea-471b-4afb-b48c-5d6863dd7104" />  


## References  
Karvinen 2022: Cracking Passwords with Hashcat  
€ Schneier 2015: Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions.  



  
