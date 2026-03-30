# How to Write a Useful Bug Report

**Applies to:** RotU 2.2 and later

## Introduction

Please follow these guidelines when submitting a bug report. Doing so will help us understand and fix the issue much more quickly.

> **Important:**  
> Bug reports are **only** for problems with the source code, build system, wiki errors, or feature requests.  
> They are **not** for general discussion about RotU or for help setting up/modding a server.  
> Please use the Heavy Gunz forum for support questions.

## Bug Report Guidelines

1. **Version Information**  
   Tell us exactly which version of RotU you are running.  
   - Are you using a binary release? If so, which one?  
   - Did you compile from source? If so, which revision?  
   - Have you made any custom changes to the source code?

2. **Build Errors**  
   If you built the mod yourself, were there any errors during the build process? If yes, what were they?

3. **Operating System**  
   What version of Microsoft Windows are you running?

4. **CoD4 Version**  
   Are you running CoD4 1.6.x or 1.7.x?

5. **Reproducibility**  
   Is the bug reproducible? Can you make it happen on demand?  
   If yes, provide the exact steps required to reproduce the issue.

6. **Be Specific**  
   Avoid vague statements like “it doesn’t work”.  
   Clearly describe:
   - What you expected to happen
   - What actually happened
   - Any error messages you saw
   - What you see or don’t see on screen

7. **Log Files**  
   Attach the **relevant portion** of `console_mp.log` and `server_mp.log` that covers the incident.  
   Do **not** attach the entire log file.

8. **Map Information**  
   Which map were you playing when the bug occurred?  
   - Are you using the latest version of that map?  
   - Does the bug also occur on other maps?

9. **One Issue Per Report**  
   Please file only one issue per bug report.

10. **Check for Duplicates**  
    Don’t file a new report if someone else has already reported the same bug. Instead, add any additional information to the existing report.

11. **Language & Communication**  
    Can you read/write English? Can you speak/understand spoken English?  
    Do you have Skype? (Do **not** post your username in the bug report — we will contact you by email if needed.)

12. **Public Server Details**  
    If the bug occurs on a public server, please provide:
    - Server IP address and port (socket)
    - Your in-game name on that server

13. **Official Dev Server**  
    Does the bug also occur on the official development server?  
    `109.70.148.178:28937`

## Submitting Patches

If you have fixed a bug in your copy of the mod, you are welcome to submit a proposed fix.

Simply attach a **unified diff** (.diff or .patch file) to the bug report, and we will review it.

---

*Originally ported from the Google Code wiki.*