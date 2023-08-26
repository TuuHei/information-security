# Darknet Diaries - Episode 126: REVIL

The episode talks about a ramsonware service and the group behind it spreading it into the world.
The guest of the episode is Will, who works for Equinix Threat Analysis Center as a threat intelligence analyst.
This episode was an interesting one. I've heard about ramsonware before and seen what it does, but I haven't read about
these attacks on the bigger companies discussed in the episode.

Before REvil, there was GandCrab which is also a ramsonware. It encrypts machines hard drives, and if the owner
wants the data back, they will have to pay the ramson to get an encryption key. I've seen this happen on personal computers where you only 
have to pay a hundred or two, but these cyber criminals behind GandCrab and REvil were ''big game hunting''. The idea is to
find the biggest companies you can attack. Big companies pay big, in these cases, millions.

Ramsonware as a service called REvil appeared in 2019 after GandCrab saw how profitable it is to sell
the ramsonware to others. It allows ''affiliates'' to use the ramsonware only if they 
have succesfully got themself into the victims network. After succesfully doing that, REvil will do the 
rest of the work, and if the victim pays the fee, the payment will go 60/40 or 70/30 favoring REvil.

I'll take one example from the episode to show how large some of these attacks can get. JBS, which is the worlds biggest
meat producer was attacked, resulting shutting down at least six plants in the US. These kinds of attacks aren't only
an inconvience for the company, but as it is deemed critical infrastructure it affects so many more people.
JBS had to pay 11 million dollars and it wasn't even the largest payment REvil had collected in their time.

## Installing Debian

First I downloaded VirtualBox and the correct Debian ISO Image, and followed instructions shown on the page: https://terokarvinen.com/2021/install-debian-on-virtualbox/

![kuva](https://github.com/TuuHei/information-security/assets/122973223/23df1db9-1330-4776-b208-b4dfcb93bcb9)

After setting up the virtual machine I did the final tweaks in storage the settings.

![kuva](https://github.com/TuuHei/information-security/assets/122973223/2b4223b6-f3ab-4c53-bfcc-f65ef3bf3103)

Next up I tried to boot it up, but this error occured. 

![kuva](https://github.com/TuuHei/information-security/assets/122973223/a7a7e16d-8322-480c-a086-777a01283c90)

I fixed it by enabling AMD-V in the bios following these instructions: https://youtu.be/qk42V6RfCro?si=4Vrz9sYcKCCKImu7&t=75

Once I got in, I tested the connection

![kuva](https://github.com/TuuHei/information-security/assets/122973223/d2ad6ee0-7d59-4b23-b9dd-a8a1ffea5f01)



![kuva](https://github.com/TuuHei/information-security/assets/122973223/1ffba58f-4bbf-4520-9a5d-d9ddef6d45ac)

