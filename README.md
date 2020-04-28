

import pynput
from pynput.keyboard import Key, Controller
keyboard = Controller()

import json
import time
#import pyautogui, sys

with open("abilities.json") as file_data:
  data = json.load(file_data)
while True:
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
    time.sleep(1)

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
    time.sleep(1)

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
    time.sleep(1)

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
    time.sleep(1)

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

