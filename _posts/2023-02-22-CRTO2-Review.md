---
layout: post
title: 'Zero Point Security CRTO 2 Review'
category: Review
---

I Liked the CRTO 1 course enough to volunteer for more red team operations at work which gave me a good reason to enroll in the second Red Team Operations course.  This post will contain my opinions and experiences on the course overall and whether or not the reader would like to enroll in the course.

## Course Overview

Red Team Ops 2 is the latter of two Red Team Ops courses created by [RastaMouse](https://rastamouse.me/)  continuing to cover covert adversary simulation engagements while evading and bypassing hardened systems.  In layman's terms, how to be an APT on an internal network and evade a blue team focusing heavily on [Cobalt Strike](https://www.cobaltstrike.com/).  The full syllabus can be found [here](https://training.zeropointsecurity.co.uk/courses/red-team-ops-ii).  The course opens immediately with more advanced infrastructure setup with redirectors and optimizing Cobalt Strike installation.  Redirectors were a bit mystic to me before this so seeing how to build one from scratch was a great experience as opposed to the automated redirector generators.  The course jumps into custom payload development after this for better shellcode runners by explaining the Windows API and how to build several Shellcode runners.  The code is very clearly written and easy to understand and I felt it did a better job than [OSEP](https://www.offensive-security.com/pen300-osep) for the c#/c++ droppers.  Next, the course covers common defense evasions which turns a jr red teamer into an intermediate red teamer.  Rastamouse did a great job of showing code examples of how techniques such as PPID Spoofing and ACG blocks work in custom code before mentioning that Cobalt Strike had the functionality built in to fork & run style commands.  These sections feel like natural transition to the following evasion style sections.  These begin with Attack Surface Reduction(ASR) which covers the strengths and weaknesses of Windows built in defenses and how to bypass the rules.  I will note here that myself and several of the other students I talked to in the [Zero Point Security Discord Server](https://discord.com/invite/Whz3YtY4gG) had issues getting one of the exercises to work properly in and out of the lab machines so be wary and give the server a join.  Windows Defender App Control(WDAC) is next as a fantastic Applocker replacement.  I didn't realize how effective WDAC was at preventing initial malware execution.  The course covers how to abuse several rules within WDAC policy to get initial execution.  Any bypasses outside of a misconfigured rule are CVE worthy which make bypasses tricky but technically possible.  The course ends on EDR Evasion and includes a pseudo EDR driver developed in the [Offensive Driver Course](https://training.zeropointsecurity.co.uk/courses/offensive-driver-development) to test payloads against.  I personally felt this was the most valuable and most underwhelming part of the course at the same time.  For a red teamer who is not versed in payload development, this section is invaluable in modern red teaming as most companies have a form of EDR installed on a large number of endpoints.  The techniques shown in the section however have been around a bit and are beginning to get signatured by EDR and AV more frequently.  The EDR theory and anatomy were excellent and well explained.  My favorite section included the syscalls and ArtifactKit integrations which I have already began to implement into my red team payloads.

I felt the quality of the course was very good.  Some sections have videos with walkthroughs and completed code and others don't.  Everything is explained very clearly and isn't ambiguous at all.  I feel very strongly when I say those who enroll in this course should complete [CRTO1](https://training.zeropointsecurity.co.uk/courses/red-team-ops) or [OSEP](https://www.offensive-security.com/pen300-osep) first as CRTO2 assumes some knowledge such as Active Directory exploits and other general infosec knowledge.  I wish the course included blue team detections like CRTO 1 as a red team aspect is very focused unlike CRTO1 which felt almost Purple team to me to make it valuable for blue teamers as well.  

There was a recent change with the RTO labs where the lab time is no longer lifetime access and will expire after several months so schedule your time accordingly.


## Course Update Wishlist

  ZeroPoint Security does a great job of continously updating their course content and including the updates free of charge to owners of the course.  The course itself feels full but there are a few things I feel wish was included in the content.

  * Red Team Infrastructure automation tooling creation such as [RedCloud](https://github.com/khast3x/Redcloud).
  * More Arsenal Kit modifications with aspects such as the mimikatz and process injection.
  * Custom User Defined Reflective Loader creation similar to [BokuLoader](https://github.com/boku7/BokuLoader).

## The Exam

The exam gets scheduled through Snap Labs as an event and can be scheduled on the red team ops exam page.  Students have 72 hours of powered on exam infrastructure or 5 complete days, whatever comes first.  A passing score is 4/4 flags at the time of writing this.  The course content covers the majority of what the student needs to pass but some extra research is required.  I passed within 12 hours of screen time with the first 7 being the first flag.  The 72 hours is plenty of time and if anything,  a tad overkill.  Completing the exam awards the student the Certified Red Team Lead(CRTL) certification.




## Extra Resources

I found the following guides helpful when going through the labs and recommend taking a look at them.

* [Harmjoy cheatsheets](https://github.com/HarmJ0y/CheatSheets)

* [Cobalt Strike User Guide](https://hstechdocs.helpsystems.com/manuals/cobaltstrike/current/userguide/content/topics/welcome_main.htm)

* [Rubeus Guide](https://github.com/GhostPack/Rubeus)

* [Cobalt Strike Cheatsheets](https://github.com/S1ckB0y1337/Cobalt-Strike-CheatSheet)


## Conclusion:

 ZeroPoint Security made another fantastic course that seamlessly continues where the first RTO1 course ended.  Anyone who already has CRTO should jump right into the course and get started.  I had a fantastic time going through the material.  I hope this post was helpful for anyone on the fence about enrolling in the course.