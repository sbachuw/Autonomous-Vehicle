#include <Servo.h>

Servo ssm;
Servo esc;

int steering = 90, velocity = 90;

void setup()  {
  ssm.attach(10);
  esc.attach(11);
}


void loop() {
  setVehicle(45, 90);
  delay(2000);
  setVehicle(135, 45);
  delay(2000);

}

void setVehicle(int s, int v)
{
  s = min(max(0, s), 180);
  v = min(max(75, v), 105);
  ssm.write(s);
  esc.write(v);
}

