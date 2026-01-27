#Kill Chain  
x) This article argues that conventional, vulnerability-focused security measures are insufficient against Advanced Persistent Threats. It proposes an Intrusion Kill Chain
framework to analyze adversary campaigns, prioritize defenses.  
Some of the main points are:  
1) Traditional network defense tools such as intrusion detection systems antivirus are insufficient agains sophisticated and well resourced opponents. The issue is that theu mainly assume that the intrusion has already happened.  
2) An evolution in defence is neccessary, shifting from vulnerability focus to threat focus. Intelligence-Driven Computer Network Defense (CND) is better suited as a defense mechanism in the modern day, because it focuses on threat, not just vulnerability.  
3) INtrusion KIll chain is key to mitigation and analyis. The kill chain model describes the phases of an intrusion, allowing defenders to anticipate and mitigate future intrusions.  
The intrusion kill chain is defined by seven phases: Reconnaissance, Weaponization, Delivery, Exploitation, Installation, Command and Control (C2), and Actions on Objectives

##A) Tactics, tools and procedures  
###Tactics  
An attack explains the purpose of what an attacker is trying to do. It answers the question why the attaker is doing something, rather than how. A tactic represents a goal during a cyberattack, and attackers may switch tactics as they move through different stages of their process.  
An example of a tactic is "Lateral Movement". IN this attack, the attackers goal is to move from one computer inside a network into other machines they did not have access to. They could for example break in to an employee's laptop and then try accessing the company's file server or domain controller.
###Techniques and subtechniques  
A technique describes how an attacker works torward a tactical goal. The focus in on the method the attacker uses, instead of ther reason why. Techniques help break down atacker behaviour.  
A good example of technique is "Remote Services". In this technique the attacker uses remoteaccess tools such as RDP or SSH to connect to another machine inside the network. This supports  the tactic mentioned previously, "LAteral Movement".  
Subtechniques are just more specific techniques, for example "Remote Services:SSH". This subtechnnique means the attacker is using SSH specifically to access another computer. It tells us precisely what remote service is being used.  
###Procedures  
A procedures describes a specific way an attacker performs a technique or subtechnique. It's not just a category or a specific method. It's an actual way of how attackers carried it out during a real inturusion. Procedures usually contain more details, like tools used, commands run etc.  
An exammple of a procedure would be:  
An attacker uses stolen SSH keys to log into a Linux server trough SSH and runs scripts to create a new user account on that system. It is a procedure because it show's all the steps taken: technique, tactic and real specific behaviour.  

##References  
https://attack.mitre.org/resources/faq/#general-faq  
https://terokarvinen.com/information-security/

