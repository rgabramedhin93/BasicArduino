# Basic-Arduino
I'm going to learn how to use an Arduino, and make awesome things with it!


## TableofContents
* [TableOfContents](#TableOfContents)
* [HelloArduino](#HelloArduino)
* [FiniteLEDBlink](#FiniteLEDBlink)

## HelloArduino

### Description & Code

```C++

  // the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(8, OUTPUT);
  Serial.begin(9600); // Turns on the Serial Monitor
  Serial.println("Hello World");
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(8, HIGH);   // turn the LED connected to 8th pin ON (HIGH is the voltage level)
  Serial.print("Blink")
  ;delay(250);            // wait for a second( Values are given in milli seconds)
  digitalWrite(8, LOW);    // turn the LED connected to 8th pin OFF by making the voltage LOW
  delay(250);  // wait for a second  // random comment for no reason...

```

### Evidence
[Here is my code on Arduino Create](https://create.arduino.cc/editor/rgabram93/2ebb0876-0cbd-45a0-ace6-d89d85620de8)

### Image or Wiring
![alt text](image.jpg)
### Reflection


## FiniteLEDBlink

### Description & Code

```C++
Code Goes Here
```

### Evidence

### Image or Wiring

### Reflection
