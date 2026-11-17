# Week 3: Password Cracking (John the Ripper & Networkwalks Tools)

Networkwalks Cybersecurity Internship, Batch B084. Author: Michelle Kibichii.

## Overview
This project cracks the password of a locked PDF file using two different methods, to compare a local command-line tool against a browser-based tool.

## Modules completed
| Module | Tool | Result |
|---|---|---|
| W3-PM1 | John the Ripper + Johnny (GUI), with `pdf2john.pl` to extract the hash | Password: `password1` |
| W3-PM2 | Networkwalks Hash Calculator + Password Cracker (browser-based, no install) | Password: `password1` |

## Key finding
Both methods extracted the **exact same hash** from the PDF and both cracked it to the **same password**, `password1` — confirming the extraction and cracking process is correct either way. The password was weak enough to be found almost instantly in a small built-in wordlist, which is the core lesson: short, common, dictionary-style passwords offer almost no real protection.

## Evidence
![Hash extracted with pdf2john](screenshots/pm1/pm1-01-hash-extracted.png)
![Hash loaded in Johnny](screenshots/pm1/pm1-02-hash-loaded.png)
![Cracked in Johnny](screenshots/pm1/pm1-03-cracked.png)
![Flag captured](screenshots/pm1/pm1-04-flag-captured.png)
![Hash Calculator](screenshots/pm2/pm2-01-hash-calculator.png)
![Password Cracker result](screenshots/pm2/pm2-03-cracked.png)

## Folder guide
- `screenshots/pm1/`: evidence for the John the Ripper + Johnny module
- `screenshots/pm2/`: evidence for the Networkwalks browser-tools module
- `evidence-text/`: the extracted hash file (`hash.txt`)

## Ethical use
This file was provided for the course's own practice lab. Only crack passwords on files and systems you own or have written permission to test.
