# Program-4-Servo
The code 
#include <Servo.h>

int pos = 0;
Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;


void setup()
{
  servo1.attach(9);
  servo2.attach(10);
  servo3.attach(11);
  servo4.attach(12);

}

void loop()
{
  
  for (pos = 0; pos <= 180; pos += 1) {
    servo1.write(pos);
    delay(5);
  }
  for (pos = 180; pos >= 0; pos -= 1) {
    servo1.write(pos);
    delay(5);  
  }
  for (pos = 0; pos <= 180; pos += 1) {
    servo2.write(pos);
    delay(10);
  }
  for (pos = 180; pos >= 0; pos -= 1) {
    servo2.write(pos);
    delay(10);  
  }
  for (pos = 0; pos <= 180; pos += 1) {
    servo3.write(pos);
    delay(15);
  }
  for (pos = 180; pos >= 0; pos -= 1) {
    servo3.write(pos);
    delay(15);  
  }
  for (pos = 0; pos <= 180; pos += 1) {
    servo4.write(pos);
    delay(20);
  }
  for (pos = 180; pos >= 0; pos -= 1) {
    servo4.write(pos);
    delay(20);  
  }
}
