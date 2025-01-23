---
title: "How this site works and why (..I even bothered)"
date: 2025-01-23 06:52
categories: [Hello Friend]
tags: [CI/CD, JEKYLL, GITHUB]
pin: True # Set to `true` if you want this post pinned to the top.
---

# So! Why host a blog in 2025 and on GitHub...
... which is apparently the most difficult way possible.

I was actually inspired by a former Google engineer. (Placeholder for her name when I can find it), had a brilliant use of GitHub - she showcased her work using the same place where she hosts a great portfolio of projects. 

I have several of my own domain names and I blog on one of them as well but this felt more connected than ever to my work. 

This portolio blog, however, feels much more true to the source. 

```bash
echo "Pfft. Purist snob!"
```
### Moving on
As a cybersecurity professional, it's not exactly easy to get your hands into every aspect of the business. Some companies will seek to silo your skillset to a couple of the usual (GRC, Operations, DevSec, Vulnerability Management, Threat Hunting, Pentesting, etc.) and I oftentimes find myself stuck somewhere between Operations, GRC, and Vulnerability Management. 

But little in the way of scripting for automation, or project work with any sort of value worth publishing, CI/CD, DevOps, and so on.

```bash
echo "Oh you mean the things that employers actually need and add value to your resume?"
```
Yeah, those things.

### That brings me to the how, and yeah, likely some more why. 

How this site was made was an exercise in frustration. Plain and simple. I am pretty sure the people at OPenAI decided to give my Chat instance a long vacation after yesterday. 

```bash
echo "How about you give the highlights and save the details for later?"
```

That's fair and to duplicate this entirely you would need the following:

```python
List_of_all_the_things = ("Ubuntu", "Git", "Snap", "Jekyll", "VS CODE", "GitHub Rep", "Caffeine", "Fine-Grained GITHUB permissions key", "ChatGPT", "YouTube", "Monumental Patience")
```
On the surface, it's straightforward, and to do it again, would take me maybe 15 minutes but here is the most distilled version. 

I say "Ubuntu" but really I mean "linux" but this entirely possible on windows especially with native linux emulation. 

Distilled process:

* Create a GitHub account and then clone the JEKYLL chirpy-starter to a repository in your github account using your username.github.io as the repo nam.
* In GitHUb Developer settings create a fine-grained permission key for later
* HELLO CI/CD! Install GIT on your local machine to allow you to push and pull from github (vs code does this as well and git might be skipped..sorta.. nvm)
* Install JEKYLL and all dependencies on your local machine. (this is for testing and other bits) 
* Install VS Code
* Connect VS Code to your repository (permissions ahoy!)
* Edit in VS Code and push back

That's really it to get started. 

I took the scenic route to get there but only because it allowed me to test the site on my local machine before pushing public. 

Thanks and more to come! 
Shawn L. Donahue

