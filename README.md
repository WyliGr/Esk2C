# Esk2C - Electric Skateboard

**How to Build One ?**

> Open-Source Electric Skateboard / Longboard affordable for everyone
> 

# Hardware

**A simple Skateboard** can be used for that, you don’t need a specific one or build one from scratch (But you can if you want)
A skateboard is composed of a board, Trucks, Wheels and Bearings and a grip. You can find everything per piece or buy a skateboard pre-mounted.

## Motorisation

You can fin two systems of motorisation :
- Pulley Motor
- In-wheel Motor

### Pulley Motor

A motor drives a Belt which drives a wheel. It is an apparent system located under the skateboard or at the back of the skateboard unlike the in-wheel motor system where the motor is invisible. With this system, many components may need to be replaced after many uses. (Belt, Pulley, Motor). This system can be composed of one or two motors that can be modified, changed and improved.

| Component | Item Specifications |
| --- | --- |
| Motor | The motor must be a brushless motor. The power can vary and be calculated according to the desired maximum speed. The motors can be purchased on different specialized sites (https://www.mboards.co/collections/electric-skateboard-motors) or suppliers such as aliexpress.  The most common motors for electric skatboard projects are almost 200Kv brushless motors. The use of two motors instead of one does not increase the maximum speed but allows a faster speed increase |
| Belt | The belt seize depend your pulley, your mount and your wheel gear. It need to be purchased and you can’t do it yourself. Available in several sites and in all sizes like here : https://www.mboards.co/collections/pulleys-and-mounts |
| Motor Pulley | Can be Printed in 3D if the motor is not too heavy and the speed not too high. If you print it, do not use PLA and use a heat resistant material such as carbon filament. https://www.thingiverse.com/thing:2337126 Can be purchased on differents sites like here : https://www.mboards.co/collections/pulleys-and-mounts |
| Wheel Pulley | The size varies according to the diameter of your wheel. Can be Printed in 3D. If you print it, do not use PLA and use a heat resistant material such as carbon filament. https://www.thingiverse.com/thing:2337126 Can be purchased on many sites like here : https://www.mboards.co/collections/pulleys-and-mounts |
| Motor Mount | Can be Printed in 3D. If you print it, do not use PLA and use a heat resistant material such as carbon filament https://www.thingiverse.com/thing:2429445/files Can be purchased on many sites like here : https://www.mboards.co/collections/pulleys-and-mounts |

### In-Wheel Motors

The motor is directly integrated to the rear wheels. This system is more aesthetic because you can't see the engine. However, the rear wheels are more complicated to change and the engine can be complicated to change in case of breakage or to improve without changing the whole wheel.
The use of two In-Wheel motors is preferable for this system unlike the pulley-motor which can be satisfied with a single motor.

| Component | Item |
| --- | --- |
| In-Wheel Motor | Can be found in many colors and seizes on differents sites like here : http://www.diyeboard.com/hub-motor-8352mm-450w-75kv-for-diy-electric-skateboard-p-536.html?zenid=ka8sls2lth4h54md18q2bsi2i0 |

## Electronic

Some electronic is required to use the electric skateboard. 

| Component | Item |
| --- | --- |
| ESC | Electronic Speed Controller. The most common board is a pre-built vESC board or simple ESC Board for E-Skateboards. This board can be build with a raspberry pi or an Arduino but it’s more complex to realize. The ESC depends of the battery capacity and motors. |
| Battery | The most common battery used is LiPo cells with 5000mAh minimum. The battery can be composed by multiple cells and it’s indicated with a number and the letter “s” or “p” (Serie or Parallel connection) . Prefer the battery with the most cells. |
| Controller | A lot of ESC boards have a controller provided. However, you can buy some differents controllers, build yours or just take a video game console controller (like the wii nunchuck). You can find many communication protocol used by controllers. 2.4GHz Radio, Wired, Bluetooth or Wifi. |

### ESC

Electronic Speed Controller. This board regulates the electricity emitted by the batteries to change the speed of the skateboard according to the signal emitted by the remote control. It is a composant that tends to heat up and needs to be cooled.

You need to choose one and be careful about the battery and motors support.
There are many ESC solutions :

- vESC with vesc software
- ESC Board
- Arduino with ESC circuit
- Raspberry Pi with ESC circuit

**vESC**

They are most professional boards and use a specific software but are very expensives. They are not too complex to use and have a big users community.

**ESC Boards**

They are like the vESC board but with a different software and hardware. They are not too expensive.

**Arduino and Raspberry ESC**

They are very complex to use, you need to write code and be sure he work. It can be dangerous to use a code if you’re not sure about it. But with this solution, the skateboard is completly personnalised and open source.
If you use it, you need an ESC circuit. It's just a circuit board that controls the power of the battery according to the data sent by the Arduino or the Raspberry pi.

You can find some projects with arduino and raspberry pi like these :
- [https://www.youtube.com/watch?v=2WLEur3M8Yk&t=1s](https://www.youtube.com/watch?v=2WLEur3M8Yk&t=1s)
- https://www.youtube.com/watch?v=cYdv3y90FEM&t=616s

### Battery

It’s LiPo Battery. They need to be 5000mAh (Or 5Ah) and almost 20V to 40V. They can be purchased pre-built or you can do it yourself with some little LiPo cells.

The cells form several cell packs and are connected in series or in parallel. It is indicated by a letter (”s” or “p”) after a number that indicates the number of cells.

Prefer the Li-Po battery with the hightest capacity and with the most cells.

### Controller

The controller control the speed of the skateboard. There are several types of them you can purchase but you can build your own.

The communicate with the ESC with Radio, Bluetooth, Wires or sometimes Wifi. 
You can use every controller like Xbox controller or Wiimote to control your skateboard and some peoples have build their own and publicate their work on web.

You can find some projects with arduino and raspberry pi like this:
- https://www.youtube.com/watch?v=ik0lJ54-LWc

# Software
