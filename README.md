# Task 2-Electrical-and-electronic-power
This repository contains two subtasks:
- [On off system](https://github.com/Abdullah98h/Task2-electrical-and-electronic-power/tree/main/On%20off%20system)
- [Forward kinematics & inverse kinematics](https://github.com/Abdullah98h/Task2-electrical-and-electronic-power/tree/main/Forward%20kinematics%20and%20inverse%20kinematics)
## On off system
In this task I made an electronic circuit that consists of the folloiwng components:
- Small Signal nMOS Transistor
- 10 kβ¦ Resistor
- 30 , 5 Power Supply
- DC Motor
- Diode
- Arduino Uno R3
- Pushbutton1 
- kβ¦ Resistor

Arduion code:
```
// C++ code
//
#define mosfetGate 6
#define pushButton 2

void setup()
{
  pinMode(mosfetGate, OUTPUT);
  pinMode(pushButton, INPUT);

}

void loop()
{
  int buttonState = digitalRead(pushButton);
  if(buttonState==1){
  	digitalWrite(mosfetGate, HIGH); //turn on the motor
  }
  else{
  	digitalWrite(mosfetGate, LOW); //turn off the motor
  }
}
```
This circuit enable the auto shutdown by the arduino, the motor will rotate only when the pushbutton clicked, otherwise the motor will never rotate.

------------------------------------

## Forward kinematics & inverse kinematics
In this task I draw a robot arm with a 3 DOF, then I applied the forward kinematics and the inverse kinematics to find angle measures and (x, y) point.
- Inverse kinematics:
    - The given data: (x, y) = (50, 30)
    - The calculations:
   
    > Pythagoras theorem:
    > 
    > π^π= π^π+π^π 
    > 
    > π^π= γππγ^π+γππγ^π 
    > 
    > π=β(γππγ^π+γππγ^π)
    > 
    > π=ππ.ππ
    > 
    > L1 and L3 are equal 21.21
    > 
    > πππ π½=πΆπππππππ/π―πππππππππ
    > 
    > πππ π½=ππ/(ππ.ππ)
    > 
    > π½=ππππππ ππ/(ππ.ππ)
    > 
    > π½=ππ.ππΒ°
    > 
    > π½1 and π½2 are equal 45.01
    > 
    > π½π=πππβ (ππ.ππ+ππ)
    > 
    > π½π=ππ.ππΒ°
    > 
    > π½π=ππ.ππ+ππ
    > 
    > π½π=πππ.ππ Β°
    > 
    > π½π=πππβπππ.ππ
    > 
    > π½π=  45.01 Β°
    > 
    > π½π  and π½π are equal 45.01 Β°

   
    - The solution:
    
    >  L1= 21.21
    >  
    >  L2= 20
    >  
    >  L3=21.21
    >  
    >  π½1= 45.01Β°
    >  
    >  π½π= 45.01Β°
    >  
    >  π½π= 45.01Β°


- Forward kinematics:
    - The given data: 
    
    L1= 12
    
    L2= 15
    
    L3= 18
    
    π½π=ππΒ°
    
    π½π=ππΒ°
    
    π½π=ππ

    - The calculations:
      > X= (L1 cos π½π)+π³π+"(L3 cos " π½π)
      > 
      > Y= (L1 sin π½π + L3 sin π½π)
      >
      >  X= (12 cos ππ)+ππ+"(18 cos " ππ)
      >  
      >  X= 38.75
      >  
      >  Y= (12 sin ππ + 18 sin ππ)
      >  
      >  Y= 18.02

  - The solution:
      >  (x,y)= (38.75, 18.02)
  -----------------------

