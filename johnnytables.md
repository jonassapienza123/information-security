# Johnny Tables  

### x)  
Top 10 (2021)  
### A01:2021 – Broken Access Control  
- Happens when users can act outside their intended permissions.  
- Examples: viewing other users’ data, modifying accounts, accessing admin functions without authorization.  
My thought and question:  
Access control seems simple as a concept, but is easy to implement incorrectly. Why don’t more systems default to “deny everything unless explicitly allowed”.  
### A05:2021 – Security Misconfiguration    
- Results from insecure default settings, incomplete setups, or overly detailed error messages.  
- Includes unnecessary features enabled, outdated software, or poorly configured cloud storage.  
My thought:  
Many breaches feel less like “hacks” and more like holes in the system.  
### A06:2021 – Vulnerable and Outdated Components    
- Using libraries or frameworks with known vulnerabilities exposes applications.  
- Risks increase when organizations don’t track dependencies.  
My thought:  
Modern apps depend on huge dependency chains. Id it realistically possible for debvelopers to track all of them?  
### A03:2021 – Injection  
- Occurs when untrusted input is interpreted as commands, for example SQL, OS, LDAP.  
- Classic example: SQL injection that lets attackers read or modify databases.  
### xkcd 327 — Exploits of a Mom  
To my understanding the name of the child looks like or is a malicious sql injection. Calling it will  leak a database. The idea is to show that not sanitizing commands can lead to catastrophic results.
### a) installed, as shown below
### b)  
I installed webgoat on my Debian and ran it locally. I accessed webgoat through my browser at http://localhost:8080, so it was my own machine and a safe enviroment.  
I then used devtool F12 to inspect the Network tap and analyze http request and response between the client and the server. I first had some difficulties finding the request in the correct tab, but then finally found it in the response data, and succesfully managed to find the correct number.  
It demonstrated how web applications communicate and showed the importance of not exposing sensivtive information in server responses.  
<img width="636" height="408" alt="2026-02-08 (18)" src="https://github.com/user-attachments/assets/ffd4522e-6a08-4355-990d-f1fab35dd5a4" />  
### c)  
I updated the operating system and applications to make sure the latest security patches were installed, using these commmands:  
sudo apt update  
sudo apt upgrade -y  
sudo apt autoremove -y   
### d)  
I learned how to retrieve data from a database using the SELECT statement and filter results with the WHERE clause. This helped me understand how databases are queried and how structured data can be accessed efficiently. It ws interesting and helpful, especially since I do not have much experience with SQL.  
<img width="730" height="417" alt="2026-02-09 (1)" src="https://github.com/user-attachments/assets/d82bc74f-53db-4171-8643-7d9906ce863f" />  
<img width="742" height="419" alt="2026-02-09" src="https://github.com/user-attachments/assets/efc361cd-4ef3-4c95-971d-26d9640163a6" />  
### e)  
I modified the category parameter in the URL, by injecting a condition that is always true, which caused the database to return all products instead of only the intended ones. I modified the parameter by adding ' OR 1=1-- , and removing the category name. THis creates a condition which is always true and caused the database to return all records.  
<img width="875" height="433" alt="2026-02-09 (2)" src="https://github.com/user-attachments/assets/49bdfaa6-f79f-417e-b7b0-2e7a6ec043b3" />  

## References  
Tee
OWASP Foundation. (2021). OWASP Top Ten. https://owasp.org/www-project-top-ten/  
WebGoat. OWASP Foundation. https://owasp.org/www-project-webgoat/  
PortSwigger. SQL injection vulnerability in WHERE clause allowing retrieval of hidden data.   https://portswigger.net/web-security/sql-injection  
SQLZoo. SQL Tutorial. https://sqlzoo.net/wiki/SQL_Tutorial  
Munroe, R. (2007). Exploits of a Mom (xkcd 327). https://xkcd.com/327/  
Karvinen, T. Information Security. https://terokarvinen.com/information-security  









