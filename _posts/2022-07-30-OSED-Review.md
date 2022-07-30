---
layout: post
title: 'Offensive Security OSED Review'
category: Binex
---

Around November I enrolled into Offensive Security's Windows User Mode Exploit Development(WUMED) or EXP-301 course to obtain the Offensive Security Exploit Developer(OSED) certification needed for the OSCE3 designation.  This post outlines my journey to OSED and my thoughts overall about the course from start to finish so the reader may decide if EXP-301 is right for them.

## Course Overview

  EXP-301 serves as one of the successors to the Cracking the Perimeter(CtP) course for the OSCE title and focuses on Windows x86 userland binary exploitation or 32 bit Windows 3rd party apps in layman's terms.  [The full syllabus can be found here.](https://www.offensive-security.com/exp301-osed)  I highly recommend the Learn One subscription for this course if the reader is new to binary exploitation as it took me around 6 months of study to adequately feel prepared for the exam but a 90 day option exists as well costing 1499$ and may be worth it if the reader has some binex experience.  At the time of writing this, the pdf is over 600 pages long and none of it is fluff or extra content.  All of the content is very concise and easy to understand and starts off as if the student has never performed a buffer overflow before and gradually adds the additional layers of complexity required to perform modern binex attacks. The videos are great quality as well and were essential to me understanding the content and following along.  I found myself watching them at 1.5x speed as there is some whitespace where the narrator will send the exploits and set necessary breakpoints in windbg before the next speaking sections. 


  If the reader has been out of the Offensive Security training loop for a while, it is worth noting that the courses are now within [their portal website](https://portal.offensive-security.com/) which provides a more graphical way to purchase courses and power on the required VMs to follow through the course.  This is the same platform that hosts their Proving Grounds cyber range and I recommend the reader get familiar with the web layout before enrolling in any courses as there can be a bit of a learning curve with navigating the website with things such as getting the VM credentials and managing VM instances.  It is no longer the webapp that was accessible once the VPN was connected.  The portal site it is pretty good and has a modern feel to it and I like the change to it vs the old method of access.  I found that it was easier to go through the material reading it on the website vs downloading the pdf and going through it on my local machine but that is a personal preference.

## Course Content and Exercises

The exercises consist of following along with the exploit creation process on each chapter and usually consist of a way for the student to improve on the exploit with their own research or to perform the same action again another way or on a separate application entirely.  I was able to perform all of the exercises within the course with the exception of the two monster extra miles.  The monster extra miles are a related set of optional exercises that can be performed and Offensive Security warns the student that they are incredibly difficult and time consuming.  The chapters and exercise progression feels very appropriate and concepts do a good job of building upon each other.  None of the extra miles or exercises feel unfair either and are very approachable.  I commend Offensive Security for changing to this mentality versus their old style of throwing students into the deep end immediately.  I felt the intro to reverse engineering chapter was a bit too steep of a learning curve and I would defer to a resource such as [Purplefox Vulnserver Writeup](https://www.purpl3f0xsecur1ty.tech/2021/05/26/trun_re.html) as a less steep introduction to IDA Pro + Windbg.  I also feel the course would benefit from a brief primer to x86 assembly but this can be supplemented by the student with a resource such as [SLAE from Pentester Academy.](https://www.pentesteracademy.com/course?id=3)  

## The Labs

  The labs consist of 3 applications the student must obtain a reverse shell on to consider them complete.  I found them to be very exam like and do a good job cementing the concepts of the course.  I never completed Challenge1 but was able to complete Challenge2 and Challenge3.  Challenge2 took a couple days with one sanity check whereas Challenge3 took me a month or so with several nudges.  I highly recommending joining [The Offensive Security Discord Server](https://discord.com/invite/offsec) and [Infosec Prep](https://discord.gg/infosecprep) for mentorship and nudges on the labs.  I met some of my best mentors on both and their help was worth their weight in gold.  Learn One subs are worth it if the student wants to 100% the labs.  I don't know if it is possible to go from 0% to 100% complete in the course in 90 days with no binex experience.  

## The EXAM

Offsec students should be notoriously tightlipped about the exams so I cannot reveal a ton of information.  [The Offensive Security OSED Exam Guide can be found here.](https://help.offensive-security.com/hc/en-us/articles/360052977212-OSED-Exam-Guide)  The exam consists of 3 challenges requiring a working PoC on 2 of them to pass.  Offsec requires step by step instructional writeups in the report to consider a pass within the report.  This means starting from whatever, if any, resource offsec gives you for the challenge, and explaining the PoC creation process until a reverse shell is obtained.  I didn't use any special templates for the report and used the [Offsec provided .docx file.](https://www.offensive-security.com/osed-online/OSED-Exam-Report.docx)  The exam is absolutely brutal and I had some of the worst luck during it.  My OSED exam experience is something that I will never forget as the "Try Harder" ethos rang true for me.  A timeline of my exam can be seen below of the 48 hours allotted to my exam.

Day 1
- 12pm: I start the exam feeling fresh.  The proctor couldn't see my ID so I used a copy on my computer.  A tip is to have a scan of a license saved on the computer ahead of time as a backup if the ID is bad.
- 1pm: Everything is going well.  I have a gameplan on how I want to attack the exam and have been going through the motions.  A construction crew shows up at my house and installs floors in my kitchen which is loud and distracting.
- 3pm: I am stuck.  I am not seeing a great way to move forward but thankfully the construction crew left.
- 5pm: I am unstuck and off to the races.  I take a break to eat dinner
- 6pm: I hit a snag I didn't expect and have to work through it but I am pretty much done with the first Challenge
- 8pm: It works in the debugger but not where I need it to.  After retracing my steps, I have to redo some work I did around 1pm to get it to work.
- 10pm: It works and I am halfway there.  I start taking screenshots of the process and have to go pick up a drunk friend from the bar.
- 12am: I go bunk with a friend so my 4 monitors and camera are destroying my eyes while I sleep.  I took 5 melatonin extra strength and basically just went on a trip in bed and slept maybe 3 hours tops.


Day 2:

- 6am: Wake up and grab taco bell.  Get home, shower, and drink some coffee for a bit.
- 8am: Get started with the exam again.  I read the requirements for the challenge again and write it out in OneNote so I have a clear path
- 9am: So far so good, everything is going along smoothly and I got around some curveballs pretty easily.
- 11am: I am super stuck; I am unsure why the thing I want to do isn't working and I want to bash my head against the wall.
- 1pm: My Internet goes out from a scheduled outage and I am stuck.  I do some editing offline and backup my files in case I need to move locations
- 2pm: A storm hits and my power goes out.  I am freaking the heck out.  Punching the walls, throwing my phone, yelling, etc.  It comes back on around 2:45 along with my internet so I calm down some.
- 4pm: I am unstuck and basically see how to get to the end of the assignment.  
- 7pm: I am 95% done with the second challenge and can finally see the light at the end of the tunnel.  Much like OSEP Review I celebrate with a cookie dough blizzard.
- 8pm: I start the report and begin writing up the first challenge.  I did not fix the second assignment yet.

Day 3:

- 1am: I am finished with the first section of the report.  It's really hitting me that I am tired now.
- 2am: I delete the second assignment PoC on accident and have to start it over from my last backup.  I am tired and angry.
- 4am: I fixed the exploit and got it to 100%.  I started writing that section of the report again.
- 6am: The report is done so I try and sleep so I can reread it when I am not dead tired.  At this point I am throwing up and shaking from being awake so long and completely wired on caffeine.
- 7am: A family member I like with starts acting like she's having a heart attack or stroke so I am woken up panicked and go back and forth on calling an ambulance while keeping an eye on them.
- 8am: Things have calmed down at this point and I go back to bed really scared.
- 11am: After a brief nap, I fix a ton of grammar on my report, reread the exam guide, and submit my exam at 11:45 just as my exam VPN was terminated.

It took about 2 days later that I met the requirements and became an Offensive Security Exploit Developer.  The knowledge from the course has given a new respect for binex folk and a clear path forward to polish up my reverse engineering and exploitation skills.  

## Shout-outs and extra resources

I wanted to take this space and thank ApexPredator, B0ats, and m33S33ks on discord for being amazing mentors during the course and that I appreciate their insight and desire to help the community. I would also like to give [epi](https://epi052.gitlab.io/notes-to-self/blog/2021-06-16-windows-usermode-exploit-development-review/) a shoutout for his [OSED scripts repo](https://github.com/epi052/osed-scripts) which made life a lot easier during the course.

Some extra resources I used during the course was the practice was [quote_db](https://github.com/bmdyy/quote_db) and [signatus](https://github.com/bmdyy/signatus) from [bmdyy.](https://williammoody.com/whoami)

## Conclusion:

EXP-301 was a gauntlet of fire that I am proud to say I have overcome.  The quality of the course is unmatched for an x86 exploitation course and is a worthy successor to Cracking the Perimeter.  I have no major complains about the course and am very happy with the quality of it.  I feel up to speed on modern Windows exploitation and am excited to continue my binex journey.  Thank you to Offensive Security for the course. 

Be sure to ping me in Infosec Prep or on Twitter if they need any more convincing as to why EXP-301 is an amazing Offsec training.  Hop to see everyone next post.