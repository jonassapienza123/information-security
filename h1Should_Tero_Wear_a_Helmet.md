# Should Tero wear a Helmet?

x)
Threat modeling is a structured way of thinking about security. The idea is to understand what we are building, what can happen to it, and how we can prevent the problems. Instead of guessing or reacting, it helps to identify risks early and prevent them.

Braiterman et al. — Threat Modeling Manifesto (2020)
The manifesto explains why threat modeling should be used, and who should use it. It touches on important values such as people and collaboration. 
According to the manifesto at the highest levels, when threat modeling, these four questions should be asked:
What are we working on?
What can go wrong?
What are we going to do about it?
Did we do a good enough job?

Adam Shostack — World’s Shortest Threat Modeling Course (2022)

This material mwntions the same four questions as listed above, which shows the importance of them. He also introduces the use of data flow diagrams, to visualize how data moves through systems, and where it ight be exposed to attacks. One of his main points is that threat modeling does not need to be heavy and complicated. Lightweight can still be valuable.

OWASP Threat Modeling Cheat Sheet (2021)

The OWASP cheat sheet is a more practical checlist on how to do threat modeling. Main points are defining scope, identifying assets and threats, deciding security controls, and prioritizing what to fix.


## A) 
There are many simple practices the average person and companies should follow. Some of the most important ones are listed below:
- Using strong and unique passwords
- Enabling multi-factor authentication
- Reqular software updates
- Being catious with emails and links
- Backing up important data
- Securing Wi-fi network
- Use Antivirus and Anti-Malware Software:

## B)
## Imaginary company  - ReadyFresh
  ReadyFresh is an imaginary food delivery subscription service. Meals are cooked at the ReadyFresh kitchen, and delivered to clients.
The business team's main goals are:
  - Customer satisfaction
  - Smooth orders and deliveries
  - Protecting personal and payment data
  - Keeping operations running
The technical team is responsible for explaining and deploying the systems.

# Threat modeling
  
## 1. What are we working on?

Our assets assets from most crtitical to leas
1. Customer data (names, adresses, emails, allergies, payment info
2. Operstional assets (order database, delivery route system, payment processing system, supplier contracts)
3. Infrastructure (cloud servers, internal admin portal)
4. Reputation

### Customer is king
To keep the business going we need to allow customers to browse meal kits, order and pay, track deliveries and receive support.

### Customer touchpoints
The customer interacts with the website/mobile app (wbrowsing and ordering meals), email notifications (looking for updates or order confirmation), notifictions from the delivery driver tracking delivery) and customer service chat.


## 2. What can go wrong?

We are applying STRIDE as our thret modeling methology. STRIDE is a Microsooft-developed framework, which categorizes threats into six types:
Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, and Elevation of Privilege.
Some examples of identified risks are:
Spoofing: attacker impersonates a customer account using stolen passwords.
Tampering: Order data is modified, which leads to wrong deliveries.
Information disclosure: customer data is leaked
Denial of service: Payment systems is taken down, which leads to no orders being processed
Elevation of privilege: attacker gains admin dshboard access.
Repudiation: disputes about fraudulent orders.  

#### Risk Prioritization

Looking at likelihood*impact, some of the risks are below. The higher on the list, the bigger the impact.

1. Payment data theft. No very common, but very damaging if it occurs. (fines, lawsuits, loss of trust) 
2. Ordering systems outage. LIkely to happen and stops all revenue.
3. Customer account takeovers. Common and harms trust.
4. DElivery route disruption. Annoying, but less harmful in the  bigger picture.

Specific threat actors are:

Cybercriminals want money or data..

Ransomware groups want to extort the company.

Competitors might want information.

Insiders can cause harm accidentally or on purpose.

## 3. What are we going to do about it?

To deal with the risks, the company should shrink it's attack service and close easy entry points.
The META model is a good way to think about responses.
Mitigate: make the risks smaller. (add MFA, encryption)
Eliminate: remove the risk entirely. (for example not storing credit cards at all)
Transfer: outsource the risk to someone else. (for example using a payment processor)
Accept: keep the risk if it's low and not worth fixing (for example non critical internal systems)

## 4. Did we do aa good enough job?
To check if our protections actually work we should do the following: security audits, penetration tests, and assesments. However, it does not cover all the basis, and threat modeling is a continous task. There is always new features, new attackers, and new weaknesses, whcih means that security is process that never ends.

  














## References
Cyber Hygiene
https://www.enisa.europa.eu/topics/cyber-hygiene
Threat Modeling Process
https://owasp.org/www-community/Threat_Modeling_Process#stride
APractical Guide to RIsk Response
https://www.metricstream.com/learn/risk-response.html?utm_source=chatgpt.com
