---
title: "WEEK 3 REFLECTION"
date: 2019-02-23 T09:08:48+11:00
draft: false
---

## Week 3 was awesome!!

On Tuesday I participated SecTalks!

The studio focused on "Break Into Machines", which is pretty exciting and full of challenging. It is really a huge jump from playing wargames, CTFs, and vulnernable web apps. Thanks for research about hacking tools and Piper demo practiced in the class so that I was basiclly what was going on on the VMs.

On Wednesday, our team - Bare Minimum Bandits made the presentation about two tools
One is Wireshark

The other one is CyberChef

### Monday

#### Free-for-all
We randomly sit together and talk about what we did in last few days.

*Andre*
natas 
google it robots.txt
 popular way to build up a website 90% by wordpress or wix
but  not much people know how to make it secure 

*Ian* 
tight timetable and reflection
doing research about hack the box and now he can access the hack the box now.
eu concil 
He tried to type in search box "<>", "<'script'>", "<test>"
An error page occured 
- - - -
## PHP review

I reviewed PHP staments and some notes below

<? php
	This is a single line comment
#	This is a single line comment
/*
	This is a multiple line comment
*/
 You can also use comments to leave out parts of a code line
$x =5/* + 15 */+5; (a variable starts with $)
echo $x; ———(output is 10)

echo “This “,”string “,”was “,”made “,”with multiple parameters.”;
print “can only have one argument ”

?>  
- - - -

Some tools metioned by other group at presentation

jack ripper . (a password cracker)
beef . (safe)
aircrack  . (Wifi attacker)

- - - -

![Pic1](/W3-Au.Bypass.png)

- - - -
It was the first time I participated in SecTalks at PwC
Topic "802.15.4 War Driving"
![Pic2](/SecTalks.png)
![Pic3](/ST-chips.png)
![Pic4](/ST-heying.png)

### Zigbee
Sub category of 802.15.4 protocol 
Zigbee is the most adopted 

Zigbee is the wireless language that everyday devices use to connect to one another. In fact, Zigbee could be at work in your home right now.

*Characteristics*

1. Low battery consumption. A ZigBee end device should operate for months or even years without needing its battery replaced.
2. Low cost.
3. Low data rate. The maximum data rate for a ZigBee device is 250Kbps.
4. Easy to implement.
5. Supports up to 65,000 nodes connected in a network.
6. ZigBee can automatically establish its network.
7. ZigBee uses small packets compared with WiFi and Bluetooth. 

*Attack surface*

*HW & SW options*

FreakUSB 

Massive mapping out

Beefing up

SecTalks is definitely a great meetup for who work or new in Cyber Security industry. At the evening, I met Tom & David who have more than one year working experience in internet-working and HTTP field. They are 
The fantastic presentation by Edward Farrell confused me a lot.
- - - -
## Let’s break into machines!

In week 3, the studio focused on “Break Into Machines", which is pretty exciting and full of challenging. It is really a huge jump from playing wargames, CTFs, and vulnerable web apps. Thanks for research about hacking tools and Piper demo practiced in the class so that I was basically what was going on on the VMs.

On Wednesday, our team - Bare Minimum Bandits made the presentation about two useful tools. We shared information on Microsoft Teams

One is **Wireshark**
![Pic5](/W3-Wireshark.png)
#### Offensive
* Can be used for active hacking e.f. MITM 
* Traffic 
#### Defensive 
* Network Forensics

##### Example: Network traffic detection

![Pic6](/W3-Wire-Example.png)

### The other one is *CyberChef*
![Pic7](/W3-CyberChef.png)

##### Example : Natas Level 8 

![Pic8](/W3-Natas.png)

----
## Let’s break into machines!

# TryHackMe - Mr Robot CTF
TryHackMe is a super cool free website for Cyber Security education. It offers a platform makes learning and teaching Cybersecurity a comfortable experience to learn by designing prebuilt courses which include virtual machines (VM) hosted in the cloud ready to be deployed. 

This week I tried to get in TryHackMe - Mr.Robot 

### Task 1 Connect to our network
Task arrange is really friendly that teach me how to connect the network and start the challenge. 

### Task 2  Hack the machine

Deploy first then we can start with the IP Address

#1 
![Pic9](/W3-MR-Burp.png)

- - - -
![Pic10](/WK3-MR-WPlogin.png)
- - - -
Yes! I login as Administrator, that means I can install plugin.
Then we need to exploit the WP server.
#Reverse-Shell
![Pic11](/WK3-MR-Admin.png)
- - - -
Open msfconsole and see if there is any exploits in metasploit

![Pic12](/WL3-MR-Metasploit.png)

- - - -
Type in ‘search wp_admin’ and find one matching module that has excellent rank, looks it will work through.
![Pic13](/WK3-MR-WP-admin.png)

Sorry I did not get key 2 and key 3 at the moment, because the Metasploit did not work and I have no idea about it just stuck there. But I found a video that show using password brute force tools to get this virtual machine. 

<a href="http://www.youtube.com/watch?feature=player_embedded&v=pgfYKUXGhOY
" target="_blank"><img src="http://img.youtube.com/vi/pgfYKUXGhOY/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="600" height="540" border="10" /></a>
- - - -
### Reference

Tryhackme, <https://tryhackme.com/><br>
Ata.E & Adam.G, 2009, <http://www.informit.com/articles/article.aspx?p=1409785&seqNum=2><br>
HackerSploit, 2018, <https://www.youtube.com/watch?v=pgfYKUXGhOY><br>
Pentesting Field, 2017, <https://pentestlab.blog/category/privilege-escalation/><br>
