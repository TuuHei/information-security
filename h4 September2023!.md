## x) Read or watch and summarize

Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions:

* Computing of  one-way functions is relatively easy, but if you want to reverse them, it would take millions of years.
* Mathematically speaking, There is no proof one-way functions really exist.
* Trapdoor one-way fuction is the same as one-way functions, but there is a secret added, which makes the function computable in both directions.
* Hash functions take an input string, which varies in lenght, and converts it to an output string (hash value), which has a fixed length.

Soure: https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003

Särökaari 2018: Phishing trough email:

*
*
* Filtering, SPF, DMARC and DKIM are the main tools against phishing.
* 

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

![kuva](https://github.com/TuuHei/information-security/assets/122973223/b5e8cb6f-bf58-4d68-aff1-7c0704295e34

As MD5 is the most used in the top three, we are going to go with that.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/1932ef2b-d8a0-48eb-b384-8f91c60103c0)

It shows that it has cracked the passwords. Lets see what it is.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/1975e31e-1d67-4680-b055-e0555f75922a)










Phishing email

Pikkujoulu paikka tarjous
Kirjaudutaan työpaikan sähköpostilla
Lataa hintataulukko
