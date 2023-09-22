## x) Read or watch and summarize

Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions:

* Computing of  one-way functions is relatively easy, but if you want to reverse them, it would take millions of years.
* Mathematically speaking, There is no proof one-way functions really exist.
* Trapdoor one-way fuction is the same as one-way functions, but there is a secret added, which makes the function computable in both directions.
* Hash functions take an input string, which varies in length, and converts it to an output string (hash value), which has a fixed length.

Source: https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003

Särökaari 2018: Phishing trough email:

* Phishing means sending emails that look like they are from a reputable source, and the goal is to gain information.
* The information is gathered by malicious attachments or links.
* Sender Policy Framework (SPF) is a validation system which checks if the senders IP addres is the expected one.
* DomainKeys Identified Mail (DKIM) helps to validate that no one has tampered with an email during transmit by adding a digital signature in the emails headers.
* SPF and DKIM make domains more legitimate.
* Malware and spam filtering help to protect you against malicious attachmenst and poorly made phishing emails.

Source: https://www.youtube.com/watch?v=m9YFJGSHYtY

## a) Install Hashcat

First I updated linux and installed hashcat using.
- $ sudo apt-get update
- $ sudo apt-get -y install hashid hashcat wget

I also created a new directory for the exercise.
![kuva](https://github.com/TuuHei/information-security/assets/122973223/192881d6-4ade-45a9-901c-d0e729f49c2b)

Secondly I downloaded the Rockyou dictionary.
![kuva](https://github.com/TuuHei/information-security/assets/122973223/1aace2cb-62e1-431b-9e31-b55cc2a52799)

I'm going to use the same hash used in the exercice at: https://terokarvinen.com/2022/cracking-passwords-with-hashcat/.

I need to identify the hash type for 6b1628b016dff46e6fa35684be6acc96.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/b5e8cb6f-bf58-4d68-aff1-7c0704295e34)

>As MD5 is the most common one in the top three, we are going to go with that.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/1932ef2b-d8a0-48eb-b384-8f91c60103c0)

>It shows that it has cracked the passwords. Lets see what it is.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/1975e31e-1d67-4680-b055-e0555f75922a)

The password is summer.

## b) Crack this hash

Im trying to crack "8eb8e307a6d649bc7fb51443a06a216f" with the same method as above.

First identify the hashid:

![kuva](https://github.com/TuuHei/information-security/assets/122973223/73f7c4f5-366a-411d-8fbc-3be518ce3222)

Then MD5 seems to be again the most probable one, so I'll test that.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/e2719089-a00a-43ee-9824-c13a31890eca)

It has cracked it again. Lets see what the password is.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/344a853e-e4cf-4de6-b12c-36cc6043fad6)

It is february.


## c) Gone phishing

- How, and who am I phishing?

My idea is to create a fake event planning service. At this time it is concentrated on pre-Christmas parties. This could work against almost any-sized companies, as my fake service could provide smaller events like dinners or other activities for smaller groups. It would also offer cruises, for example, for bigger parties.

- How to lure

First step is to create and email which looks legit, and has content that could interest the recipient. I know that many companies have events like pre-Christmas parties for their employees, so I'm trying to get their interest by offering a variety of events. That alone might not get their interest, so I'm offering them discounts, which might peak their interest enough to go to the fake site or open attachments.

- The process

1. Making an email that looks it could be real. It has to look professional and have realistic offers. Email contains a link that leads to a fake website and an malicious attachment.
2. Send the email. My targets are Finnish companies. It is easy to find their contact information from the internet, and I could even directly contact their management.
3. If they take the bait and click the link, It would take them to the website, which has more opportunities to get their information. For example a  malicious file that is called "Pricing_2023". A fake email login could also be done to gather passwords and access to their emails. For this exercise I'll only focus on the email message.

- Creating the email

I copied an email i've gotten from Elisa, and I'm planning to take its structure and replace the contents with my own.

The email structure that I'll use: 

![kuva](https://github.com/TuuHei/information-security/assets/122973223/376b444f-45b4-4e12-88e0-e3fe660aef1b)

>Every company must have a logo, so I'll create one with a free tool online.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/b8cff99a-a769-41fe-999b-504b473a5389)

>Also made a quick banner using GIMP and stock images.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/b8b7f1ff-df7b-4a7a-9ffa-e37454730e1d)

>Here is the version after adding my pictures and text:

![kuva](https://github.com/TuuHei/information-security/assets/122973223/9f2fc986-1510-47e5-a790-5546bfa27f5f)

![kuva](https://github.com/TuuHei/information-security/assets/122973223/e9437a2c-d56b-41e6-913e-5aeb1b3b9d4c)

![kuva](https://github.com/TuuHei/information-security/assets/122973223/c8d7a3d6-0694-40c9-8128-8cbf547265ed)

> Every picture or text with a backround color would be a link in a real situation. I've also added a file to the email message. The real version would ofcourse be in Finnish.
