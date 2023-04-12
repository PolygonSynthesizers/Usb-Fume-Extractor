# Usb-Fume-Extractor
This is a USB powered (5v) PWM Computer Fan Controller


Please read until the end!


This fume extractor is made with a 120 mm PWM (4pin) 12V PC Fan. 
You can use any 12V PC Fan as long as the power consomption doesn't exceed 500mA over 12V.
It has to be a 12V fan as the power supply is converting 5V USB to 12V. 24V Fans won't work.

I personally use a Noctua NF-F12 industrialPPC-3000 PWM and it can blow air 
along 6 meter of 80mm aluminium duct even at half speed.



You can control the speed of rotation via the potentiometer around 10 to 90% of the fan full speed.
It works with a 556 chip (which is two 555 timers in DIP 14 pins package) which produce a 5V square pulse
with pulse width modulation (it's how fan speed is controlled on a computer).



You can't power this circuit with a computer USB port. It doesn't have enough power. You have to power it with
a USB Power Supply like a Phone Charger for example. It has to be rated for 1 amp over 5V at a minimum. 

Connect the charger to the board via a USB A to USB A cable or a USB A to USB B cable (Printer cable). 
About the length : the shorter is the better.  



Some references :

* U1 is a NE556 in DIP14 package
* The inductor is a 10 uH Fastron 242408 FPS
* U2 is a LM2731 XMF in SOT-23 package
* R1 and R2 are 0805
* CF1 is 0805
* C1 is 1210
* C2 is 1812
* D1 is .5 amps Schottky Rectifier in SOD-123 package
* All through hole resistors are 1/4W
* All through hole capacitors are 5mm pitch film capacitors
* Except for C7 which is a 2mm pitch aluminium electrolytic.
* RV1 is a Alps Alpine RK09K113 10k Linear (Log can also work but control over speed will not be linear).
* SW1 is a 3 pin SPDT switch with 4.7mm pitch between pins. I has to be rated for 1A at least.

For values you can check the BOM under the bom folder. Values are also on the schematics.

All SMDs can be handsoldered. Start with the LM2731XMF.



This project has been made with KiCad 7.01. You may have to install the latest version of KiCad
for this project to work.
I have made some custom footprints for the switch, the inductor and the film capacitors.
They can be found under the Custom Footprints folder.

Gerbers are available for JLCPCB production under the Gerbers folder. 
Please make your own gerbers if you want to use an other PCB Manufacturer.



I'm providing some 3D files that can be modified on Solidworks. STL Files are also provided so you can print
them on your 3D printer. The rear body of the Fan has been made for 80mm duct. 
Feel free to modifiy it at your own conveniance.
It uses standard M4 screws for the body and M3 screws for the PCB holder.
Files can be found under the 3D Files folder. I will provide some 3d files for the base 
and the PCB front cover later. 
Don't be scared to make your own.

PLEASE DON'T TURN ON THE FAN WITHOUT THE 3D PRINTED FRONT AND REAR BODY PART ATTACHED TO IT !
IT CAN CUT OUT YOUR FINGERS VERY EASILY !
I WON'T TAKE ANY RESPONSABILITY FOR ANY DAMAGE, MATERIAL OR PHYSICAL. YOU HAVE BEEN WARNED !



ENJOY !
