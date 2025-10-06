`# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

### Architecture Diagram

```
+----------------+        +------------------------+        +----------------------+
| Attacker's PC  | -----> | SET (Credential        | -----> | Fake Login Page      |
| (Kali Linux)   |        | Harvester via Apache)  |        | (Hosted by SET)      |
+----------------+        +------------------------+        +----------------------+
       |                                                             |
       |                                                             v
       |   1. Configure SET with phishing site (e.g., Gmail clone)   |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Victim's Browser     |
       | <------------------------------------------------| Clicks Phishing Link|
       |                                                 +----------------------+
       |                                                             |
       |                                                             v
       |     2. Victim Enters Credentials → Sent to SET/Attacker    |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Credentials Captured |
       |                                                 | in Apache log/SET DB |
       |                                                 +----------------------+

```

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers.

**Steps to Use SET for Phishing (Credential Harvester Attack Method)**



**1. Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method  
```
<img width="1920" height="1080" alt="KALI 2  Running  - Oracle VirtualBox 27-09-2025 09_49_35" src="https://github.com/user-attachments/assets/5a7a242b-e205-47f6-914a-5aa4dfb864b3" />


**2. Enter your IP address as the attacker server.**
<img width="1785" height="578" alt="Screenshot 2025-10-06 091850" src="https://github.com/user-attachments/assets/04e46849-8952-498c-8424-ec5a3e34688d" />

<img width="1305" height="610" alt="Screenshot 2025-10-06 091859" src="https://github.com/user-attachments/assets/05648dbf-2093-49ce-a2bc-470a361b55ac" />

<img width="1448" height="653" alt="Screenshot 2025-10-06 091917" src="https://github.com/user-attachments/assets/63ccb6d6-231c-4ff4-8287-3e8aaa472370" />

**4. Choose:**
```bash
2) Site Cloner
```
<img width="774" height="52" alt="Screenshot 2025-10-04 085520" src="https://github.com/user-attachments/assets/bb2d4621-081e-4b2c-ac26-7975d50decb1" />

**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**

<img width="1920" height="1080" alt="KALI 2  Running  - Oracle VirtualBox 27-09-2025 09_50_34" src="https://github.com/user-attachments/assets/77486ede-5b69-4abb-9808-015a9ae35076" />


**6. Send the generated link to the victim.**

**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```

<img width="1920" height="1080" alt="KALI 2  Running  - Oracle VirtualBox 27-09-2025 09_50_28" src="https://github.com/user-attachments/assets/31baa5b7-dbb8-4349-bdab-d8539c6aee75" />


## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
