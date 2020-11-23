# Basic-Arduino
I'm going to learn how to use an Arduino, and make awesome things with it!


## TableofContents
* [TableOfContents](#TableOfContents)
* [HelloArduino](#HelloArduino)
* [FiniteLEDBlink](#FiniteLEDBlink)
* [VariableLEDBlink](#VariableLEDBlink)

## HelloArduino

### Description & Code
This is the code of my Arduino LED blinking. When I put Serial.begin that means it turns on the the Serial Monitor. Then Serial Print Line means each line it is gonna say "Hello World" and this is for the void setup. For the void loop I put down Serial Print without the line which means it will print "Blink" beside each other instead of line by line.
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
![alt text](https://raw.githubusercontent.com/rgabramedhin93/BasicArduino/main/IMG_20201116_160537.jpg)
### Reflection
This is the first assignment where I coded and it is pretty cool! I made the LED blink twice a second so in the code the delay would be 250. Overall it came out good and looking forward for the next assignment the Finite LED Blink

## FiniteLEDBlink

### Description & Code
For this assingment I had to make an LED blink 5 times and stop.

```C++
int ledPin = 13;
int blinkTime = 500;

void setup()
{
  pinMode(ledPin, OUTPUT);
  blinkyBlinky(5, blinkTime); // 5 is number of blinks, blinkTime is the milliseconds in each state from above: int blinkTime = 500;
}

void loop()
{
  //
}

void blinkyBlinky(int repeats, int time)
{
  for (int i = 0; i < repeats; i++)
  {
    digitalWrite(ledPin, HIGH);
    delay(time);
    digitalWrite(ledPin, LOW);
    delay(time);
  }
}
```

### Evidence
[Here is my code on Arduino Create](https://create.arduino.cc/editor/rgabram93/c1b52a36-2070-44e5-81fd-024e30300fb0)
### Image or Wiring
![alt text](https://raw.githubusercontent.com/rgabramedhin93/BasicArduino/main/Screenshot%202020-11-18%20at%204.16.05%20PM.png)
### Reflection
I made an LED blink 5 times. Most of my wiring stayed the same I just changed one of the wires to a new pin. I created the wiring I had on a website called TinkerCAD. Pretty cool seeing it blink 5 times and stopping. Looking forward to the next assingment.

## VariableLEDBlink

### Desceiption & Code

```C++

```
