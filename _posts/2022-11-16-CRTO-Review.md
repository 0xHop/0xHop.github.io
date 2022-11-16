---
layout: post
title: 'Zero Point Security CRTO 1 Review'
category: Review
---

I recently changed organizations and had the privilege for them to offer me the [Zero Point Security Red Team Ops Course](https://training.zeropointsecurity.co.uk/courses/red-team-ops).  I am a huge fan of the Zero Point Security courses having recently also done the [C2 Development in C#](https://training.zeropointsecurity.co.uk/courses/c2-development-in-csharp) and the [Offensive Driver Development](https://training.zeropointsecurity.co.uk/courses/offensive-driver-development) as well.  I wanted to give my thoughts again on the course so the reader understands how the course operates and what to expect.  Let's Hop in.

## Course Overview

Red Team Ops 1 is the first of two Red Team Ops courses created by [RastaMouse](https://rastamouse.me/) covering covert adversary simulation engagements.  In layman's terms, how to be an APT on an internal network and evade a blue team focusing heavily on [Cobalt Strike](https://www.cobaltstrike.com/).  The full syllabus can be found [here](https://training.zeropointsecurity.co.uk/courses/red-team-ops).  At the time of writing this, the course is on version 2.0.2.  The course begins with some Red Team definitions and explains setting up Cobalt Strike.  The course begin goes through a typical engagement of recon, getting a foothold, escalating privileges, and moving laterally throughout a Microsoft Active Directory network.  

I felt the quality of the course was very good.  Some sections have videos with walkthroughs and others don't.  Everything is explained very clearly and isn't ambiguous at all.  That isn't to say the course isn't for absolute beginners.  Anyone with an [OSCP](https://www.offensive-security.com/pwk-oscp/) is ready and anyone with an [OSEP](https://www.offensive-security.com/pen300-osep/) will fly through the course.  This isn't to say those with an OSEP won't benefit as the Cobalt Strike knowledge and OPSEC notes are incredibly valuable.  Throughout the course there is a SIEM logging on all of the lab machines and the course teaches the student how to threat hunt for themselves while performing attacks.  I thought this was brilliant as it makes the course valuable to blue teams as well and makes for a stronger red team by allowing the student to experiment and bypass the SIEM detections.  


## The Labs

  The labs are hosted in [Snap Labs](https://www.snaplabs.io) as virtual machines that can be stopped/started on demand by the student in a browser.  When registering for the course, the student can optionally get access to the lab.  I strongly recommend doing so as the hands on aspect of the course are excellent.  Students will get 40 hours of lab time when registering and the hours only count when the virtual machines are powered on. I felt like 40 hours was more than enough as I only used approximately 10 hours throughout the course and extra miles that I made for myself.  Below are some additional exercises that I did to help myself learn Cobalt Strike:

  - Made several Beacon Object Files
  - Created an artifact kit that used a method form [Alternative Shellcode Exec](https://github.com/aahmad097/AlternativeShellcodeExec) to load Shellcode instead of CreateThread.
  - Create a custom .cna file and exam.profile

## The Exam

The exam gets scheduled through Snap Labs as an event and can be scheduled on [this](https://training.zeropointsecurity.co.uk/pages/red-team-ops-exam) page.  This section on the bottom of the page is not a png and actually how you schedule the exam which admittedly tripped me up.

<img src="https://0xhop.github.io/images/CRTO/Register.PNG">

The exam consists of an environment similar to the labs where a student is expected to collect labs on Administrator Desktops throughout a network.  6/8 flags are required for a passing score.  48 hours of the VMs powering on or a full four (4) days are the allotted time limits for the exam.  So, if an exam is scheduled on noon Friday, it will last 48 hours of the environment being powered on or until Tuesday at noon.  The exam can be powered off for extended breaks such as sleep which is amazing.  I wish other certification providers did this as well as it's the only time in my professional career I didn't feel like I was being punished for sleeping for 9 hours.  The exam is very straightforward and I was never in a position where I didn't know what to do.  Not to say it was easy, just straightforward.  

That being said the environment has the potential to be very unstable, things that worked in the labs didn't work for me, reverts sometimes fixed issues and sometimes they caused more, sometimes boxes wouldn't come back up after I would do a start/stop, etc.  This is more a complaint at Snap Labs than it is Zero Point Security and just the nature of the beast.  Fighting the bugs and stability was 3/4 the battle of the exam.  Flags get uploaded in the exam webpage and a report is not required for pass, just upload the flag hash and call it a day.  A pass or fail email will be received after the exam lab expires.  It took around 20 minutes for me to get my pass email after it was over.


## Extra Resources

I found the following guides helpful when going through the labs and recommend taking a look at them.

* [Harmjoy cheatsheets](https://github.com/HarmJ0y/CheatSheets)

* [PowerUpSQL Cheat sheet](https://github.com/NetSPI/PowerUpSQL/wiki/PowerUpSQL-Cheat-Sheet)

* [Rubeus Guide](https://github.com/GhostPack/Rubeus)

* [Cobalt Strike Cheatsheets](https://github.com/S1ckB0y1337/Cobalt-Strike-CheatSheet)


## Conclusion:

 Zero Point Security Red Team Ops was an amazing experience to go through.  The quality of the course is fantastic and very valuable for both red and blue teams alike.  I feel more comfortable than ever with Cobalt Strike and understand the buzz about it now as well.  I can't think of a better value certification than CRTO and fully recommend it to any information security professional.  Feel free to ping me if there are any questions about CRTO or if any more testimonial is needed. I look forward to doing CRTO 2 in the future.