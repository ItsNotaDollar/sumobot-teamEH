#**master Code Info**

The master arduino should be in control of the overall function of the robot. 

###Set Up
Set up code starts by getting an initial sensor reading so that we can precompute where the opponent is and then starts the **5 second**.
<!--Add in screen shot of code here to get nice syntax highlighting instead of code tag-->
```
void setup() {
	
}
```

###Main Loop
The main loop has a very basic implementation, seek & destroy. Each loop we will read from the sonar sensors and determine how to adjust where its going. If an interrupt is triggered then it will read the data from the sensors and adjust accordingly.
<!--Add in screen shot of code here to get nice syntax highlighting instead of code tag-->
```
void loop() {

}
```

###Pins in Use
| Pin           | Function                     |
|:-------------:|:----------------------------:|
| in A0         | Left Sonar Sensor            |
| in A1         | Right Sonar Sensor           |
|               |                              |
| in D0         | Front Left QRD bit           |
| in D1         | Front Right QRD bit          |
| in D2         | Back Left QRD bit            |
| in D3         | Back Right QRD bit           |
| in D4         | Front Pressure Sensor bit    |
| in D5         | Back Pressure Sensor bit     |
|               |                              |
| RX            | QRD Interrupt                |
| TX            | Pressure Sensor Interrupt    |