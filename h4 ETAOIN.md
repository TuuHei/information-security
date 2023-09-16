## Schneier 2015: Applied Cryptography: Chapter 1: Foundations

* Cryptography is the science of keeping messages secure.
* Cryptanalysis tries to recover the message without acces to the key.
* Cryptographys requirements are confidentiality, authentication, integrity and nonrepudiation.
* The algorithm and all the possible keys, ciphertexts and plaintexts make a cryptosystem.
* The secrecy of the cryptosystem doesn't make it powerful. The best algorithms are the public ones which haven't been broken yet.
* To reduce the risk of attacks, the value of the data should remain less than the cost to break the security systems.
* Good cryptosystems are designed to work even after the expected rise in computing power in the future.
* 
.. further reading

## y)
The six most common letter for the Finnish language are A (11.45%), I (10.46%), T (9.98%), N (9.14%), E (8.42%) and S (6.59%). https://www.sttmedia.com/characterfrequency-finnish

## z) Choose a password manager.

I chose KeePassXC as my password manager. It can be helpful against brute force attacks, since you can use very complicated passwords without having to remember them all. Also if your password have been leaked from someones database, the hackers wouldn't benefit having only one of your passwords, since they vary from site to site.

Password managers encrypt the database you put your login information in. Cloud based password managers use zero-knowledge technology, that encrypt the data, lets say on my device, before sending it to the server. 

KeepassXC is licensed under GPL-2 or GPL-3.

KeepassXC allows you to store the data where you choose. You can select any location you want or put them on the cloud. 

The data is protected by AES-256 encyption.


## a) ETAOIN

HDMH'B TH. KWU'YI AWR WSSTOTMJJK M OWQINYIMLIY! MB KWU BII, BTGPJI BUNBHTHUHTWA OTPDIYB OMA NI NYWLIA RTHD SYIEUIAOK MAMJKBTB. BII KWU MH DHHP://HIYWLMYCTAIA.OWG

The task was to crack the ciphertext seen above. I started by making a list of alphabets and put a "=" mark next to them for example A = ? , B = ?, C = ?... Then I started to analyze the mess of symbols seen above. I saw that the last sentence looks like an URL, and I got my first symbols cracked. DHHP:// = HTTP://. and .OWG = .COM. Then I replaced all the remaining D's, H's, O's, W's and G's. Then I went from the shortest words to the longer ones until I had all the symbols right. 

that's it. you're now officially a codebreaker! as you see, simple substitution ciphers can be broken with frequency analysis. see you at http://terokarvinen.com


## b) Demonstrate the use of a password manager.

Lets use KeepassXC for this example. You download it from their website and you open the application. You have to create a database, that you protect with a strong password. Once the database is done and stored probably on your computer, you can start adding information in the database. KeepassXC has a password generator, so you can create strong passwords and keep them safe in the database. You can say bye bye to your passwords if they are stored offline and you forget your database's password or something happens to your hard drive.

## c) Encrypt and decrypt a message

I use GnuPG as an encryption method. I tried to recreate what we did in school, but a little different. I installed GnuPG on both of my virtual machines, and created both public keys. Then I exchanged them via email.

Then it was time to create the message. I made an asc. file with the message inside it, and encrypted it using $ gpg -e -r "Matti" viesti.asc. Matti is the receiver. It then created a file looking like this:

![kuva](https://github.com/TuuHei/information-security/assets/122973223/aaac68ee-da46-48ec-a4d4-2ed7458e2a4b)

I then sent the file again via email, and opened it with "Matti"'s virtual machine using $ gpg -d viesti.asc.gpg. It then shows the decrypted message.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/bae5384b-4195-4f0d-bd78-fbecf0b1656a)







