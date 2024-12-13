# Threat Modeling

## Threat Modeling Methodologies
* Adam Shostack's 4 questions
    - What are we working on 
    - What could go wrong
    - What are we going to do about it?
    -  Did we do a good job
* PASTA - Process for Attack Simulation and Threat Analysis 
    - Objective
    - Technical scope
    - Decompose the application
    - Threat analysis
    - Vulnerability analysis
    - Attack tree
    - Risk impact analysis and prioritization

* OWASP Threat modeling
    - Step 1: Scope your work
    - Step 2: Determine Threats
    - Step 3: Determine Countermeasures and Mitigation
    - Step 4: Assess your work    
* STRIDE
    - Spoofing Identity, - Authentication and authorization
    - Tampering with Data, - integrity of the data - validation
    - Repudiation, logging
    - Information Disclosure, - encruyption 
    - Denial of service, - availability
    - Elevation of Privilege - 

## MITRE ATT&CK framework
* **Reconnaissance**
* Resource Development
* **Initial Access**	
* Execution
* **Persistence**
* **Privilege Escalation**
* **Defense Evasion**
* Credential Access
* Discovery
* **Lateral Movement**
* Collection
* **Command and Control**
* **Exfiltration**
* Impact

## Common Threats: 
	Eavesdrop (interception)
	modify messages
	impersonation
    hijacking
    denial of service


## Theat Rating
Risk = Threat likelihood x Impact

**DREAD:** 

DAMAGE + REPRODUCIBILITY + EXPLOITABILITY + AFFECTED USERS + DISCOVERABILITY

## Tools:
Threat dragon by Mike goodwin
AWS Threat Composer
Microsoft Threat modeling tool
Irius Risk
Threat Modeler
