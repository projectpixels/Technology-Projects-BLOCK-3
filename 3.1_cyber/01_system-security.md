# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/e8ff4656-a2d6-4e62-9946-4d920ea93885" />


### Questions

1.  How many users exist on the system?
ans= 37 users
2. Which accounts appear to be system accounts?
ans= daemon, bin, sys, www-data, sshd, etc
3.  Why do operating systems create system accounts?
   ans= ...
### Reflection

Explain why understanding system users is important for cybersecurity.
  most attacks exploit people and their accounts, not the technology itself.
  knowing who uses a system lets you limit access spot abnormal behaviour, and build controls people will follow.
------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/01f94ed5-f98d-4c22-831b-6d5d5e0cc663" />


### Questions

1.  Which processes are running as `root`?
 ans=/sbin/init splash (PID 1), kthreadd, kworker/*, ksoftirqd etc
2.  Why can processes running as root be dangerous?
ans= Root has unrestricted access, so a bug or compromise gives an attacker full control of the system.
3.  What could happen if a malicious program ran with root privileges?
   ans= It could read, change or delete any file, install backdoors or rootkits, create accounts, disable security tools, erase logs and spread to other machines.

### Reflection

What did you learn about system processes and security?
ans= Running processes show what the system is doing and under which user. Processes running as root carry the most risk, so services should use the least privilege they need.

------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot

(Add screenshot here)

### Questions

1.  Which ports are open?
2.  Which services appear to be listening?
3.  Why might open ports represent a security risk?

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
