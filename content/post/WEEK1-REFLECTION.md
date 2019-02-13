---
title: "WEEK 1 REFLECTION"
date: 2019-02-13T09:08:48+11:00
draft: false
---

## At the beginning

<p>
	The first week in Cyber Sec Studio let me know a new world of network which is sophisticated, sapiential, dangerous and full of unknows. Under the help with friendly mates in the studio, this would be a great chance to dive deeper in the internet, and to learn and see how cyber things work. Because cyber-attacks always happen all around the world, so that cyber security become more and more important. There is a word said, “the best way to defense is attack.” After this summer studio, I hope I can have a general knowledge of cyber security especially in Web application Security and enjoy sharing knowledge. 
</p>

## What I experienced?

<p>
	The first day, when I grabbed T-shirt and sit down there, I felt all of students are engaged and full of energetic. There was a man who looks like more than 40 years old with at least 20 years working experience. He taught me a lot hidden rules in workplace. Like ‘technician only like to talk to technician’, ‘achievement is more important than education when you work more than 5 years’. It really is a fantastic experience that talk to people in different fields. Sometimes it opens my mind and learns a lot from them.
</p>

## Meet new friends

<br>

## Team & Studio

My team member: Rowan, Christopher and Corey. 
Very lucky to team with these guys. Rowan and Chris helped me a lot in team. Because this is the first time I get in touch with cyber security, sometimes I cannot really follow the topic when people speak English too fast, they would ask me if I understand or not. And they are actively talk to me. 

Also, Larry and Darsh are great too, they have abundant experience and knowledge to share with us. Leading the studio to discover questions by ourselves under a friendly, technical and professional study atmosphere. 

Jason helped me a lot when I was struggling with CTF and natas. I have to say he is a geek that he got those flags like cookies in the dish. He taught me how to penetrate a vulnerable website by using SQL injection ‘OR 1=1 --' tricks and decrypting of MD5 cipher and cookies token to get domain authority.

## Defined a problem and made a presentation

<p>
The major task of week 1 is to define a problem. Our team did a lot of research about latest cyber security news. Finally, we chose our topic based on [Massive DDoS Attack Generates 500 Million Packets per Second](https://www.darkreading.com/attacks-breaches/massive-ddos-attack-generates-500-million-packets-per-second/d/d-id/1333766), and we mainly discussed about principle of DDoS attack, SYN flood, Browser Based Bots, business impact, High Bandwidth vs High PPS and problem solution - Mitigation. 
</p>

<br>
![pic1](/SearchNewsRecord.png)
<br>
<p>From Larry’s feedback, my part of the presentation is not good because of too general. Browser based bots need more research for specific attack such as XSS.
<br>
<br>
Cross-site scripting (XSS) is a type of computer security vulnerability typically found in web applications. XSS enables attackers to inject client-side scripts into web pages viewed by other users. A cross-site scripting vulnerability may be used by attackers to bypass access controls such as the same-origin policy.
</p>

## What I learnt?
### Agile Methodology
<br>
<p>A good way to work out clients’ needs and solve the problem. We have efficient and face-to-face communication. Using sprints to record the workflow and work on it Iteratively but make changes every time. </p>
![pic2](/Agile.png)
<br>
## DDoS
![pic2](/DDoS.png)
<br>
### What is a DDOS attack?
<p>What is a DDOS attack?
A distributed denial-of-service (DDoS) attack occurs when multiple systems flood the bandwidth or resources of a targeted system</p>

### What is a TCP 3 Way Handshake?

<p>
A TCP connection is established through a 3-way handshake. The client sends a an SYN packet (connection request) to a server. It receives the packet sent by the client and acknowledges the connection. The client then establishes a connection with the server by sending an ACK (or acknowledgement) packet back to the client.
</p>

<br>

### What is a SYN-Flood Attack

<p>A SYN-Flood attack sends repeated Syn (Synchronize) packets to every open port on a server, often using a fake address. The server thinks these are legitimate requests and tries to establish a connection. Responds to each SYN-ACK packet to each open port. The attacker doesn’t respond back to complete the 3-way handshake, or if the IP address is spoofed (doesn’t receive the packet in the first place). The server cannot stop the connection by sending an RST (reset) packet, so the connection stays open. Before the connection time out another SYN packet will arrive.
<br>
The goal of the SYN floods are to exhaust network ports and clog your ports with fake packets to achieve network saturation, and to exhaust resources like the CPU and network bandwidth.</p>

### Impact on the Business

<p>
DDoS attacks in general can often make websites and servers unavailable to legitimate users for hours, days or even months. This can have several critical impacts on businesses which rely on customer traffic to their sites.
</p>

1.	Loss of revenue – for retail sites, sites that rely on ad revenue or that provide a premium subscription based SaAS e.g. GitHub

2.	Damage customer trust – If a website which contains sensitive information or is a service which user’s reliably need, then the business may lose the trust of the employee

3.	Reputation damage – The company’s reputation as a whole could be negatively affected.

4.	Large compensation costs – If the inaccessibility of the website/servers causes the customers to directly or indirectly lose money, the company could be forced to pay large compensation costs. For example, an internet banking site which is down and therefore does not let the customer access their funds. An event/subscription service that was paid for and could not be accessed by the customer.


### High Bandwidth vs High PPS

<p>
	There are two main attack types (or vectors) that can be involved with a SYN-Flood.
The first is a high bandwidth attack. This consists of a small number of large-sized packets and can be up to hundreds of gigabits per second. The infamous GitHub attack consisted mainly of large packets sent from the same port on different servers at low PPS (129.6m). It was one of the largest bandwidth-intensive attacks ever. They often cause more collateral damage to bystanders due to being crowded by congestion, which forces out users.
The second attack type uses high Packets Per Second (PPS) in order to increase the intensity of the attack. This is often more difficult to generate as it requires far more compute resources. The Imperva attack consisted of 4 times the number of packets of the GitHub attack, sent from random sources i.e. 500 (Mpps). They do not saturate links as often.
The impact of an attack depends on the attack vector and vulnerability of the target. Both can be equally damaging. Multivector attacks are the most damaging, as they consist of multiple attack types and tools, making them far more difficult to generate and mitigate.
</p>

### Mitigation

<p>
	"In reality, size isn't the best reflection of how difficult attacks are to mitigate or how damaging they can be. Packets per second (PPS) is actually a better indicator.”- Tomer Shani, Security Researcher at Imperva
Different vectors have different mitigation challenges.
For High Bandwidth. greater provisioning of network bandwidth reduces the effectiveness of the attack. Not cost effective for most businesses, but this is where economy of scale comes into play. Create network bandwidth with larger capacity than largest known/observed DDoS attack.
Mitigating PPS is more difficult due to the processing power required to evaluate every packet. Requires much higher capacity on routers and switches than usual. Organizations more concerned with size of attack (number of packets) rather than the PPS.
</p>

<br>

1.	Microblocks – Admin can allocate small memory blocks instead of complete connection object per connection.

2.	SYN Cookies – Uses cryptography. Server sends SYN-ACK message with seq number produced from client IP/port number and other unique info. Client responds with ACK with hash of seq num. Server only initiates connection if hash is verified.

3.	RST Cookies – for the first request from a given client, the server intentionally sends an invalid SYN-ACK. This should result in the client generating an RST packet, which tells the server something is wrong. If this is received, the server knows the request is legitimate, logs the client, and accepts subsequent incoming connections from it.

4.	Stack tweaking – Admin can tweak TCP stacks to mitigate the effect of SYN floods e.g. reduce timeout duration.

### Capture the flag

<p>
	I spent at least 3 hours every day on this game. It gave me so much fun especially when I capture the hidden flag for next level. The most important thing is I learnt a lot from attacking the vulnerable website. Some notes I took below.
<p/>
<br>

