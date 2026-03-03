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

## a)  
I installed haschat, you can see the latest version active in the screenshot below:  
<img width="744" height="479" alt="Screenshot From 2026-03-03 14-52-29" src="https://github.com/user-attachments/assets/48da38b6-d6d9-43cf-8ac8-80195b819b74" />    
I ran hashcat --benchmark to test that Hashcat works correctly. The benchmark measured hashing performance in hashes per second.    
<img width="744" height="479" alt="Screenshot From 2026-03-03 14-53-12" src="https://github.com/user-attachments/assets/df86c597-aac0-4f3e-902e-6a45d68bb8a9" />  
I generated a sample hash using the MD5 algorithm by running echo -n 'example123' | md5sum in the terminal.  
<img width="744" height="65" alt="Screenshot From 2026-03-03 14-54-59" src="https://github.com/user-attachments/assets/136d18c1-84ee-49d1-9a16-579574389d26" />  




## b)  
First I updated packages.  
<img width="732" height="333" alt="Screenshot From 2026-03-01 14-21-14" src="https://github.com/user-attachments/assets/8f5d96ca-4107-450f-86c2-9a2e655b94fb" />   
I then installed hashcat.   
<img width="732" height="142" alt="Screenshot From 2026-03-01 14-28-01" src="https://github.com/user-attachments/assets/2bbb889c-abbc-44d7-9427-bbcb7c46b8ef" />  
I got the dictionary.  
<img width="729" height="61" alt="Screenshot From 2026-03-01 15-11-02" src="https://github.com/user-attachments/assets/df5a50c9-c02b-4073-aeb7-f28557affa7d" />  
I used the command given by the teahce, and added the hash which we are cracking. Also saved the solution as plain text to a new file called "solved".    
<img width="730" height="458" alt="Screenshot From 2026-03-01 14-41-44" src="https://github.com/user-attachments/assets/7ab6e084-fa54-48f1-8b17-627b1b174495" />  
Using comand "cat solved" I could see the hash and the solution in plain text, which was disobey:  
<img width="733" height="76" alt="Screenshot From 2026-03-01 14-45-13" src="https://github.com/user-attachments/assets/f0c699ea-471b-4afb-b48c-5d6863dd7104" />  


## References  
Karvinen 2022: Cracking Passwords with Hashcat  
€ Schneier 2015: Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions.  



  
