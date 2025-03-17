---
title: "CIP Happens: A prattle about NERC, FERC, and the abundance of standards."
date: 2025-03-16 17:00
categories: [Prattle]
tags: [Critical Infrastructure]
pin: false # Set to `true` if you want this post pinned to the top.
image:
  path: /assets/img/NERC.png
  alt: Preview image
---

### I find more and more of my writings are prattles than projects these days.

For reasons I will keep to myself unless otherwise necessary - I found myself navigating the CIP menu on the NERC website:
https://www.nerc.com/pa/Stand/Pages/ReliabilityStandards.aspx

As I stared into the abyss, I decided to read more into CIP 11-3 which is title	"Cyber Security — Information Protection": <br>
https://www.nerc.com/pa/Stand/Reliability%20Standards/CIP-011-3.pdf

Almost immediately, I discovered that I might have jumped ahead. Much of the classification of systems comes from another CIP, 2-5.1a:<br>
https://www.nerc.com/pa/Stand/Reliability%20Standards/CIP-002-5.1a.pdf

Which (heavily) discusses cyber systems referred to as "BES" -

And per our LLM pal:<br>
"BES Cyber Systems (Bulk Electric System Cyber Systems) and their associated BES Cyber Assets are key components in the context of cyber security for the energy sector, specifically for the protection of critical infrastructure in the electric grid. These terms are defined by the North American Electric Reliability Corporation (NERC) as part of their Critical Infrastructure Protection (CIP) standards."

```bash
A few moments later
```

Admittedly, I am immediately jealous. 

One of the nice things about the NERC CIPs is that, by way of industry-sourcing knowledge, they fundamentally remove some of the guesswork when it comes to the criticality rating of some assets. A task that can sometimes be cumbersome and time-consuming in security.

Also, it's a standard and not a framework. 
It's expected, not optional. 

I also appreciate these standards are not long-winded. Comparing the 500+ page NIST frameworks to a dozen or so of these CIPs - declares a clear winner in the streamlined category.

One of the fun moments when working in cybersecurity is when you discover there is absolutely no shortage of frameworks or standards. 

### In many ways, most modern frameworks all sort of blend together in an blanket of catch-all, grey security. But standards like the NERC CIP really make you appreciate when an industry gets together and removes much of the room for error.

However, nothing is perfect. 

For example, NERC CIPs do not allow for the use of Cloud services as discussed in the article:<br> 
https://www.industrialdefender.com/blog/nerc-cip-and-the-cloud-tom-alrich

some more, slightly older, reading on the topic:
https://learn.microsoft.com/en-us/azure/azure-government/documentation-government-overview-nerc

It's worth noting that Microsoft themselves washes their hands of CIP responsibility on the same page:
<br>"Customers operating the Bulk Electric System (BES) are wholly responsible for ensuring their own compliance with NERC CIP standards. Neither Azure nor Azure Government constitutes a Bulk Electric System (BES) or BES Cyber Asset."

With that, I have a lot more reading to cover and skeletons to dig up. 

I have quite a bit of IAM technologies to cover along with Application Development security and might not touch on CIPs for a bit. 

```python
print("Shawn L. Donahue")
```
