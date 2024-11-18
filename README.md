# What is a LED?
LED stands for Light Emitting Diode, and it's a semiconductor device that emits light when
an electric current passes through it.

## Tutorial 1: Make an LED blink (in Python)
1 ) Materials:
   
- 1x LED
- 2 Female/Male Jumpers
- 1x Resistor 100 ohn
- Breadboard
- Raspberry Pi
- Micro SD Card
  
2 ) Building the Circuit:

_Step 1:_ <br>
Connect one of the female/male jumper to the GND pin
 
_Step 2:_ <br>
Connect another female/male jumper to the GPIO 17 pin

_Step 3:_ <br>
Connect the GND jumper to the negative row of the breadboard (Right Side)

_Step 4:_ <br>
Connect the GPIO 17 jumper to the positive row of the breadboard (Right Side)

_Step 5:_ <br>
Grab your LED and connect it to the negative row and the other leg to the 25 column (Right side)

_Step 6:_ <br>
Grab your resistor and connect it to the positive row and the 25 column (Right Side)

3 ) Set Up the Code:

You need to import the LED module:
<pre>
from gpiozero import LED
</pre>

Create a variable named "led" and attach the "LED(17)" value to it:

<>	*led = LED(17)*

The 'led.on()' method turns on the LED:

<>	*led.on()*

The 'led.off()' method turnd off the LED:

<>	*led.off()*

The 'led.toggle()' method changes based on the current state of the LED. If the LED is on it will turn it off, and if the LED is off it will turn it on:

<>	*led.toggle()*
