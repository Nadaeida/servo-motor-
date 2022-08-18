# servo-motor-

The steps of servo motor is:
The supply of the motor must be connected ( 5V and ground GND) First, Create a funtion to power servo motors after that declare the angle of motors rotation then, give a signal to the motors and this signal is from pin 13 from the arduino uno r3 then do a for loop to control of motor rotation. if the angle of rotation is from 0 to smaller than or equal 180, the motors rotates in counterclockwise direction for 15 millisecond. if the angle of rotation is equal to 180 to greater than or equal to 0, the motors rotates in clockwise for 15 millisecond.

the code :
// C++ code

//
#include<Servo.h>
Servo servoequiv;
int pos = 0;
void setup()
{
  servoequiv.attach(13);  //because I have connected signal pin with 13
  
}

void loop()
{
  // rotate from 0 to 180 degree
  for(pos=0;pos<=180;pos++)
  {
    servoequiv.write(pos);
    delay(15);
  }
  for(pos=180;pos>=0;pos--);
  {
    servoequiv.write(pos);
    delay(15);
  }
}
About brushless motor :
1- connecting the wires like the circuit:
![brushless](https://user-images.githubusercontent.com/108246979/185383218-28adf9c7-718e-409f-9f22-29d90033c2c9.png)

![brushless2](https://user-images.githubusercontent.com/108246979/185383289-9c0fd79b-8486-405b-bfa9-fc546e656cbd.png)

2-step2:Run the brushless motor:
https://user-images.githubusercontent.com/108246979/185382480-92838a7a-9625-4ee3-94b0-01157e739734.mp4


