# Reign of the Undead

This project is the "Reign of the Undead" CoD4 Mod.  It is *not* compatible with ROTU-Revolution.  
I am importing it from the archived Google Code Subversion repo, which is really just a working copy on steroids, and augmenting it with my local original files.  Note that *all* of the version control information was lost when Google Code shut down.  I have the original repo up to rev 87, before I moved to Google Code, but I can't see how that would be helpful.

Do NOT fork/clone it yet, as things will change wildly as I port this to github, the best I can. I'm making breaking changes to the build system, but I have successfully gotten CoD4 installed and patched on Linux, and also got the entire RotU mod compiled on Linux. I'll update this message when it is safe to tinker.

 - [Installing CoD4 on Kubuntu 25.10](wiki/InstallingCoD4Kubuntu25.10.md)
 - [Setting Up a Development Environment](wiki/DevelopmentEnvironment.md)

## Description

RotU was originally written by Bipo (bipolarmonk) for the 1.x series.  Bipo then stopped development, open-sourced his code, and then I wrote the 2.2.x series.  ROTU-Revolution was independently created by others from Bipo's original code (I started working months earlier, but they made a public annoucement of their intention while I was still hacking in private).  So, they are two separate mods; any code or resources that work together is coincidence.

## Getting Started

Cloning the repository will *not* get you working code, suitable for playing or hosting a server.  There are many in-work changes in master that aren't ready for release.  If you want to play, download 2.2.2 and then 2.2.1-Patch1.

To get a copy of the project running locally:

1. Clone the repository:
```bash
git clone https://github.com/marktaff/reign-of-the-undead.git