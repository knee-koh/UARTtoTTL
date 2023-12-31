# UARTtoTTL Adapter Board
PCB to convert UART signals to TTL with level shifting in order to communicate with Dynamixel motors.

<img src="Media/Gifs/DynamixelClose1.gif" width=90% />
<p float="left" align="center">
	<img src="Media/Images/V1 PCB.JPG" width=45% />
	<img src="Media/Images/V1 Components.JPG" width=45% />
</p>

##Usage:
1. Downlaod the .zip file from the V1 folder, and upload it directly to a PCB printing service. Install the ICs, Level Shifter, and Dynamixel connectors according to the markings on the silk screen.
2. Attach the Dynamixel Voltage to VCC and GND pins
3. Attach 5V and 3V from your microcontroller (a Teensy was used for testing with the Dynamixel2Arduino library) to control the logic levels
4. Attach the TX, RX, and DIR pins according to how your code is configured

##V1 BOM:
- (12X) [2.54mm spacing header pins](https://www.amazon.com/MCIGICM-Header-2-45mm-Arduino-Connector/dp/B07PKKY8BX/ref=sr_1_5?crid=2B0UKD4FHHPAV&keywords=header+pins&qid=1703965345&sprefix=header+pi%2Caps%2C143&sr=8-5) - Use two 6-pin rows for the Level Shifter and the remaining 7-pins for the input pins, if desired.
- (1X) [Level Shifter](https://www.amazon.com/HiLetgo-Channels-Converter-Bi-Directional-3-3V-5V/dp/B07F7W91LC/ref=sr_1_3?crid=2UK39K6IAPTMH&keywords=level+shifter&qid=1703966291&sprefix=level+shift%2Caps%2C174&sr=8-3)
- (1X) [Hex Inverter (SN74HC14N)](https://www.amazon.com/Bridgold-SN74HC14N-Schmitt-Trigger-Inverters-DIP-14/dp/B0983ZXJFZ/ref=sr_1_3?crid=1BJWQIMZNLUQZ&keywords=SN74HC14N&qid=1703964695&s=industrial&sprefix=sn74hc14n%2Cindustrial%2C157&sr=1-3)
- (1X) [Buffer (SN74HC125N)](https://www.amazon.com/Pieces-SN74HC125N-Logic-Gates-DIP-14/dp/B0C746GFZQ/ref=sr_1_2?crid=2A1WBHEH1MIIR&keywords=SN74HC125N&qid=1703964843&sprefix=sn74hc125n%2Caps%2C149&sr=8-2)
- (1X) [Molex 0532530370](https://www.digikey.com/en/products/detail/molex/0532530370/965997)
- (1X) [Molex 0022035035](https://www.digikey.com/en/products/detail/molex/0022035035/403302)  
- (1X) [JST B3B-EH-A](https://www.digikey.com/en/products/detail/jst-sales-america-inc/B3B-EH-A/926521)

##Optional:
- (2X) [14-pin DIP socket (2.54mm spacing)](https://www.amazon.com/uxcell-2-54mm-Soldering-Socket-Adaptor/dp/B07H3WQYRQ/ref=sr_1_8?crid=DGJEVV0V7XPY&keywords=dip+socket&qid=1703965150&sprefix=dip+socke%2Caps%2C154&sr=8-8) - Use these to make the ICs removable
- (12X) [Female Pin Header socket (2.54mm spacing)](https://www.amazon.com/Hxchen-2-54mm-Straight-Single-Headers/dp/B07VBYD2C3/ref=sr_1_7?crid=1WUWCIGXKZBAN&keywords=header+socket&qid=1703965065&sprefix=header+socke%2Caps%2C153&sr=8-7) - Use two 6-pin sockets to make the Level Shifter removable
- (7X) [2.54mm spacing header pins](https://www.amazon.com/MCIGICM-Header-2-45mm-Arduino-Connector/dp/B07PKKY8BX/ref=sr_1_5?crid=2B0UKD4FHHPAV&keywords=header+pins&qid=1703965345&sprefix=header+pi%2Caps%2C143&sr=8-5) - Place on the input pins on the left-hand side of the board.
