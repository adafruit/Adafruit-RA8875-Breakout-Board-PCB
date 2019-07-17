## Adafruit RA8875 Driver Board for 40-pin TFT Touch Displays - 800x480 Max PCB

<a href="http://www.adafruit.com/products/1590"><img src="assets/1590.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit RA8875 Driver Board for 40-pin TFT Touch Displays - 800x480 Max. Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/1590

### Description

Have you gazed longingly at large TFT displays - you know what I'm talking about here, 4", 5" or 7" TFTs with up to 800x480 pixels. Then you look at your Arduino. You love your Arduino (you really do!) but there's no way it can control a display like that, one that requires 60Hz refresh and 4 MHz pixel clocking. Heck, it doesn't even have enough pins. I suppose you could move to ARM core processors with TTL display drivers built in but you've already got all these shields working and anyways you like small micros you've got.

What if I told you there was a driver chip that could fulfill those longings? A chip that can control up 800x480 displays, and heck, a resistive touchscreen as well. All you need to give up is 5 or so SPI pins. Would you even believe me? Well, sit down because this product may shock you.

The RA8875 is a powerful TFT driver chip. It is a perfect match for any chip that wants to draw on a big TFT screen but doesn't quite have the oomph (whether it be hardware or speed). Inside is 768KB of RAM, so it can buffer the display (and depending on the screen size also have double overlaying). The interface is SPI with a very basic register read/write method of communication (no strange and convoluted packets). The chip has a range of hardware-accelerated shapes such as lines, rectangles, triangles, ellipses, built in and round-rects. There is also a built in English/European font set (see the datasheet section 7-4-1 for the font table) This makes it possible to draw fast even over SPI.

The RA8875 can also handle standard 4-wire resistive touchscreens over the same SPI interface to save you pins. There's an IRQ pin that you can use to help manage touch interrupts. The touchscreen handler isn't the most precise driver we've used, so we broke out the X/Y pins so [you can connect them up to something like the STMPE610 which is a very classy touchscreen controller](http://www.adafruit.com/products/1571).

On the PCB we have the main chip, level shifting so you can use safely with 3-5V logic. There is also a 3V regulator to provide clean power to the chip and the display. For the backlight, we put a constant-current booster that can provide 25mA or 50mA at up to 24V. The connector to the screen is a classic '40 pin' connector. All the 40-pin TFT's in the Adafruit shop are known to work well. There are other 40-pin displays that have different pinouts or backlight management and these may not work - they may even damage the driver or TFT if the boost converter pushes 24V into the display logic pins! For that reason, we only recommend the displays we've tested and sell here.

Each order comes with an assembled, tested RA8875 breakout and a stick of header. You'll also need to purchase a 40-pin TFT screen. We currently have 4.3", 5.0" and 7.0" screens available.

To get you started we've written a graphics library that handles the basic interfacing, drawing and reading functions. [Download the Adafruit RA8875 library from github](https://github.com/adafruit/Adafruit_RA8875) and [install as described in our tutorial](http://learn.adafruit.com/adafruit-all-about-arduino-libraries-install-use). Connect a 40 pin TFT to the FPC port and wire up the SPI interface to an Arduino as described in the example code. Once started you'll be able to see the graphic/text demo and then touch the screen to 'paint'. For more advanced details on what the RA8875 can do (and it can do a lot) check the datasheet.



RA8875 Driver Board for 40-pin TFT Touch Displays - 480x800 Max ([11:54](https://www.youtube.com/watch?v=PsfHcXO7IAI#t=714))

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional details.
