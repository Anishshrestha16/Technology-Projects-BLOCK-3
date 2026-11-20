# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/0a24230e-d766-4155-874e-00a>


### Questions

1.  How many users exist on the system? 34
2.  Which accounts appear to be system accounts? codingcomets and digitaldetectives
3.  Why do operating systems create system accounts? to save login details and make separate user preferences.

### Reflection

Explain why understanding system users is important for cybersecurity.
System users for personalization and separation of files and data for multiple users to use one system, or a network of>

------------------------------------------------------------------------


## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)

### Questions

1.  Which processes are running as `root`? SSH daemon, system logging, dhcpcd for networking, and desktop environment.
2.  Why can processes running as root be dangerous? Unlimited control over the user's system, changing all users settings and can mess with the device.
3.  What could happen if a malicious program ran with root privileges?  Make more malware, damage the system, spy on user activity, and read or change or delete files. 

### Reflection

What did you learn about system processes and security?

------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln


<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/894b894a-6909-4c65-8a71-99f>



### Questions


1.  Which ports are open? The first 3 udp and the first 2 tcp
2.  Which services appear to be listening? TCP appear to be the only ones listening
3.  Why might open ports represent a security risk? A known port may allow unknown users to connect with the system.


### Reflection


Explain the relationship between open ports and potential attack
surfaces.


Open points are entry points to the system, forming where attackers might exploit. More reachable services mean more misconfigerations and vulnerablities.

