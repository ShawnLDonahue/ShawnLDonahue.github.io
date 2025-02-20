---
title: "How this site works and why! Now with Dark Mode!"
date: 2025-01-23 10:00
categories: [Hello Friend]
tags: [CI/CD, JEKYLL, GITHUB]
pin: False # Set to `true` if you want this post pinned to the top.
---

# Why host a blog in 2025 and on GitHub...
... which is apparently the most difficult way possible.

I was actually inspired by a former Google engineer. (Placeholder for her name when I can find it), had a brilliant use of GitHub - she showcased her resume using the same place where she hosts a great portfolio of projects. 

Now, I do have several of my own domain names and I blog on one of them as well but this portolio/project/blog, however, feels much more true to the source. 

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

How this site was made was an exercise in frustration. Plain and simple. I am pretty sure the people at OpenAI decided to give my chat instance a long vacation after yesterday. 

```bash
echo "How about you give the highlights and save the details for later?"
```

That's fair and to duplicate this entirely you would need the following:

```python
List_of_all_the_things = ("Ubuntu", "Git", "Snap", "Jekyll", "VS CODE", "GitHub Rep", "Caffeine", "Fine-Grained GITHUB permissions key", "ChatGPT", "YouTube", "Monumental Patience")
```
On the surface, it's straightforward, and to do it again, would take me maybe 15 minutes but here is the most distilled version. 

Breakdown of the list:

   * Ubuntu: The foundation of your workspace. Reliable, open-source, and just plain awesome.
   * Git: The version control system that gives structure to the chaos.
   * Snap: For those quick, efficient installations without the dependency drama.
   * Jekyll: The static site generator that's both your muse and your nemesis right now.
   * VS Code: Your coding sanctuary. Tabs, extensions, and linting to keep you sane.
   * GitHub Rep: Your online repository of hopes, dreams, and carefully curated markdown.
   * Caffeine: The actual energy driving all this work.
   * Fine-Grained GitHub Permissions Key: Unlocking GitHub’s secrets with precision.
   * ChatGPT: Your trusty sidekick, debugging assistant, and occasional cheerleader.
   * YouTube: Your crash-course university for tutorials, inspiration, and probably a few distractions.
   * Monumental Patience: The real MVP of this journey. You can’t download it, but you definitely need it.

I say "Ubuntu" but really I mean "linux" but this entirely possible on windows especially with native linux emulation. 

Distilled process:

   * Create a GitHub Account
    Start your journey by signing up for a GitHub account (if you don’t already have one). Then, fork or clone the Chirpy Starter repository. Name your repository <your-username>.github.io (e.g., shawnldonahue.github.io) to get that sweet GitHub Pages auto-hosting magic.

   * Set Up Fine-Grained Permissions
    Go to GitHub Developer Settings and create a fine-grained personal access token. Keep it handy-you’ll need it for connecting your tools later. (Pro tip: This is your key to the castle, so guard it well!)

   * HELLO CI/CD! Install Git
    Install Git on your local machine to manage pushing and pulling code from GitHub.
    Fun fact: VS Code comes with Git baked in, so technically, you can skip this if you prefer VS Code’s built-in tools. (But having Git directly installed is like keeping a Swiss Army knife in your pocket.)

   * Install Jekyll + Dependencies
    Get Jekyll running locally by installing Ruby, Bundler, and any other Jekyll dependencies. This is important for testing your blog before you push changes. Bonus: You can also build locally and see what your blog looks like offline! 🚀

   * Install VS Code
    Grab Visual Studio Code, your all-in-one text editor and development powerhouse. Extensions, themes, linting-it’s all here.

   * Connect VS Code to GitHub
    Set up Git integration in VS Code. Use your fine-grained permissions token to authenticate. Now you can clone, commit, push, pull, and live your best dev life-all from VS Code.

   * Customize Chirpy and Push Changes
    Open your repo in VS Code and start customizing Chirpy! Add posts, tweak settings in _config.yml, and make it your own. When you're happy, commit your changes and push them back to GitHub. 🚢

   * Test Locally Before Pushing (Optional but Worth It)
    Run bundle exec jekyll serve in your terminal to spin up a local development server. Open http://localhost:4000 in your browser to preview your blog.

   * Profit
    Okay, not literally, but your GitHub Pages site should now be live at https://<your-username>.github.io. 🎉

Bonus Steps (for Future-Proofing)

   * Install Node.js: Some Jekyll plugins and themes like Chirpy use Node.js for extra features.
   * Add GitHub Actions: Automate the deployment process for extra CI/CD awesomeness.
   * Learn Markdown: Posts in Jekyll are written in Markdown. Mastering it is key to crafting great content.


That's really it to get started. 

I took the scenic route to get there but only because it allowed me to test the site on my local machine before pushing public. 

Thanks and more to come! 

```python
print("Shawn L. Donahue")
```

