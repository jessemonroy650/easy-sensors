# Anatomy of an IoT System #
Date: 2016-05-02<br>
Last Update: 2016-05-03

1. Quick Videos
2. What is IoT?
3. Human Senses
4. System Overview
5. Resistive Sensors
6. CPU Vendors
7. Sensor Vendors
8. Ohm's Law
9. Voltage Divider
10. Close Up of Arduino Schematic
11. Thermistor Formula
12. Arduino Code
13. Bridge Examples
14. Control Protocol
15. Polling vs. Push
16. Arduino Power Consumption
17. Phonegap Tools
18. HTML view
19. Ajax and JQuery

----
## Quick Videos ##

Person          | Organization          | time marks
----------------|-----------------------|------------
Jeff Bezos      | CEO Amazon            | [0s-11s](https://www.youtube.com/watch?v=QoqohmccTSc)
Steve Jobs      | CEO Apple Computers   | [12s-32s](https://www.youtube.com/watch?v=QoqohmccTSc&start=12&end=33)
Kevin Systrom   | CEO Instagram         | [8m8s-8m34s](https://www.youtube.com/watch?v=QoqohmccTSc&start=489)
Mark Zuckerberg | CEO Facebook          | [16m14s-16m51s](https://www.youtube.com/watch?v=QoqohmccTSc&start=975)

----
## What is IoT? ##

----
## Human Senses ##

https://en.wikipedia.org/wiki/Sense

1. **sight** - ophthalmoception
2. **sound** - audioception
3. **taste** - gustaoception
4. **smell** - olfacception
5. **touch** - tactioception
6. *balance* - equilibrioception
7. *temperature* - thermoception
8. *vibration* - mechanoreception

----
## System Overview ##

- image of hot and cold
- image of Arduino Yun
- image of Wifi Symbol
- image of Mobile Phone

----
## Resistive Sensors ##

| Sense  |    sensor   |  source/price |
|--------|-------------|--------------:|
| Sight  | PIR         | [adafruit](http://www.adafruit.com/products/189)  $9.95<br>[sparkfun](https://www.sparkfun.com/products/13285) $9.95<br>[ebay](http://www.ebay.com/itm/HC-SR501-Adjust-IR-Pyroelectric-Infrared-PIR-Motion-Sensor-Detector-Module-NEW-/271638488228) $1.35 |
| Sight  | Mini Photocell<br>(photo detector) | [adafruit](http://www.adafruit.com/products/161) $0.95<br>[sparkfun](https://www.sparkfun.com/products/9088) $1.50<br>[ebay](http://www.ebay.com/itm/20x-5537CDS-Photo-Light-Dependent-Sensitive-Resistor-Photoresistor-LDR-Photocell-/271591239495) 20 @ $3.99<br> |
| Sight  | Ambient Light<br>(TEMT6000) | [adafruit](http://www.adafruit.com/products/1384) $3.95<br>[sparkfun](https://www.sparkfun.com/products/8348) $1.50<br>[ebay](http://www.ebay.com/itm/1pcs-TEMT6000-Light-Sensor-TEMT6000-Professional-Light-Sensor-IC-NEW-/262030683849) $3.70 |
| sound  | -           | -  |
| Smell  | -           | -  |
| Touch  | load        | [adafruit](http://www.adafruit.com/products/166) $7.00<br>[sparkfun](https://www.sparkfun.com/products/10245) $9.95<br>[ebay](http://www.ebay.com/itm/M-Electronic-Balance-Weighing-Load-Cell-Sensor-0-5Kg-K-/331571837632) $2.50 |
| Touch  | weight      | [adafruit](http://www.adafruit.com/products/166) $7.95<br>sparkfun<br>[ebay](http://www.ebay.com/itm/M-Electronic-Balance-Weighing-Load-Cell-Sensor-0-5Kg-K-/331571837632) $2.50 |
| Balance | Tilt <br>(AT407) | [adafruit](http://www.adafruit.com/products/173) $2.00<br>[sparkfun](https://www.sparkfun.com/products/10289)  $1.95<br>[ebay](http://www.ebay.com/itm/Vibration-Knock-Sensor-5-Pack-Tilt-SW-18020P-AT407-Mercury-Free-5x-5pcs-/231740544669) 5 @ $3.83 |
| temperature | temperature<br>(TMP36) | [adafruid](http://www.adafruit.com/products/165) $1.50<br>[sparkfun](https://www.sparkfun.com/products/10988) $1.50<br>[ebay](http://www.ebay.com/itm/1pcs-TMP36GT9-ORIGINAL-Low-Voltage-Temperature-Sensors-/181004901020) $1.36<br>[ebay](http://www.ebay.com/itm/5pcs-TMP36GT9-ORIGINAL-Low-Voltage-Temperature-Sensors-/181004901551) $5.31 |
| vibration | Piezo Vibration<br>(small) | [adafruit](http://www.adafruit.com/products/1740) $0.95<br>[sparkfun](https://www.sparkfun.com/products/9198) $2.95<br>[ebay](http://www.ebay.com/itm/Piezo-Vibration-Sensor-Small-Vertical-/271618771586) $2.79 |

- icons of 5 senses
- small images of sensors

----
## CPU Vendors ##

- [Arduino Yun](https://www.arduino.cc/en/Main/ArduinoBoardYun), Yun Mini, Tian
- [Particle Photon Kit](https://store.particle.io/)
- [Raspberry Pi 2](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/)
- [BeagleBone Black](https://beagleboard.org/black)

----
## Sensor Vendors ##

- [adafruit](http://www.adafruit.com/)
- [sparkfun](http://www.sparkfun.com/)
- [mouser](http://www.mouser.com/)
- [digikey](http://www.digikey.com/)
- [Seeed Studio](http://www.seeedstudio.com/depot/)
- [Newark](http://www.newark.com/)
- [Jameco](http://www.jameco.com/)
- [Arduino List](http://playground.arduino.cc/Main/Resources)

----
## Ohm's Law ##

Ohms Law => I = V / R

- icon of Ohm
- image of Ohm's Law


----
## Voltage Divider ##

> a series of resistors or capacitors that can be tapped at any intermediate point to produce a specific fraction of the voltage applied between its ends.


- image of voltage divider circuit

----
## Close Up of Arduino Schematic ##

- drawing of overview
- drawing of close up


----
## Thermistor Formula ##

- http://playground.arduino.cc/ComponentLib/Thermistor2
- http://www.eidusa.com/Electronics_Kits_TEMP_THERMISTOR_1.htm

- R = 10K * { (2V / Vout) -1}
- 1/T = a + b ln(R) + c (ln(3))^3

----
## Arduino Code ##

    const secondsDelay  3;

    void loop () {
         /* ::: */
         temp = analogread(a0);
         transTemp = translate(temp);
         print (transTemp);
         delay (1000 * secondsDelay);
         /* ::: */
    }


----
## Bridge Tutorial ##

Action        | URL | translates to code
--------------|-----|--------------------
Read Digital  | http://myArduinoYun.local/arduino/digital/13     | `digitalRead(13);`
Write Digital | http://myArduinoYun.local/arduino/digital/13/1   | `digitalWrite(13,1);`
Write Analog  | http://myArduinoYun.local/arduino/analog/9/123   | `analogWrite(9,123);`
Read Analog   | http://myArduinoYun.local/arduino/analog/2       | `analogRead(2);`
Set Input     | http://myArduinoYun.local/arduino/mode/13/input  | `pinMode(13, INPUT);`
Set Output    | http://myArduinoYun.local/arduino/mode/13/output | `pinMode(13, OUTPUT);` 

----
## Control Protocol ##

R or W | URL | translates to code
-------|-----|--------------------
Read   | http://myArduinoYun.local/arduino/analog/1      | `analogRead(A1);`
Write  | http://myArduinoYun.local/arduino/analog/1/0    | `analogWrite(A1,0);`
Write  | http://myArduinoYun.local/arduino/analog/1/1023 | `analogWrite(A1,1023);`

----
## Polling vs Push ##


----
## Yun Power Consumption ##

http://playground.arduino.cc/Hardware/Yun#power_consumption

Power consumption in mA |
--------------------------------------------|-----|---------|------ 
 Configuration                              | min | typical |  max
--------------------------------------------|-----|---------|------ 
WiFi on, no wired connection, no sd         | 170 | 240     | 300
WiFi on, wired connection, no sd            |     | 277	    |
WiFi on, wired connection, no sd, max. load |     | 315     |

Disabling the WiFi on the board saves ~20mA

Typical mobile phone battery is 800mA - 2000mA

----
## Phonegap Overview ##

Tools available

- HTML5
- CSS3
- Javascript
- Phonegap Plugin (Accelerometer, GPS, Camera, Media (audio), UI, etc)
- Third-Party Plugin (Paypal, Urban Airship, Push, in-app Purchase, QR-code reader, [etc](https://cordova.apache.org/plugins/))
- Javascript Library (User Interface, HTML5 API, etc)
- Online Service (Parse (DB), Firebase (DB), PubHub (RT Messaging), Pushbot (Push Messaging/Twitter) , etc)

----
## HTML view ##

    Temperature <span id=data></span>

----
## Ajax and JQuery ##

    $.get(URL, function(data) {
        $('#data').text(data);
    });


