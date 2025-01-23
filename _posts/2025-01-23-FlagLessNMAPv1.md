---
title: "Tired of remembering NMAP flags? Me too. So here's a tool I made to make it a litte easier."
date: 2025-01-22 17:56
categories: [Coding, Python, Projects, Cybersecurity]
tags: [Coding, Python, Cybersecurity, Linux]
pin: false # Set to `true` if you want this post pinned to the top.
---

I worked up a simple NMAP tool that prompts the user for IP and what degree of scan they are trying to accomplish on their local machine without having to remember nmap flags for themselves. 

This is just the first iteration. I saved and launched it locally using python3.

We're only human. 

To launch
```bash
python3 ./FlaglessNMAP.py 
```

Which produced this output:

```bash
Welcome to the Dead Simple Nmap Scanning Tool
Enter the IP address you want to scan: 192.168.240.1

Scan Levels:
1. Ping Scan (Check if the host is up)
2. Quick Scan (Basic port scan)
3. Intense Scan (Comprehensive analysis)
4. Custom Scan (Enter your own Nmap flags)
Select a scan level (1-4): 2

Running: nmap -T4 -F 192.168.240.1

Starting Nmap 7.94SVN ( https://nmap.org ) at 2025-01-23 15:12 MST
Nmap scan report for firewalla.lan (192.168.240.1)
Host is up (0.0041s latency).
Not shown: 98 closed tcp ports (conn-refused)
PORT   STATE    SERVICE
22/tcp filtered ssh
53/tcp open     domain

```



Here is the code. Dead simple. 
```python
import os

def nmap_scanner():
    print("Welcome to the Dead Simple Nmap Scanning Tool")
    
    # Prompt user for the target IP address
    target_ip = input("Enter the IP address you want to scan: ")
    
    # Display scan options
    print("\nScan Levels:")
    print("1. Ping Scan (Check if the host is up)")
    print("2. Quick Scan (Basic port scan)")
    print("3. Intense Scan (Comprehensive analysis)")
    print("4. Custom Scan (Enter your own Nmap flags)")
    
    # Get the user's scan choice
    scan_choice = input("Select a scan level (1-4): ")
    
    # Map choices to corresponding Nmap flags
    nmap_flags = {
        "1": "-sn",                  # Ping scan
        "2": "-T4 -F",               # Quick scan
        "3": "-T4 -A -v",            # Intense scan
    }
    
    # Determine the command to run
    if scan_choice in nmap_flags:
        flags = nmap_flags[scan_choice]
    elif scan_choice == "4":
        flags = input("Enter custom Nmap flags: ")
    else:
        print("Invalid choice. Exiting.")
        return

    # Build and execute the Nmap command
    nmap_command = f"nmap {flags} {target_ip}"
    print(f"\nRunning: {nmap_command}\n")
    os.system(nmap_command)

# Run the Nmap scanner
if __name__ == "__main__":
    nmap_scanner()

```