# KaliLinux-Metasploit

# Description
Project Consist of using Kali Linux Vm to Scan Metasploitable 2 For Security Flaws and Vulnerabilities to be fixed and reduce attack surface, tools used were Nmap, and Nessus
Vulnerability Scanning tool. Nmap command was used to show how many open TCP and UDP ports were open on the device, while The Nessus Scan Displayed the amount of Vulnerabiliies on the device, the CVSS score, and the Remediation steps to reduce attack Surface.

# Environments Used
Kali Linux VM Debian 
Metasploitable 2 VM

# Program Walk through
Running ifconfig command for Ip address for Vm to run scans against https://imgur.com/a/DQr4X04

Running Ping command on Kali Linux Vm to make sure there is communication between machines https://imgur.com/0IVAzZ0

Using Nmap -sT command to show how many TCP ports are open on Metasploitable VM https://imgur.com/SEMZRkk

Nmap -sU Command shows the amount of open UDP ports on Metasploitable VM https://imgur.com/OuWE0qD

Nessus Scan took 20 minutes to complete on kali Linux Vm https://imgur.com/0yqJT4n

72 vulnerabilities were found https://imgur.com/E6dqXlB

# Top 5 Vulnerabilities found from Nessus Scan and remidiation tips
1.NFS Exported Share information with this attacker may be able to leverage this to read, and possibly write files on the remote host 

Remidiation- Configure NFS on the remote host, so that only authorized host can mount its remote shares.

2.Unix operating system Unsupported Version Detection remote host is no longer supported, lack of support implies no new security patches for product making it susceptible for Zero-day attacks, Priveledge Escalation, and Dos Attacks.

Remidiation-Upgrade to a version of the unix operating system that is currently supported.

3.VNC Server ‘Password’ VNC Server on remote host is secured with a weak password, An attacker could exploit this with brute force or other password cracking methods to take control of the system.

Remediation-Solution would be to Secure with a Strong Password.

4.SSL Version 2 and 3 Protocol Detection Remote Service accepts connections using SSL 2.0 and SSL 3.0 SSL is no longer Acceptable Via Nist Recommendations Can be susceptible to Man-in-the-middle attacks or On Path Attacks

Remediation-Use TLS 1.2 with approved cipher suites or higher instead.

5.Bind Shell Backdoor Detection A shell is listening on the remote port without any authentication being required

Remediation-Verify if the remote host has been Compromised, and reinstall the system if necessary.




