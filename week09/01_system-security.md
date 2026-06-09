# Exploring Your System's Security
To explore the system users, I used the command cat/ etc/ passwd, which displays all the user accounts stored on the system. This file contains important information such as username, user IDs, group IDs, home directories, and default shells.
## Task 1 --- List System Users

Run: After running the command, I observed that the systen has multiple users, including both system user( like root and service accounts) and regular users. System users are mainly used by the operating system and background service, while regular users are created for human interaction.

    cat /etc/passwd

### Screenshot

(Add screenshot here)

### Questions

1.  How many users exist on the system?
2.  
3.  Which accounts appear to be system accounts?
4.  System accounts are usally built-in profile crested by the operating system rather than teal people. You can easily spot them because they have names like root, bin, daemon, sys, nobody, systemd network, or messagebus. Another dead giveaway on Linux systems is their User ID (UID)-system accounts almost always have a UID below 100o ( or below 500, depending on the specific distribution setup).
5.  Why do operating systems create system accounts?
6.  Operating system use these separate accounts to keep things  safe and organized through concept called ''least privilege.'' Inestead of running every background process and service with full administrative power (like root), the OS gives each background task its own limited account.

### Reflection

Explain why understanding system users is important for cybersecurity.

------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)

### Questions

1.  Which processes are running as `root`?
2.  Why can processes running as root be dangerous?
3.  What could happen if a malicious program ran with root privileges?

### Reflection

What did you learn about system processes and security?

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
