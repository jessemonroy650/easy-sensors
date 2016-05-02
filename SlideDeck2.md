# Anatomy of an IoT System #
Date: 2016-05-02

1. System Overview
2. Resistive Sensors
3. Voltage Divider
4. Arduino Schematic
5. Sensor Formula
6. Arduino Code
7. Bridge Examples
8. Actual Protocol
9. Polling vs. Push
10. Arduino Power Consumption
11. Phonegap Tools
12. HTML view
13. Ajax and JQuery

----

Person          | Organization          | time marks
----------------|-----------------------|------------
Jeff Bezos      | CEO Amazon            | [0s-11s](https://www.youtube.com/watch?v=QoqohmccTSc)
Steve Jobs      | CEO Apple Computers   | [12s-32s](https://www.youtube.com/v/QoqohmccTSc&start=12&end=33)
Kevin Systrom   | CEO Instagram         | [8m8s-8m34s](https://www.youtube.com/watch?v=QoqohmccTSc&start=489)
Mark Zuckerberg | CEO Facebook          | [16m14s-16m51s](https://www.youtube.com/watch?v=QoqohmccTSc&start=975)

----

- image of hot and cold
- image of Arduino Yun
- image of Wifi Symbol
- image of Mobile Phone

----

## Human Senses ##

https://en.wikipedia.org/wiki/Sense

1. **sight** - ophthalmoception
2. **sound** - audioception
3. **taste** - gustaoception
4. **smell** - olfacception
5. **touch** - tactioception
6. balance - equilibrioception
7. temperature - thermoception
8. vibration - mechanoreception

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

