# Dota_2_script
ENGS_110_Individual_Project

Target Audience - Dota_2 players(~700.000)
In the game exist heroes that need a lot of more keyboard touches, than other ones, to be useful in the game. A script which provides us with the oportunity to make several actions clicking on one button will increase human players' APS(Actions Per Second) and potentiality to be able to win AI bots.

f = q + q + e + r + t (auto ghost walk)

g = q + q + q + r + t + leftclick+ b + a + a + e + r + t + leftclick + q + e + a + r + t + leftclick (cold snap + hex + meteor + blast)e

h = e + e + q + r + t + leftclick(timing) + e + e + e + r + t + a + a + a + r + t + t(timing) + a + a + e + r + t + leftclick(timing) + q + e + a + r + t + leftclick(timing)


from pynput.Keyboard import Key, Controller
keyboard = Controller()

import json

import time


"abilities" : [
  {
  "ability" : "cold_snap",
  "sphere_1" : "q",
  "sphere_2" : "q",
  "sphere_3" : "q"
  },
  {
  "ability" : "ghost_walk",
  "sphere_1" : "q",
  "sphere_2" : "q",
  "sphere_3" : "e",
  },
  {
  "ability" : "ice_wall",
  "sphere_1" : "q",
  "sphere_2" : "q",
  "sphere_3" : "a",
  },
  {
  "ability" : "emp",
  "sphere_1" : "e",
  "sphere_2" : "e",
  "sphere_3" : "e",
  },
  {
  "ability" : "tornado",
  "sphere_1" : "e",
  "sphere_2" : "e",
  "sphere_3" : "q",
  },
  {
  "ability" : "alacrity",
  "sphere_1" : "e",
  "sphere_2" : "e",
  "sphere_3" : "a",
  },
  {
  "ability" : "sunstrike",
  "sphere_1" : "a",
  "sphere_2" : "a",
  "sphere_3" : "a",
  },
  {
  "ability" : "forged_spirit",
  "sphere_1" : "a",
  "sphere_2" : "a",
  "sphere_3" : "q",
  },
  {
  "ability" : "chaos_meteor",
  "sphere_1" : "a",
  "sphere_2" : "a",
  "sphere_3" : "e",
  },
  {
  "ability" : "deafening_blast",
  "sphere_1" : "q",
  "sphere_2" : "e",
  "sphere_3" : "a",
  }
 ]


#InstantInvis:
keyboard.press('1')
keyboard.release(for ability ghost_walk in data print 'sphere_1', 'sphere_1', 'sphere_3')
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
keyboard.release('t')



#COMBOS


#tornado+emp+meteor+sunstrike+blast:

keyboard.press('2')
keyboard.release(for ability tornado in data print 'sphere_1', 'sphere_1', 'sphere_3')
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
#todo left in click in the arg
keyboard.release('t', 'LeftClick')
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

keyboard.release(for ability emp in data print 'sphere_1', 'sphere_1', 'sphere_3')
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
#todo left in click in the arg
keyboard.release('t', 'LeftClick')
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

keyboard.release(for ability chaos_meteor in data print 'sphere_1', 'sphere_1', 'sphere_3')
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
#todo left in click in the arg
keyboard.release('t', 'LeftClick')
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

keyboard.release(for ability sunstrike in data print 'sphere_1', 'sphere_1', 'sphere_3')
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
#todo left in click in the arg
keyboard.release('t', 'LeftClick')
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

keyboard.release(for ability deafening_blast in data print 'sphere_1', 'sphere_1', 'sphere_3')
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
#todo left in click in the arg
keyboard.release('t', 'LeftClick')
#todo get the data about hero level
time.sleep(LiftTime - CastTime)



