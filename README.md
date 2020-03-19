# Dota_2_script
ENGS_110_Individual_Project

Target Audience - Dota_2 players(~700.000)
In the game exist heroes that need a lot of more keyboard touches, than other ones, to be useful in the game. A script which provides us with the oportunity to make several actions clicking on one button will increase human players' APS(Actions Per Second) and potentiality to be able to win AI bots.

f = q + q + e + r + t (auto ghost walk)

g = q + q + q + r + t + leftclick+ b + a + a + e + r + t + leftclick + q + e + a + r + t + leftclick (cold snap + hex + meteor + blast)e

h = e + e + q + r + t + leftclick(timing) + e + e + e + r + t + a + a + a + r + t + t(timing) + a + a + e + r + t + leftclick(timing) + q + e + a + r + t + leftclick(timing)


import time

1::
InstantInvis:
SendInput, qqe
time.sleep(.05)
SendInput, r
time.sleep(.2)
SendInput, t
return


2::
coldsnap:
SendInput, qqq
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput, t
return


3::
iceWall:
SendInput, qqa
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput, t
return

4::
EMP:
SendInput, eee
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput, t
return

5::
tornado: 
SendInput, eeq
time.sleep(.05)
SendInput, r
return


6::
alacrity:
SendInput, eea
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput, tt
return


7::
blast:
SendInput, qea
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput, t
return


8::
sunstrike:
SendInput, aaa
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput t
return


9::
forgedSpirits:
SendInput, aaq
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput, t
return


p::
meteor:
SendInput, aae
time.sleep(.05)
SendInput, r
time.sleep(.05)
SendInput, t
return

COMBOS

F::
tornado+emp+meteor+sunstrike+blast:
SendInput, 5
time.sleep(LiftTime - CastTime)
SendInput, 4
time.sleep(1.5)
SendInput, p
time.sleep(1.5)
SendInput, 8
time.sleep(2)
SendInput, 7
