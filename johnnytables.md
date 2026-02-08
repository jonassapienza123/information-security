#Johnny Tables  

###x)  
Top 10 (2021)  
A01:2021 – Broken Access Control  
- Happens when users can act outside their intended permissions.  
- Examples: viewing other users’ data, modifying accounts, accessing admin functions without authorization.  
My thought and question:  
Access control seems simple as a concept, but is easy to implement incorrectly. Why don’t more systems default to “deny everything unless explicitly allowed”.  
A05:2021 – Security Misconfiguration  
- Results from insecure default settings, incomplete setups, or overly detailed error messages.  
- Includes unnecessary features enabled, outdated software, or poorly configured cloud storage.  
My thought:  
Many breaches feel less like “hacks” and more like holes in the system.  
A06:2021 – Vulnerable and Outdated Components  
- Using libraries or frameworks with known vulnerabilities exposes applications.  
- Risks increase when organizations don’t track dependencies.  
My thought:  
Modern apps depend on huge dependency chains. Id it realistically possible for debvelopers to track all of them?  
A03:2021 – Injection  
- Occurs when untrusted input is interpreted as commands, for example SQL, OS, LDAP.  
- Classic example: SQL injection that lets attackers read or modify databases.  
xkcd 327 — Exploits of a Mom  
To my understanding the name of the child looks like or is a malicious sql injection. Calling it will  leak a database. The idea is to show that not sanitizing commands can lead to catastrophic results.  

