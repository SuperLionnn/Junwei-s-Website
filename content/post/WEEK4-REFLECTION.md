---
title: "WEEK 4 REFLECTION"
date: 2019-03-02T22:08:48+11:00
draft: false
---

## WEEK 4
On Monday, a industry professional expert 'Ruben' that introduced us to the world of reverse engineering.
![0](WK4-RUBUN.PNG)
[Reverse Engineering and Binary Exploitation 0x00]()


Reverse Engineering

Reverse Engineering is the skill of figuring out what a black box is doing. This includes being able to figure out what a set of assembly instructions means. This doesn’t mean you have to understand every single instruction. With enough practice you’ll start recognising structures pretty quickly.<br>
![1](WK4-stack-heap.png)<br>

Some common instructions are:<br>
<br>
je: Jump to an address if its equal to something. If unequal, continue with the flow.<br>
jmp: Perform a jump to an address.<br>
call: Jump to a new function while also pushing the current EIP/RIP value to the stack.<br>
cmp: compare two values with each other.<br>
lea: Load effecive address: load a pointer into a register<br>
mov: Move the value (at the pointer) into a register<br>

---
The most important part for reverse project is to looking for data flow and logic control. There are also many data that been encoded. Sometimes we need to recognise and decode them. 
![2](WK4-RE.PNG)

(I did not really understand what is going on here, so I just make it generally. Is that human-readable?)
<br>
<br>
<br>
# Deakin Oweek CTF
Portal: https://ctf.deakininfosec.com.au/challenges
These challenges are really friendly for those who are new to cyber security.<br>

I solved half of them and here I will list the details about Reversing challenge - Unbreakable.<br>

To accept the challenge, you need to download a .exe file which can easily open in Windows system. This application can be opened and pops up a box only let you to try the right password. <br>

I just did reversing to view the source code using Strings, ILSpy and Reflexil.for.ILSpy. <br>

Strings is the tool that provided by Microsoft <br>

**Introduction**<br><br>
Working on NT and Win2K means that executables and object files will many times have embedded UNICODE strings that you cannot easily see with a standard ASCII strings or grep programs. So we decided to roll our own. Strings just scans the file you pass it for UNICODE (or ASCII) strings of a default length of 3 or more UNICODE (or ASCII) characters. Note that it works under Windows 95 as well.<br>
<br>
It’s easy to use and Strings can scans the file to human readable UNICODE characters, and it shows all components of this application. 


![3](WK4-01.PNG)

I actually found the Password and the FLAG from here (when 2nd time I reviewed these strings). I think I found it without following this designer’s design but I just got it. Piece of cake :p<br>
![4](WK4-02.PNG)

At the end, here is my Rank score.
![4](WK4-DK-RANK.PNG)

Through these Oweek challenges, I found it is easy for me (after 3 weeks cyber security study). Simple question I knew how to do so that I found a few flags immediately. That felt so cool!<br>


<br>

## EXPO !

Friday was a big day! The whole summer studio stay together and enjoyed free pizza! Also, it was the time we show our final artifects to other fields students. After talking a while, I found that everyone think cyber security is pretty cool and full of challenges. I showed a little to my friends about how to get Invite Code from HackTheBox. He was fully attracted like he was watching a magic show by the pentesting and encode/decode staff.
To be honest, there are more students who did summer studio from other fields, expect to joined Cyber Security if there is another chance to choose.


![4](WK4-EXP-WARP.png)

Took a selfie with Crist :p
![4](WK4-EXP-CRIS.png)

Jason was focused on his fantastic presentation.
![4](WK4-JASON.png)

I also visited to Real-World Nerual Network team. One team did one recognition system that it can label every human images in the video. And shared me a open course video link to study NN from the beginning.<br>
https://www.lynda.com/Keras-tutorials/Neural-Networks-Convolutional-Neural-Networks-Essential-Training/689777-2.html?org=uts.edu.au
<br>
<br>
In conclusion, week 4 everyone was engaged and excited. At the end of 2019 summer seesion, I feel great and be powered by all other guys in the studio. And I still need do more research to get one box for the final report. 

Reference: 
<https://stackoverflow.com/a/80113>
<http://uts-cs.securitygrounds.org/reverse-engineering/0x00/index.html>

