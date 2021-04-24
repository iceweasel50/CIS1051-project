https://youtu.be/gL9847Nnqwk

#include <Servo.h>
unsigned long startTime=0;
Servo servo_9;
int offset =.2;
void setup() {
  Serial.begin(9600);
  pinMode(A0, INPUT); 
  servo_9.attach(9);
  servo_9.write(80); 
  delay (10000);
}
void loop() {
  int volt = analogRead(A0);
  double voltage = map(volt,0,1023, 0, 2500); 
  voltage /=100;
  Serial.print("Voltage: ");
  Serial.print(voltage);
  Serial.println("V");
  Serial.println(millis());
  
  if (voltage  >= 11.3){
  startTime= millis();
  
  ## The main challenge that I faced while working on this project was learning C while it was similar to python there were some differences in how I had to write out fuctions and loops. 
  ## the most time consuming part of this project by far was getting the logic correct that would open the switch only after the voltage had dropped down below 11.3 for 5 or more seconds. my inital thought was to use an if else statement. I used a seried of if else statements with delays between each but I found that the delay function compleatly stoped everything and it would immediately open the switch after 5 seconds. I needed the switch to open if it was consitantly under 11.3 volts for 5 seconds. this is because the voltage can fluctuate alot in a car unddr normal conditions and I didnt want the switch to open if it jumped down to 10 volts for a split second. So this was afailsafe that was vital to the BMS working well. additionally upon strting the vehicle the voltage drops down to around 6 or 7 volts and i didnt want it to prevent the car from starting. to acheive this i learned about the millis function in arduino. and the millis function just continously counts up. I had the arduino store the last time the voltage was above 11.3 volta and then subtract that from the current time. and used an if statement to see if that time was greater then or equal to 5 seconds. 
  ## over all i had accomplished what i set out to do, however there are som improvements that I would like to make in the future. I want to add a current sensor and a temperature sensor. with theese two additional probes i would be able to tell the state of charge of the battery and could obtain more information about the battery. alos i would like to get an arduino max which has the capibility of connecting to the internet so the user could see alll of the vitals and control the switch from their smartphone. 
