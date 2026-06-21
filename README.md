# Task 1 - Network Scanning and Reconnaissance

## Objective

To identify open ports, running services, and operating system information of target systems using network scanning tools.

## Tools Used

* Nmap
* Zenmap

## Procedure

1. Installed Nmap.
2. Selected the target system.
3. Performed network scanning using Nmap.
4. Identified open ports and running services.
5. Analyzed scan results.

## Sample Command

nmap -sV -A <target_ip>

## Results

* Identified active hosts.
* Discovered open ports.
* Enumerated running services.
* Gathered operating system information.

## Outcome

Successfully performed network reconnaissance and service enumeration using Nmap.

## Files Included

* Report PDF
* Screenshots
* README.md










# Task 2 - Vulnerability Assessment

## Objective

To identify known vulnerabilities in systems and applications using vulnerability assessment tools.

## Tools Used

* OpenVAS
* Nessus

## Procedure

1. Installed and configured the vulnerability scanner.
2. Created a new scan task.
3. Selected the target system.
4. Executed the vulnerability scan.
5. Analyzed vulnerability findings and risk scores.

## Activities Performed

* Vulnerability discovery
* Risk assessment
* CVSS score analysis
* Review of remediation recommendations

## Results

* Identified potential security weaknesses.
* Reviewed vulnerability severity levels.
* Examined recommended mitigation measures.

## Outcome

Successfully performed vulnerability assessment and analyzed security risks.

## Files Included

* Report PDF
* Screenshots
* README.md










# Task 3 - Web Application Penetration Testing

## Objective

To perform web application penetration testing using Burp Suite and OWASP Juice Shop.

## Tools Used

* Burp Suite Community Edition
* Docker Desktop
* OWASP Juice Shop

## Procedure

1. Installed Docker Desktop.
2. Deployed OWASP Juice Shop locally.
3. Opened the application through Burp Suite.
4. Captured HTTP traffic using HTTP History.
5. Mapped the application using Site Map.
6. Analyzed requests and responses.
7. Used Repeater to replay requests and inspect server responses.

## Activities Performed

* Traffic interception
* Site mapping
* Request analysis
* Response analysis
* Request replay using Repeater

## Results

* Successfully captured HTTP traffic.
* Mapped application endpoints.
* Analyzed requests and responses.
* Verified server responses using Repeater.

## Outcome

Successfully completed web application penetration testing activities using Burp Suite and OWASP Juice Shop.

## Files Included

* Report PDF
* Screenshots
* README.md





# Task 4 - Password Cracking

## Objective

The objective of this task is to evaluate password strength by performing password hash cracking using John the Ripper. This task helps in understanding how weak passwords can be recovered through dictionary-based attacks and emphasizes the importance of strong password security practices.

## Tools Used

* Kali Linux
* John the Ripper
* Terminal
* Custom Wordlist

## Procedure

### Step 1: Verify Installation

Verified that John the Ripper was installed and working correctly in Kali Linux.

```bash
john --version
```

### Step 2: Generate Password Hash

Generated an MD5 hash for a sample password using:

```bash
echo -n "password123" | md5sum
```

Generated Hash:

```text
482c811da5d5b4bc6d497ffa98491e38
```

### Step 3: Create Hash File

Stored the generated hash in a file named:

```text
hashes.txt
```

### Step 4: Create Custom Wordlist

Created a custom wordlist named:

```text
passwords.txt
```

Contents:

```text
123456
admin
welcome
password123
qwerty
```

### Step 5: Perform Password Cracking

Executed John the Ripper using the custom wordlist:

```bash
john --format=raw-md5 --wordlist=passwords.txt hashes.txt
```

### Step 6: Display Cracked Password

Displayed the recovered password:

```bash
john --show --format=raw-md5 hashes.txt
```

## Result

John the Ripper successfully cracked the MD5 hash using the provided wordlist and recovered the original password.

**Recovered Password:**

```text
password123
```

## Learning Outcomes

* Learned the fundamentals of password hashing.
* Understood dictionary-based password attacks.
* Gained practical experience using John the Ripper.
* Learned how weak passwords can be easily compromised.
* Understood the importance of using strong and unique passwords.

## Conclusion

This task successfully demonstrated password auditing and password hash recovery using John the Ripper. The experiment highlighted the risks associated with weak passwords and reinforced the importance of implementing strong password security practices.



