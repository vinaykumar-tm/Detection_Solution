# Detection_Solution
>SIEM detection solutions 


Attacks 

## 1. [Ransomware](https://en.wikipedia.org/wiki/Ransomware)
**What it is**:- A type of malware that encrypts files and requests a ransom(money payment)from the user to decrypt the traffic

**Threat Indicators**:- User contacting: Burst of “file update” logs Anti-virus alerts; Connection to suspicious IPs

**Where to Investigate**:-  AV Logs: OS Logs; Account Logs; Network traffic; etc.

**Possible Actions**:-  Request AV checks; Isolate the machine; turn off the machine.

## 2. [Brute Forcing](https://en.wikipedia.org/wiki/Brute-force_attack)
**What it is**:-  An attacker trying to guess a password by attempting several different passwords

**Threat Indicators**:-  Multiple login failures in a short period of time

**Where to investigate**:-  Active Directory Logs; Application Logs; Operational System logs; Contact user

**Possible Actions**:- If not legit action, disable the account and investigate/block the attacker

## 3. [Botnets](https://www.paloaltonetworks.com/cyberpedia/what-is-botnet)
**What it is**:-  when attackers are using the victim server to perform DDoS attacks or other malicious activities.
 
**Threat Indicators**:- Connection to suspicious IPs; Abnormally high volume of network traffic

**Where to investigate** :-  Network traffic; Os logs(new Process); Contact server owner; Contact support teams;

**Possible Actions**:-   If confirmed; Isolate the server; Remove malicious process; Patch the vulnerability utilized for infection.

## 4. [Advanced Persistent Threats](https://en.wikipedia.org/wiki/Advanced_persistent_threat)
**What it is**:-  when attackers get access to the system and create backdoors for further exploitation. Usually hard to detect.

**Threat Indicators**:- Connection to suspicious IPs; Abnormal high volume of network traffic; Off-hours access logs; New admin account creations;


**Where to investigate** :-  Network traffic; Access logs; Os logs(New Processes, new connections, abnormal users); Contact server owner/support teams;

**Possible Actions**:-  If confirmed; Isolate the machine; Start formal forensics process; Start escalations/communication plan

## 5.[Compromised Accounts](https://en.wikipedia.org/wiki/Wikipedia:Compromised_accounts)
**What it is**:-  When an attacker gets access to one account (via social engineering or other methods)

**Threat Indicators**:-  Off-hours account logins; Account group changes; Abnormal high network traffic;

**Where to investigate**:-  Active Directory logs; OS logs; Network traffic; Contact user for clarifications.

**Possible Actions**:-  If confirmed: Disable account; Password changes; Forensic investigations

## 6.[Data Exfiltration](https://en.wikipedia.org/wiki/Data_exfiltration)
**What it is**:-   when an attacker(or rogue employee) exfiltrate data to external sources

**Threat Indicators**:-  Abnormal high network traffic; Connection to cloud-storage solutions(Dropbox, Google Cloud, etc); Unusual USB sticks;

**Where to investigate**:-  Network traffic; Proxy logs; OS logs

**Possible Actions**:-  if rogue employee; contact manager, perform full forensics If external threat; Isolate the machine, disconnect from network

## 7.[Denial of Service(DOS / DDoS)](https://www.investopedia.com/terms/d/denial-service-attack-dos.asp)
**What it is******:-  When an attacker is able to cause interference in a system by exploiting DoS vulnerabilities or by generating a high volume of traffic

**Threat Indicators**:-  Abnormal high networks in public-facing servers;

**Where to investigate**:-  Networks traffic; Firewall logs; OS logs;

**Possible Actions**:-  If Dos due to vulnerabilities; Contact patching team for remediation; if DDoS due to network traffic; Contact network support or ISP
