# BasicArduino
I'm going to learn how to use an Arduino, and make awesome things with it!


## TableofContents
* [TableOfContents](#TableOfContents)
* [HelloArduino](#HelloArduino)
* [FiniteLEDBlink](#FiniteLEDBlink)
* [VariableLEDBlink](#VariableLEDBlink)
* [ButtonActivatedLED](#ButtonActivatedLED)

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

### Description & Code
The Variable LED Blinker is when you make the LED blink but every second it gets faster and faster. You have to use a new variable called delayVar. Since you know that 1000 milliseconds equals 1 second, you would have to do minus 100 after the delayVar so the LED can get faster.

```C++
/* Karl Helmstetter
variable LED BLink
This should blink an LED faster and faster, until it reaches 5 blinks per second
*/

int ledPin = 8;
int delayVar = 1000;  //this variable is used for my delays.

void setup() {
  pinMode(ledPin,OUTPUT);    
}

void loop() {
    digitalWrite(ledPin, HIGH);           // turn the LED on (HIGH is the voltage level)
    delay(delayVar);                       // wait for a second
    digitalWrite(ledPin, LOW);            // turn the LED off by making the voltage LOW
    delay(delayVar);                       // wait for a second
    Serial.println(delayVar);
    delayVar = delayVar - 100;
    
    //as long as the delay is longer than 100 ms, we should continue to blink,
    // and we should also 
}
```

### Evidence
[Here is my code on Arduino Create](https://create.arduino.cc/editor/rgabram93/f6526129-7bb6-47d5-9727-540a27ceaf62)
### Image or Wiring
![alt text](https://raw.githubusercontent.com/rgabramedhin93/BasicArduino/main/Screenshot%202020-11-23%20at%204.18.49%20PM.png)
### Reflection
This assignment is a really cool one. The LED gets faster each time which makes it look cool. Nothing really changed in the wiring other than changing the wire to pin 8 to light the LED.


## ButtonActivatedLED

### Description & Code
In this assignment we had to wire up an LED and use a pushbutton to make the LED blink. Once you press the button the LED starts blinking and once you let go it turns off.
```C++
int buttonPin = 2; // Pin connected to PushButton                                                                       
int ledPin = 13; // Pin connected to LED
int buttonState = 0; // Gives pushbutton a value

void setup() {
  
  pinMode(ledPin, OUTPUT); // Sets LED pin as an output
  pinMode(buttonPin, INPUT); // Sets pushbutton pin as an input
}

void loop() {
  buttonState = digitalRead(buttonPin); // Reads input from pin 2
  if(buttonState == HIGH) { // If pushbutton is pressed, set as high
    digitalWrite(ledPin, HIGH); // Turn on LED
  }
  else{
    digitalWrite(ledPin, LOW); // Otherwise turn off LED
  }
  }
```

### Evidence
[Here is my code on Arduino Create](https://create.arduino.cc/editor/rgabram93/14482634-3e11-4d00-87e6-d0dcc1a53768)
### Image or Wiring
![alt text](https://raw.githubusercontent.com/rgabramedhin93/BasicArduino/main/button%20LED-1.jpg)
### Reflection
This assignment was kind of hard for me, I had trouble trying to make the right code for this but it ended up working out for me. Looking forward to the next assignment!
