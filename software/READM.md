Dowload from v1.24.0(2024-10-25).uf2  from
https://micropython.org/download/RPI_PICO/

+Install micropython 

+Open Thorny and select the board (bottom right corner)
+Create "blinky.py" on your computer and upload with Thorny (View->Files) 

------------
import time
from machine import Pin

print("starting")

OFF = 1
ON = 0

ledB = Pin(15, Pin.OUT)
ledR = Pin(13, Pin.OUT)
ledG = Pin(12, Pin.OUT)

ledB.value(OFF)
ledR.value(OFF)
ledG.value(OFF)

for i in range(10):
    ledR.value(OFF)
    time.sleep(1)
    ledR.value(ON)
    time.sleep(1)
---------

In Thorny (Shell) type the following
execfile ("blink.py")
