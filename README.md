# Z-Scale-Decoder

### A ultra tiny DCC decoder build for Z scale trains using the universal DCC protocoll at 10V

<img width="1285" height="805" alt="Screenshot 2026-11-08 at 22 20 37" src="https://github.com/user-attachments/assets/cff1420b-77f3-4e2c-a87a-108216320c2e" />
<img width="920" height="692" alt="Screenshot 2026-11-08 at 22 20 52" src="https://github.com/user-attachments/assets/79533e68-6b99-4641-a918-b2ef942e58b5" />

## Why this exists
All Z-scale trains on the market today are analog meaning they have poor slow speed performance as the motor jolts to life to get it going. They are also limited to only 1 train per track loop.
My DCC decoder is meant to bridge this gap and fit in larger locomotives and the Rokuhan® "Shorties" carriages to allow for precise pwm motor control with back EMF detection, multiple trains per loop, and optional rgb LED for dynamic running lights.  

## What it does

* ATtiny826 8-bit AVR MCU base running a DCC decoder
* Runs straight from DCC track power, up to 10 V
* Bridge rectifier, (So it works with either track polarity)
* DRV8220 H-bridge motor driver for high compatibility
* Back-EMF speed regulation 
* Optional directional front and rear lights plus an optional cab light
* TPS70950 5 V LDO 
* UPDI programming pads  
* 12 x 7.5 mm
* 2-layer board,0201 componets

## Version History
* 0.1
    * Initial release 

## BOM
|Value         |Designator |Footprint     |JLCPCB Part #          |
|--------------|-----------|--------------|-----------------------|
|0.1uF         |C1,C3      |C0201         |C2158829               |
|10uF 25V      |C2         |C1206         |C2158829               |
|2.2uF         |C4         |C0201         |C6204143               |
|1uF           |C5         |C0201         |C307385                |
|PMEG3010AESBYL|D1,D2,D3,D4|D0402         |C28646369              |
|220k          |R1         |R0201         |C158699                |
|470           |R2         |R0201         |C144816                |
|47k           |R3,R5      |R0201         |C100140                |
|22k           |R4,R6      |R0201         |C295842                |
|DRV8220DSGR   |U1         |WSON-8(2x2)   |C3681269               |
|TPS70950DRVR  |U2         |WSON-6-EP(2x2)|C527527                |
|ATTINY826-MU  |U3         |VQFN-20(3x3)  |C3216887               |


## Help

Contact author 

## Author

Lucas Klemmer  
klinksolutions22@gmail.com

## License
MIT LIcense

If anyone ends up reproducing this device or making it even bettter I would be happy to see your improvements and add them to the oficial release.
