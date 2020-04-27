# Dota_2_script
ENGS_110_Individual_Project

Target Audience - Dota_2 players(~700.000)
In the game exist heroes that need a lot of more keyboard touches, than other ones, to be useful in the game. A script which provides us with the oportunity to make several actions clicking on one button will increase human players' APS(Actions Per Second) and potentiality to be able to win AI bots.

f = q + q + e + r + t (auto ghost walk)

g = q + q + q + r + t + leftclick+ b + a + a + e + r + t + leftclick + q + e + a + r + t + leftclick (cold snap + hex + meteor + blast)e

h = e + e + q + r + t + leftclick(timing) + e + e + e + r + t + a + a + a + r + t + t(timing) + a + a + e + r + t + leftclick(timing) + q + e + a + r + t + leftclick(timing)




#abilities.json 

{
  "cold_snap" :
  {
    "sphere_1" : "q",
    "sphere_2" : "q",
    "sphere_3" : "q"
  },
  "ghost_walk" :
  {
    "sphere_1" : "q",
    "sphere_2" : "q",
    "sphere_3" : "e"
  },
  "ice_wall" :
  {
    "sphere_1" : "q",
    "sphere_2" : "q",
    "sphere_3" : "a"
  },
  "emp" :
  {
    "sphere_1" : "e",
    "sphere_2" : "e",
    "sphere_3" : "e"
  },
  "tornado" :
  {
    "sphere_1" : "e",
    "sphere_2" : "e",
    "sphere_3" : "q"
  },
  "alacrity" :
  {
    "sphere_1" : "e",
    "sphere_2" : "e",
    "sphere_3" : "a"
  },
  "sunstrike" :
  {
    "sphere_1" : "a",
    "sphere_2" : "a",
    "sphere_3" : "a"
  },
  "forged_spirit" :
  {
    "sphere_1" : "a",
    "sphere_2" : "a",
    "sphere_3" : "q"
  },
  "chaos_meteor" :
  {
    "sphere_1" : "a",
    "sphere_2" : "a",
    "sphere_3" : "e"
  },
  "deafening_blast" :
  {
    "sphere_1" : "q",
    "sphere_2" : "e",
    "sphere_3" : "a"
  }
}




#ind_project.py

import pynput
from pynput.Keyboard import Key, Controller
keyboard = Controller()

import json
import time
import pyautogui, sys

with open("abilities.json") as file_data:
  data = json.load(file_data)

#InstantInvis:
keyboard.press('1')
sphere_1 = ""
sphere_2 = ""
sphere_3 = ""
keyboard.release(data["ghost_walk"]["sphere_1"])
keyboard.release(data["ghost_walk"]["sphere_2"])
keyboard.release(data["ghost_walk"]["sphere_3"])
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
keyboard.release('t')



#COMBOS
#tornado+emp+meteor+sunstrike+blast:

keyboard.press('2')
try:
    while True:
        x, y = pyautogui.position()
        positionStr = 'X: ' + str(x).rjust(4) + ' Y: ' + str(y).rjust(4)
        print(positionStr, end='')
        print('\b' * len(positionStr), end='', flush=True)
except KeyboardInterrupt:
    print('\n')
sphere_1 = ""
sphere_2 = ""
sphere_3 = ""
keyboard.release(data["tornado"]["sphere_1"])
keyboard.release(data["tornado"]["sphere_2"])
keyboard.release(data["tornado"]["sphere_3"])
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
keyboard.release('t')
pyautogui.click(x,y)
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

sphere_1 = ""
sphere_2 = ""
sphere_3 = ""
keyboard.release(data["emp"]["sphere_1"])
keyboard.release(data["emp"]["sphere_2"])
keyboard.release(data["emp"]["sphere_3"])
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
keyboard.release('t')
pyautogui.click(x,y)
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

sphere_1 = ""
sphere_2 = ""
sphere_3 = ""
keyboard.release(data["chaos_meteor"]["sphere_1"])
keyboard.release(data["chaos_meteor"]["sphere_2"])
keyboard.release(data["chaos_meteor"]["sphere_3"])
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
keyboard.release('t')
pyautogui.click(x,y)
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

sphere_1 = ""
sphere_2 = ""
sphere_3 = ""
keyboard.release(data["sunstrike"]["sphere_1"])
keyboard.release(data["sunstrike"]["sphere_2"])
keyboard.release(data["sunstrike"]["sphere_3"])
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
keyboard.release('t')
pyautogui.click(x,y)
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

sphere_1 = ""
sphere_2 = ""
sphere_3 = ""
keyboard.release(data["deafening_blast"]["sphere_1"])
keyboard.release(data["deafening_blast"]["sphere_2"])
keyboard.release(data["deafening_blast"]["sphere_3"])
time.sleep(.05)
keyboard.release('r')
time.sleep(.05)
keyboard.release('t')
pyautogui.click(x,y)
#todo get the data about hero level
time.sleep(LiftTime - CastTime)

