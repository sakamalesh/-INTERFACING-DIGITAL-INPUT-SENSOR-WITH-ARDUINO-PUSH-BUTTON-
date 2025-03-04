## INTERFACING DIGITAL INPUT SENSOR WITH ARDUINO PUSH BUTTON
## DATE :15-02-24
## NAME : KAMALESH S																	             
## ROLLNUMBER :212223040083
## DEPARTMENT COMPUTER SCIENCE ENGINEERING


## AIM:
To interface a digital input (push button) and blink and LED upon activation.
## COMPONENTS REQUIRED:
1.	1 KΩ Resistor 
2.	Arduino Uno 
3.	Bread board 
4.	USB Interfacing cable 
5.	Jumper wires 
6.	LED of choice 
## THEORY :
Arduino UNO
 	  The Uno is a microcontroller board based on the ATmega328P. It has 14 digital input/output pins (of which 6 can be used as PWM outputs), 6 analog inputs, a 16 MHz quartz crystal, a USB connection, a power jack, an ICSP header and a reset button. It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with a AC-to-DC adapter or battery to get started.
	Technical specifications of Arduino UNO :
Microcontroller	ATmega168/328
Microcontroller	ATmega168/328
Operating Voltage	5V
Input Voltage (recommended)	7-12V
Input Voltage (limits)	6-20V
Digital I/O Pins	14 (of which 6 provide PWM output)
Analog Input Pins	6
DC Current per I/O Pin	40 mA
DC Current for 3.3V Pin	50 mA
Flash Memory	16 KB (ATmega168) or 32 KB (ATmega328) of which 2 KB used by boot loader
SRAM	1 KB (ATmega168) or 2 KB (ATmega328)
EEPROM	512 bytes (ATmega168) or 1 KB (ATmega328)
Clock Speed	16 MHz
## PIN DIAGRAM FOR ATMEGA 328
 
![image](https://user-images.githubusercontent.com/36288975/163530394-115baee4-7ed1-49fe-9cce-d7b625e11e85.png)

FIGURE-01
![image](https://user-images.githubusercontent.com/36288975/163530431-4d390e98-0942-42d8-95b8-f57d348e6ad8.png)

FIGURE-02
## PROCEDURE 
 Open tinker cad account 
1.	Select Arduino uno , bread board , digital input and digital output 
2.	Connect the circuit as given in the figure 
3.	Develop the program and compile it for any errors 
4.	 .Execute the program 
5.	Check the simulation 



## CIRCUIT DIAGRAM 


![Screenshot 2024-02-15 110628](https://github.com/sakamalesh/-INTERFACING-DIGITAL-INPUT-SENSOR-WITH-ARDUINO-PUSH-BUTTON-/assets/149148235/2a8a423a-86fc-432a-bb4e-dc500d4969e1)

![Screenshot 2024-02-15 110845](https://github.com/sakamalesh/-INTERFACING-DIGITAL-INPUT-SENSOR-WITH-ARDUINO-PUSH-BUTTON-/assets/149148235/6c754801-0fda-4a0f-a497-ed248cf66873)


FIGURE -03




## PROGRAM 
 
 int led=4;
int pushbutton=3;

void setup()
{
  pinMode(led, OUTPUT);
  pinMode(pushbutton, INPUT);
}

void loop()
{
  int pb;
  pb= digitalRead(pushbutton);
  if(pb==HIGH)
{


  digitalWrite(led, HIGH);
  delay(500); 
  digitalWrite(led, LOW);
  delay(500); 
}
else
{
  delay(500); 
  digitalWrite(led, LOW);
  
}
}









 
 
 



## OUTPUT OF SIMULATION :

![Screenshot 2024-02-15 110628](https://github.com/sakamalesh/-INTERFACING-DIGITAL-INPUT-SENSOR-WITH-ARDUINO-PUSH-BUTTON-/assets/149148235/2a8a423a-86fc-432a-bb4e-dc500d4969e1)

![Screenshot 2024-02-15 110845](https://github.com/sakamalesh/-INTERFACING-DIGITAL-INPUT-SENSOR-WITH-ARDUINO-PUSH-BUTTON-/assets/149148235/6c754801-0fda-4a0f-a497-ed248cf66873)


