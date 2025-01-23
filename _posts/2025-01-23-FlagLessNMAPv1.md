---
title: "Introducing dsNMAP.py - dead simple NMAP"
date: 2025-01-22 17:56
categories: [Coding, Python, Projects, Cybersecurity]
tags: [Coding, Python, Cybersecurity, Linux]
pin: false # Set to `true` if you want this post pinned to the top.
---

# dsNMAP.py

I worked up a simple NMAP tool that prompts the user for IP and what degree of scan they are trying to accomplish on their local machine without having to remember nmap flags for themselves. 

This is just the first iteration. I saved and launched it locally using python3.

In the near future, I will put up a repository on GitHub.

### We're only human. 

To launch from terminal (assuming you have python3)
```bash
python3 ./dsNMAP.py 
```

Which produced this output:

```bash

      _     _   _ __  __          _____             
     | |   | \ | |  \/  |   /\   |  __ \            
   __| |___|  \| | \  / |  /  \  | |__) | __  _   _ 
  / _` / __| . ` | |\/| | / /\ \ |  ___/ '_ \| | | |
 | (_| \__ \ |\  | |  | |/ ____ \| |_  | |_) | |_| |
  \__,_|___/_| \_|_|  |_/_/    \_\_(_) | .__/ \__, |
                                       | |     __/ |
                                       |_|    |___/ 


    
Welcome to dsNMAP: The Dead Simple Nmap Scanning Tool!
Please enter the IP address or subnet you want to scan (e.g., 192.168.1.1 or 192.168.1.0/24): 192.168.240.1

Choose a scan level (the more invasive, the more detailed the scan):
1. 'The Peek' (Quick & Low-key, non-invasive)
2. 'The Look Around' (A little deeper, still friendly)
3. 'The Full Monty' (Warning: Very Invasive & Time Consuming!)
4. 'The All-Seeing Eye' (Super Invasive, Extremely Detailed - Proceed with Caution!)

Select the scan level (1-4): 1

You chose 'The Peek': A quick look to see if the host is up.

Initiating -sn scan on 192.168.240.1...

Starting Nmap 7.94SVN ( https://nmap.org ) at 2025-01-23 16:33 MST
Nmap scan report for firewalla.lan (192.168.240.1)
Host is up (0.0052s latency).
MAC Address: 20:6D:31:EF:9C:92 (Firewalla)
Nmap done: 1 IP address (1 host up) scanned in 0.07 seconds

Would you like to perform another scan? (y/n): n

Thank you for using dsNMAP! Goodbye.
```

## Here is the code. Dead simple. 

```python

      _     _   _ __  __          _____             
     | |   | \ | |  \/  |   /\   |  __ \            
   __| |___|  \| | \  / |  /  \  | |__) | __  _   _ 
  / _` / __| . ` | |\/| | / /\ \ |  ___/ '_ \| | | |
 | (_| \__ \ |\  | |  | |/ ____ \| |_  | |_) | |_| |
  \__,_|___/_| \_|_|  |_/_/    \_\_(_) | .__/ \__, |
                                       | |     __/ |
                                       |_|    |___/ 


    
Welcome to dsNMAP: The Dead Simple Nmap Scanning Tool!
Please enter the IP address or subnet you want to scan (e.g., 192.168.1.1 or 192.168.1.0/24): 192.168.240.1

Choose a scan level (the more invasive, the more detailed the scan):
1. 'The Peek' (Quick & Low-key, non-invasive)
2. 'The Look Around' (A little deeper, still friendly)
3. 'The Full Monty' (Warning: Very Invasive & Time Consuming!)
4. 'The All-Seeing Eye' (Super Invasive, Extremely Detailed - Proceed with Caution!)

Select the scan level (1-4): 1

You chose 'The Peek': A quick look to see if the host is up.

Initiating -sn scan on 192.168.240.1...

Starting Nmap 7.94SVN ( https://nmap.org ) at 2025-01-23 16:33 MST
Nmap scan report for firewalla.lan (192.168.240.1)
Host is up (0.0052s latency).
MAC Address: 20:6D:31:EF:9C:92 (Firewalla)
Nmap done: 1 IP address (1 host up) scanned in 0.07 seconds

Would you like to perform another scan? (y/n): n

Thank you for using dsNMAP! Goodbye.

```