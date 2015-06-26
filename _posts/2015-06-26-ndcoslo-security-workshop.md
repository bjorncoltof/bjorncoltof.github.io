---
layout: post
title: NDC Oslo 2015 Hack Yourself First workshop
---
This year I had to pleasure to go to the [NDC Oslo][NDC] conference. I attended the two day preconference workshop 'Hack Yourself First' by [Troy Hunt][TH] which I'll give a short overview of in this post. For the rest of the conference stay tuned for another post (or two).

Troy Hunt is a well known security expert and also a [Pluralsight][PS] author.  To support the workshop and the associated training course [Hack Yourself First: How to go on the Cyber-Offense][HYF],  Troy hosts a site at [Hack Yourself First][HYFS] which is full of sloppy security practices. The setup of the workshop was to first cover a subject (theory) and then do an exercise to exploit the vulnerability that was just explained. In the remainder of this post I will shortly list the subjects that were covered and refer you to Pluralsight courses for more information on the threats /vulnerabilities and how to deal with them. I'd like point out that for me the hands-on hacking was what made these two days very valuable as that really made the security risks real and not just something mentioned in a report by an auditing firm.


##Subjects covered
- **SQL Injection** (Error Based, Union Based, Blind Boolean based, Blind Time based): This vulnerability is one that many people are aware of but somehow is still number 1 in [OWASP Top 10][OWASP] list.
- **Cross Site Scripting** (XSS): This vulnerability can lead to the attacker being able to execute arbitrary JavaScript in your site. This is most often the result of bad input sanitization and/or improper output encoding.
- **Cross-Site Request Forgery** (CSRF)
- **Content Security Policy** (CSP)
- **HTTP Strict Transport Security** (HSTS)
- **Brute-Force Attacks**: How to counter these and how this interacts with usability 
- **Account Enumeration**: Expose who your systems users are. Could not be a issue at all, but if your [adultfriendfinder.com](http://adultfriendfinder.com "AdultFriendFinder") it might be a bigger issue.
- **HTTP vs. HTTPS**: HTTP is very vulnerable to Man In The Middle (MITM) attacks. That's why Chrome will soon start marking pages served over HTTP as unsafe. Using his [Pineapple](https://www.wifipineapple.com/ "Pineapple") Troy easily launched a MITM attack on a number of devices that automatically connected to the local WiFi. 
- **Cookies**: Plain, HttpOnly and Secure
- **FiddlerScript**: [Fiddler](http://www.telerik.com/fiddler "Fiddler") is great tool to monitor and change traffic between systems. [FiddlerScript](http://docs.telerik.com/fiddler/KnowledgeBase/FiddlerScript/ModifyRequestOrResponse "FiddlerScript") amongst others allows you to script traffic as it is flowing through the system.
- **Automating**: Doing this by hand is tedious and most importantly slow, so of course automated tools have been created. E.g. we used sqlmap to expose some SQL injection vulnerabilities in the [Hack Yourself First][HYFS] site.

##Courses
- [Hack Yourself First: How to go on the Cyber-Offense][HYF] by [Troy Hunt][TH]
- [Ethical Hacking: SQL Injection][SQLI] by [Troy Hunt][TH]
- [Web Security and the OWASP Top 10: The Big Picture][TH_OWASP] by [Troy Hunt][TH]
- [OWASP Top 10 Web Application Security Risks for ASP.NET](http://www.pluralsight.com/courses/owasp-top10-aspdotnet-application-security-risks) by [Troy Hunt][TH]

##NDC Oslo Videos
- *Making Hacking Child’s Play* by Troy Hunt (sadly the video upload was not succesful)
- [*50 Shades of AppSec*](https://vimeo.com/131411406 "50 Shades Of AppSec") by [Troy Hunt][TH]
- [*.Net Rocks Panel on Application Security*](https://vimeo.com/131640203 ".Net Rocks Panle on Application Security") with Andre Klingsheim, Barry Dorrans, Troy Hunt, Niall Merrigan, Carl Franklin and Richard Campbell


##Information sources
- [OWASP Top 10 2013][OWASP]
- [Notes](https://theholyjava.wordpress.com/2015/06/17/notes-from-troy-hunts-hack-yourself-first-workshop/) from [@HolyJak](https://twitter.com/HolyJak) made during the workshop

[TH]: http://www.troyhunt.com/ "Troy Hunt"
[NM]: https://twitter.com/nmerrigan "Niall Merrigan"
[OWASP]: https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project#tab=OWASP_Top_10_for_2013 "OWASP Top 10"
[TH_OWASP]: http://www.pluralsight.com/courses/web-security-owasp-top10-big-picture "Web Security and the OWASP Top 10: The Big Picture"
[HYF]: http://www.pluralsight.com/courses/hack-yourself-first "Hack Yourself First: How to go on the Cyber-Offense"
[HYFS]: http://hackyourselffirst.troyhunt.com/ "Hack Yourself First"
[SQLI]: http://www.pluralsight.com/courses/ethical-hacking-sql-injection "Ethical Hacking: SQL Injection"
[PS]: http://www.pluralsight.com/ "Pluralsight"
[NDC]: http://www.ndcoslo.com "NDC Oslo"


