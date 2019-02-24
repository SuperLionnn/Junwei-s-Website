---
title: "HackTheBox - How to get invite code"
date: 2019-02-13T09:08:48+11:00
draft: false
---

## HackTheBox

Link https://www.hackthebox.eu/invite

Firstly, try to find any interesting hidden folders.

These are folders I found: 
_image_
_image_png/
_js_
_css_
_password_
_password_reset/
_login_
_invite_
_storage_companies/
Error 403: 
Error 404: Source not found

- - - -

try input “”


![pic1](htf-xsrf.png)
XSRF Protection

Then try https://www.hackthebox.eu/invite/id 
Code 404 error
![pic2](htf-404.png)

- - - -
Try to find some in robots.txt but there is nothing
![pic3](htf-robot.png)

- - - -
Injection will be blocked 
https://www.hackthebox.eu/invite/%3CsCript%3Ealert(1);%3C/scRiPt%3E

![pic4](htf-injection.png)
- - - -
- - - -
Look at the source code
/inviteapi.min.js. file looks like the key point to get the invite code.
![pic5](htf-inviteapi.png)

See I found this — “makeInviteCode”, let’s try to find its contents
![pic6](htb-MICode.png)

Just type makeInviteCode() in Console and see what will happen.
![pic7](htf-Console.png)
There is a response and an encoded text hide there. 

Use CyberChef to decode ROT13
![pic8](htf-cyberchef.png)

Way 1 : Send POST request in Terminal
![pic9](htf-POST.png)

Way 2: In Chrome Developer Tool -> Console
![pic10](htf-way2.png)

Use CyberChef to decode
The text looks like be encoded by Base64, then try to decode it
![pic11](htf-cyberchef2.png)
Then copy and paste and click btn Sign up!
![pic12](htb-signup.png)
Bingo
![pic13](htb-bingo.png)

Looks cool at the Dashboard~ more challenges are w8ing for me!
![pic14](htb-inside.png)
- - - -

kali tools: 
**ident-user-enum**  (Port 113/TCP)
Description: Query ident to determine the owner of a TCP network process
  ident-user-enum is a simple PERL script to query the ident service (113/TCP)
  in order to determine the owner of the process listening on each TCP port of a target system.
  This can help to prioritise target service during a pentest (you might want
  to attack services running as root first).
  Alternatively, the list of usernames gathered can be used for password
  guessing attacks on other network services.
- - - -
Challenge Lernaean
1. Access, use command openvpn xxx.ovpn
2. Launch Instance
3. Open the page with port num
￼￼￼
![pic15](l.png)

4. Tried to type in some wrong text and get response “Invalid password”
5. Learn how to use Brup Suite to get more info behind the scene. 
Problem: Poor connection after proxy manual setup.
		No idea how to use it correctly

