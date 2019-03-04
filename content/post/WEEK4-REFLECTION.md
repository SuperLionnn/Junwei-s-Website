---
title: "WEEK 4 REFLECTION"
date: 2019-03-02T22:08:48+11:00
draft: false
---

## WEEK 4
On Monday, a industry professional expert 'Ruben' that introduced us to the world of reverse engineering.
![0](WK4-RUBUN.PNG)
[Reverse Engineering and Binary Exploitation 0x00](http://uts-cs.securitygrounds.org/reverse-engineering/0x00/index.html)


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



# Deakin Oweek CTF
Portal: https://ctf.deakininfosec.com.au/challenges
These challenges are really friendly for those who are new to cyber security.
I solved half of them and here I will list the details about Reversing challenge - Unbreakable.

To accept the challenge, you need to download a .exe file which can easily open in Windows system. This application can be opened and pops up a box only let you to try the right password. 

I just did reversing to view the source code using Strings, ILSpy and Reflexil.for.ILSpy. 

Strings is the tool that provided by Microsoft 

**Introduction**
Working on NT and Win2K means that executables and object files will many times have embedded UNICODE strings that you cannot easily see with a standard ASCII strings or grep programs. So we decided to roll our own. Strings just scans the file you pass it for UNICODE (or ASCII) strings of a default length of 3 or more UNICODE (or ASCII) characters. Note that it works under Windows 95 as well.

It’s easy to use and Strings can scans the file to human readable UNICODE characters, and it shows all components of this application. 


![3](WK4-01.PNG)

I actually found the Password and the FLAG from here (when 2nd time I reviewed these strings). I think I found it without following this designer’s design but I just got it. Piece of cake :p
![4](WK4-02.PNG)

Reference/Credit: https://stackoverflow.com/a/80113


