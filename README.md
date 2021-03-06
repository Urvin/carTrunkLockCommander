Car trunk lock commander
=====================

> *Firstly designed for my Lifan Smily (Lifan 320) car*

This is a motor- and wire- protection device for car trunk lock actuator/solenoid.
When you push the button on the trunk door, solenoid works for 0.8 second and then turns off, independently if you still hold the button or not.
The time is enough to open a trunk and to protect system to work on high-ampere current.

«Switch» is a device, that converts a +5V «doors opened» signal from BCM to a +12V power voltage going through the cabin to main lock control device.

##NE555 Component list
* [SA555 chip](http://ww1.microchip.com/downloads/en/devicedoc/41211d_.pdf) (same as popular NE555 with extended temperature range);
* [IRLR024NPBF MOSFET](http://www.irf.com/product-info/datasheets/data/irlr024npbf.pdf);
* [VS-6CWQ03FNPbF 2x3.5A diode](http://www.vishay.com/docs/94247/6cwq03fn.pdf);
* 2 x 0805 10kOhms resistors;
* 1 x 0805 100Ohms resistor;
* 1 x 0805 680kOhms resistor;
* 1 x 0805 47kOhms resistor;
* 2 x 0805 1uF capacitors;
* 1 x 0805 10nF capacitor.
* Can be supplied with connectors 3x3.96 and 2x3.96.

Instead of (680kOhms + 47kOhms) + 1uF elements (R3, C3 on schematics) you can use any other, that correspond the equation 0.8 = (R1 + R2) * C.
For example, use 150kOhms + 4.7kOhms + 4.7uF.

##Switch component list
* 2 x [IRLML2402 MOSFET](http://www.irf.com/product-info/datasheets/data/irlml2402.pdf);
* [IRF9540N MOSFET](http://www.irf.com/product-info/datasheets/data/irf9540n.pdf);
* 2 x 0805 100kOhms resistors;

##Directory tree
* circuit — device schematic diagram designed in Splan 7;
* layout — PCB layout designed in Sprint Layout 6;
* model — device simulation designed in Proteus 7;

##Photos, etc
You can read about this device in my car blog, [part 1](http://www.drive2.ru/l/3670015/), [part 2](http://www.drive2.ru/l/3711382/), in Russian.