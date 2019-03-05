---
title: "Portfolio"
date: 2019-03-04T10:00:48+11:00
draft: false
---

# Portfolio

### Introduction
My name is Junwei Liang, a 3rd year student in Bachelor of Engineering (Software Engineering). I am so lucky that I enrolled in the summer studio. In Cyber Security studio, all colleagues are friendly and energetic. Because of I was almost start from zero in Cyber Security, and everyone in the studio helped me a lot on both communication and technical problem solving. So that, I would like to recommend that the Cyber Security summer studio is definitely one of the worthiest elective subjects in UTS. <br>

* * All brilliant staff and students who are interested in the same field with creative design thinking which apply the subject objective in real-world task. 

* * The studio welcomes all students who are interested in cybersecurity whatever you are a noob or expert. That means the assessment requirements based on your personal technical skills. Students just followed learning objectives and writing reflection every week. Abundant resources from beginner level to hell level.
<br>
For more information, please forward to  [WEEK1-4 REFLECTION](https://www.blank1024.me/post/week1-reflection/)  to find out something really cool staff in cyber security studio. This portfolio mainly discusses the summaries of the personal experience in this studio.<br>

### Conclusion
At the beginning of journey, I thought that I could be a pentester or internetworking engineering in Cyber Security industry, but I got no idea about offensive security and how attack happens and never stop in real world. The only thing I known is from subject Security Fundamental – mainly about high-level security properties and data encryption (hashing). However, in cyber world, that like a metal cog is part of a factory and do not engage or thought-provoking practice in real-world. For 4 weeks busy weeks study, I found a new cyber world that I never known before. There are so many vulnerable layers (data packet in network traffic, website penetration, physical) and unbelievable ways of attack. Gradually, I realized that not everyone could work in security industry because it definitely requires abundant and multi-fields technical knowledge with creative design thinking. I learnt basic PHP grammar, Linux commands and website building with the help of lovely studio mates. The word says, “It’s never too late to start”, I will keep going in security industry, but for now, let me go pass CTF challenges first!
<br>
At first two weeks our team did a wide range research for some famous hacking news which caused millions or billions property lost, such as “Third-party application caused Facebook user info leaks” and “Massive DDoS attack on GitHub”. That was a great start for me to have a general idea about cyber attacking how its results. My mainly objective in week 1 is to do research about attacks happened in real-world and try some Wargames challenges on Overthewire website, also using SQL injection and other basic web attacks through the OWASP Juice shop. One special achievement that I built my first static website by using “hugo” templates and “Netlify” to deploy the site. The figure 1 below is one great resource that covered almost all the basic knowledge for beginner of web pentesting. 
![Pic1](/P-pentesting.png)

<br>
<br>
Last two weeks I felt really hard to follow the steps. Time management is a big problem in summer session, because the studio prepared a lot of resources and tasks to be done in a limited. However, I just figured out what is web penetration, new challenge – HackTheBox(HTB) come behind and I learnt a lot like open a compressed zip. HTB invite code spent me one week to get access in HTB. All kinds of attacking tools in Kali box were required so that I learnt them in a short time. One shortness is that sometimes I was confused which tool should I use in different situation. Like Luke said no experts were born as experts, just keep practicing and experience more. Furthermore, in last two weeks, I had been to SecTalk which is a friendly technician meet-up, and talked to professional staff who are really famous in this industry and learnt a lot about their personal experience sharing in Sec industry. The topic was about sub category of 802.15.4 protocol Zigbee is the most adopted. Zigbee is the wireless language that everyday devices use to connect to one another. In fact, Zigbee could be at work in your home right now.

![Pic1](/SecTalks.png)
<br>
![Pic2](/ST-heying.png)
<br><br>
### SLO 1: Engage with stakeholders to identify a problem
From my sight, engaging with stakeholders is also one efficient way to dive in this industry quickly. The interactive workshops from Darsh, Luke, Deloitte and Rubin lead the studio a positive and Agile study environment. There was one presentation by Robert from Gitlab, provided a basis for a simplified statement about security industry and the general trend of cybersecurity industry. That was a great chance for us to learn what are the real problems that security engineers are facing. 




### SLO 2: Apply design thinking to respond to a defined or newly identified problem

There were so many identified problems to walkthrough in 4 weeks. At the beginning, I did not know how to find hidden directory in website. In  [week 1](https://www.blank1024.me/post/week1-reflection/) , I learnt to test some common folder names such as: /images, /login…;  [In week 4](https://www.blank1024.me/post/final-report/)  when I tried to walkthrough HTB Curling, I learnt to use the tool - dirb to search potential web folders and found the possible vulnerabilities in them. 

Another example, when I did Mr.Robot on Tryhackme website. Its IP address direct to a WordPress based website which can be easily scanned by WPScan. To identify website vulnerabilities by : ~$ sudo wpscan - -url ‘url’ - -enumrate 

![Pic3](/P-Nmap.png)
<br><br>
### SLO 3: Apply technical skills to develop, model and/or evaluate design
By doing the HTB Curling, it did need a comprehensive research to walkthrough. 
1.Recon Stage - Using Nmap to search for port scanning; Using dirb to search for hidden web directory. 
2.Require a deep understanding of Joomla website structure. 
3.Encoding and decoding.
4.PHP injection and PHP-reverse-shell to access internal system.
5.Some CTF experiences to guide you to the correct way.

For this part, I highly recommend the resource:
(Link provid at the end of this portfolio)
![Pic4](/P-CTFweb.png)

<br>
### SLO 4: Demonstrate effective collaboration and communication skills
Reviewing passed 4 weeks, there is a lot of presentations I did, also free-for-all talking every morning, stand ups to discuss the milestones, challenges, and what roadblocks are encountered. The picture below is one record of Free-For-All notes.

![Pic5](/P-freeforall.png)

<br>

Teams online chatting helped me to solidify my understanding of key concepts and increased my confidence in demonstrating a practical attack to an audience. Part of online chatting evidence below: 
![Pic6](/P-GRP1.png)
<br>
![Pic7](/P-GRP2.png)
<br>
![Pic8](/P-GRP3.png)
<br>
Our team Bare Minimum Bandits did very well on effective collaboration that every group task like presentation, we acted as a scrum team that had a well-organized task distribution and everyone did efforts to achieve the same goal. Sometimes I lost the topic, Cowan and Chris are great mates and repeat the confusing part. Furthermore, me and Cowan shared our reflection website so that teammates can view and learn something new through visiting websites.

### SOL 5: Conduct critical self and peer review and performance evaluation
In 4 weeks, I think what I learnt and what I achieved is an honor for myself. But my weakness also explored. Lack of efficient communication and task_time management are terrible. Because of my first language is not English so that most of time, understanding what my teammates are talking about (with super-fast speaking speed) worried me a lot. I think I need to encourage myself to talk to other people positively. As for task_time management, I did not have a clear estimate of how long I am going to spend on walk through CTF challenge or write-up a reflection which caused my last two weeks acts pretty passive and lack of self-motivation. 
<br>
From week 1 to week 4, I had a significant improvement in offensive security. As I evaluated in SLO 2, with the help of studio mates, I started to challenge harder CTF and I will continue in future. 
<br>
Special thank you to Darshil Shah, who leaded me step-by-step to walkthrough the darkest time. Also thank you to Larry Jason, Cowan, Frank, Andy, Christopher and all other mates in Cyber Security who patiently and positively helped me a lot. Best wishes! 


### References: 

https://pentesterlab.com/exercises/web_for_pentester/course
<br>
_https://bitvijays.github.io/LFC-VulnerableMachines.html#rabbit-holes_

