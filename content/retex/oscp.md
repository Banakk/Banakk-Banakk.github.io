---
title: "OSCP+"
date: 2025-02-24
draft: true
---

### Introduction
<br><br>

Hello everyone 👋👋, on February 21st, 2025, I passed the OSCP+ certification after two attempts. My first attempt was before OSCP+, and I'm not sure how much time I spent preparing for this certification because I took many breaks between each attempt. However, today I want to write this "retex" because OSCP+ is a new format, and there are not many "retex" available for it. I know that for anxious people, it can be important to anticipate all scenarios before the exam day.


### Quick remember about new format OSCP+.

Detailled new format can be found : [OSCP OFFICIAL GUIDE](https://help.offsec.com/hc/en-us/articles/29865898402836-OSCP-Exam-Changes).

#### What are the changes to exam format?

The OSCP exam format change provides learners with the ability to work through an “assumed compromise” where learners start with a standard user account on the Activity Directory (AD) domain with the goal of full domain compromise. OffSec will allow learners to earn partial points within the AD domain removing the requirement to fully clear the AD exam set to receive any AD exam related points. Bonus points will no longer be awarded.

In particular:

    For the Active Directory exam set, learners will be provided with a username and password, simulating a breach scenario;
    Learners may then accumulate points for machines 1, 2 and 3 of the Active Directory exam set - 40 points in total
        10 points for machine #1
        10 points for machine #2
        20 points for machine #3;
    Removal of 10 bonus points.

#### How will points be allocated / distributed?

OSCP exam points will be allocated as follows:

    3 stand-alone machines (60 points in total)
        20 points per machine
            10 points for initial access
            10 points for privilege escalation
    1 Active Directory (AD) set containing 3 machines (40 points in total)
        10 points for machine #1
        10 points for machine #2
        20 points for machine #3
    Possible scenarios to pass the exam (70/100 to pass)
        40 points AD + 3 local.txt flags (70 points)
        40 points AD + 2 local.txt flags + 1 proof.txt flag (70 points)
        20 points AD + 3 local.txt flags + 2 proof.txt flag (70 points)
        10 points AD + 3 fully completed stand-alone machines (70 points)

### Background

I start since 2023 to focus cybersecurity with many challenges in [root-me](https://www.root-me.org/) platforme and switch on Hackthebox to reinforce my methodology.

### Exam Day

- 11:00 PM: Start
- 1:00 AM: Standalone 1 - Local.txt + 10 PTS
- 2:00 AM: Active Directory - First machine proof.txt + 10 PTS
- 4:00 AM: Fully stuck, I go to sleep
- 9:00 AM: Wake up
- 10:00 AM: Standalone 1 - Root.txt + 10 PTS
- 12:00 PM: Standalone 2 - Local.txt + 10 PTS
- 1:00 PM: Standalone 2 - Root.txt + 10 PTS
- 3:00 PM: Active Directory - Domain Controller proof.txt - 20 PTS
- 4:00 PM: Active Directory - Second machine proof.txt - 10 PTS

<br>
<br>

Now I know I have all the points needed to validate the exam, so I took one more hour to try the last standalone machine, but I stayed stuck. Therefore, I chose to give up the last standalone machine and I repeated each machines, taking screenshots for the report.
<br>

Don't stress about a report , if you take screenshot or good doc with your process during exam it could be good.

###  My advices

A short list of things that helped me during the exam day:

- Keep it simple! If at any point you find an exploit that is too difficult and requires a deep understanding of concepts, it's probably the wrong approach.
- Don't place all your trust in tools. OSCP+ wants to check if each student has a good understanding of basic pentesting, and it's not for script kiddies. Obviously, run tools like linpeas/winpeas, but also know how to manually check the machine.
- For each exploit, my advice is to know at least two tools to confirm whether it's the right or wrong approach. For example, if you want to check the RPC protocol, you can use rpcclient and nxc with the --rid-brute option.
- Check, check, check, and CHECK AGAIN: default credentials, weak credentials, and keep it all in files like user.txt and pass.txt.
- Ensure you understand the concept of pivoting. I recommend ligolo-ng; it's pretty simple to deploy.
- Obviously, you need to train with boxes like HTB and PG, but in my opinion, the main component of your success in the exam is understanding what you're doing. If you know what you're searching for and why, you will literally win the exam. Additionally, having a good methodology is key.
- For Active Directory, ensure you know how to use key tools like BloodHound, Impacket, BloodyAD, etc.


### Result

![](/images/oscp.png)

### What next ?

Now, my new challenge is cloud and systems hardening. Before I end my student life, I want to pass the Kubernetes certifications (CKA, CKS) and the AWS certification (AWS Certified Solutions Architect – Associate).
<br>

Thank you for reading my retex,  you can contact me if you want . See you later 😎😎