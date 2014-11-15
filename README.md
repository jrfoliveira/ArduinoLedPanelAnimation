ArduinoLedPanelAnimation
========================

Space Invaders and Letters @ Funduino pro mini (Arduino) 8x8 LED panel (MAX7219)

/* SPACE INVADERS and LETTERS Animation for MAX7219 from maxim @ Funduino mini pro (Arduino mini pro clone), 
reduced and optimised for useing more then one 7219 in a row,
______________________________________

 Code History:
 --------------

The orginal code was written for the Wiring board by:
 * Nicholas Zambetti and Dave Mellis /Interaction Design Institute Ivrea /Dec 2004
 * http://www.potemkin.org/uploads/Wiring/MAX7219.txt

First modification by:
 * Marcus Hannerstig/  K3, malmï¿½ hï¿½gskola /2006
 * http://www.xlab.se | http://arduino.berlios.de

Second version is by:
 * tomek ness /FH-Potsdam / Feb 2007
 * http://design.fh-potsdam.de/ 

 * @acknowledgements: eric f. 


This version is by:
 * Juliano R. F. de Oliveira / November 2014
 * email: jrfoliveira@gmail.com
 * @acknowledgements: all previous authors and the below two sites who provide animations for aliens and letters.
 * Letters: Animation Tool for 8x8 LED Matrix http://www.diyode.com/mini8x8/
 * Aliens: Gemma Space Invaders https://learn.adafruit.com/trinket-slash-gemma-space-invader-pendant/animation
-----------------------------------

General notes: 


-if you are only using one max7219, then use the function maxSingle to control
 the little guy ---maxSingle(register (1-8), collum (0-255))

-if you are using more then one max7219, and they all should work the same, 
then use the function maxAll ---maxAll(register (1-8), collum (0-255))

-if you are using more than one max7219 and just want to change something
at one little guy, then use the function maxOne
---maxOne(Max you wane controll (1== the first one), register (1-8), 
collum (0-255))

/* During initiation, be sure to send every part to every max7219 and then
 upload it.
For example, if you have five max7219's, you have to send the scanLimit 5 times
before you load it-- other wise not every max7219 will get the data. the
function maxInUse  keeps track of this, just tell it how many max7219 you are
using.
*/
