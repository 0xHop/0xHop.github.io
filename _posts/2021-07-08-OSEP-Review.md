---
layout: post
title: 'Offensive Security OSEP Review'
category: evasion
---

My AV Evasion posts seem to be popular so I wanted to take the time to review Offensive Security's 'Evasion Techniques and Breaching Defenses or Pen-300' course.

## Overview

Pen-300 serves as a continuation of the Pwk/OSCP course and picks up right where OSCP left off.  The course aims to cover 'evasion and breach techniques in greater depth and to prepare students for real-life field work' and the course excels at both.  [the full syllabus can be found here](https://www.offensive-security.com/pen300-osep).  The TL;DR version is, learn how to stage file transfer and write droppers in various formats, modify them to get around A/V, get them around other hardenning strategies such as Application Whitelisting and Network Filters, then move around until the network is fully compromised.  The PDF provided is approximately 750 pages long and is full of external reference to expand in any of the taught subjects.  At the time of writing this post, the course costs 1299$ for 60 days of lab time or 1499$ for 90 days of lab time.  I highly recommend the 90 day lab time.  I was finished with pdf and all labs on day 83.  

## The Exercises

The exercises have come a long way from the PwKv1 and CTP days.  The exercises move in a crawl, walk, then run approach where a concept will be introduced, It will be weaponized, and finally Offsec will give the student a twist to put their own style on it.  I agree with Offsec that there are no prerequisites required to jump into the exercises and content.  The exercises are enough to take the average OSCP to the next level. Each exercise was full of external references so there was always more to learn.  Usually at the end of the chapter, Offsec mentions some public toolbases that achieve similar functionality as the PoC written by the student.  I am very happy Offsec does this as it helps the student understand what is going on under the hood and encourage students to create their own tools.  I have seen a sharp increase in tools being published recently and its no surprise what training they all took.  I found a few exercises to be very confusing and had to do a few several times such as the early dropper development.  The videos were excellent for code review as the PDF does not always show the final code where the videos do.  While on the topic of the videos, they are clear and straight to the point.  Johnny Long does a great job voicing the videos again.  


The first few chapters focus on droppers such as metasploit's meterpreter payload and getting them passed Antivirus or "AV".  This is what I would call the "meat" of the course and where the best value is.  Each section of code is expertly explained and enough 3rd party links are provided to be familiar with the required code snippets.  The next sections focus on bypassing network filters and breaking out of Kiosks which were useful to know and really expanded on sandbox escapes and how to get the most out of the student's C2 server.  The final section involves lateral movement and more advanced attacks to pivot in the network and get to Domain/Enterprise Admin.  I had the most fun in the Active Directory and SQL Server trusts chapters by far. The course wraps up with a practice lab range to get a feel for how the labs would work. It took me around 35 days to get through the exercises and the 750 page PDF + videos.

## The Labs

Offensive Security provides 6 PRIVATE labs to practice what the student has learned.  Each lab has some similar servers experienced in the exercises but a few with the classic Offsec twist we all have come to know and ~~rage at~~ love.  This forced me into trying some new things that proved to pay off and learn the full capability of my selected C2 and built in Kali tools that weren't necessarily covered.  I required 12 nudges the entire lab range that my peers helped get me through.  Most were toward the first couple machines as it gets easier to figure out what needs done when three quarters of the network is already compromised.  My preference goes from most favorite to least favorite as shown below.  Labs 1-3 are very small and get the student comfortable while 4-6 grow in size and let the student play around and truly pivot between child domains and networks.  Please be sure to join the Offsec discord or [Infosec Prep](discord.gg/infosecprep) if you need any nudges yourself.  The labs are very fair and do not through excessive CTP curveballs and do a wonderful job preparing for the exam.

Lab 5 -> Lab6 -> Lab2 -> Lab1 -> lab3 -> Lab4.  Screw you lab4.  

## The EXAM

Offsec students should be notoriously tightlipped about the exams so I cannot reveal a ton of information.  I will say that the if you can finish all the labs and claim all of the flags, the exam will be smooth sailing.  There are no specific chapters to mention as all the chapters cover important stages of a pentest.  If I had to describe the exam, I would call it "tough but fair like a military step parent".  I did not feel like at any point I was unfairly stuck or lost in the exam.  The exam is 47 hours and 45 minutes long with an additional 24 hours alloted for reporting.  This is more than enough time in my opinion and very doable.  The only tool restriction on the exam is no commercial tools AKA nothing that normally costs money for example Burpsuite Pro or Cobalt Strike.  There are multiple paths to success.  A student needs 10 flags or to obtain the "secret.txt" flags and a report for a pass.  My timeline went as follows:

Day 1
- 10am: Start exam after joining and performing proctor actions.
- 10:30am:  Got my 1st flag
- 12pm: got stuck and change strategies and it works.  2nd flag obtained
- 1pm: 3rd flag obtained  
- 3pm: finish up some environment enumeration and get my 4th flag while I was at it.
- 4pm: Got two more flags and I am feeling great.
- 5pm: break for dinner.  I see what I have to do just haven't done it yet.  Gotta consult pdf.
- 6pm: Saw I got a missed call from a job opportunity.  Call them back.
- 7pm: 8 flags down.  I finally feel like I am going to pass.
- 9pm: 9 flags in.  I am so close I can taste it.
- 11pm: Why isn't anything working A*3000.
- 12am: Go to bed.  Decide to write my report while I think what to do.

Day 2:

- 6am: wake up and shower/make breakfast
- 8am: Start writing the report
- 9am: Get a call from job.  I had landed my first Red Team job.  
- 10am:  The things I was doing yesterday aren't working wtf.
- 5pm: Report is finished.  All i got to do is eat dinner and figure out this last flag.
- 6pm: Still nothing.  At this point I am ready to cry.  All of that work for nothing.
- 7:30pm:  I took a shower and had several ideas of things to try.
- 8:30pm:  secret.txt in the bag.  I step out for some dairy queen for celebration.  I got a large cookie dough blizard.
- 11pm: Report ready.  Decide to sleep on it a day and proof read one more time before I turn it in.

Day 3:

- 6am: Wake up and make breakfast
- 8am: Report submitted.

I found out 2 days later that I met the requirements and became an Offensive Security Experienced Penetration Tester.  The knowledge I gained from the course was more than enough to clear me a Red Team role and I hadn't even gotten the title yet.  I was sure to tell the proctor and pass on to the Offsec Content Devs that I appreciated all the work they put into the course. 

## Conclusion:

PEN-300 was the best IT training I had ever received.  Not only did it get me my first red team role, it gave me the confidence I needed to feel comfortable calling myself a pentester.  I strongly believe anyone who passed PwK and earns the OSCP should go straight into PEN-300 to take their skills to the next level.  I recently did an Ask Me Anything in Infosec Prep and I will update this post when the recording is up for anyone would like to listen in.  

Be sure to ping me in Infosec Prep or on Twitter if they need any more convincing as to why PEN-300 is the next level Offsec training.  Hop to see everyone next post.