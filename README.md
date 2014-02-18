lcd_display_backlight
=====================

This is a some changes to the previously modified Arduino Library which use SPI to a shift register to control an LCD display from 74HC595 shift register.   The code originally came from the link on this tutorial:-

[http://playground.arduino.cc/Main/LiquidCrystal](http://playground.arduino.cc/Main/LiquidCrystal)

I've modified this to add two extra features:-

	- Added  void setSecondPins(uint8_t secondPins); which allows a second shift register to be added and use the overflow (effectivly shifting 16 bits)
	- Added the backlightOn() and  backlightOff() methods which toggle pin QC on the shift register controlling the display.  I have a MOSFET between the Cathode and Ground.  The QC pin is connected to the gate to toggle the backlight.
	
I will add a blog article and details on makicity.com.
	

