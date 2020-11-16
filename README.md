# Not_so_basic_aurduino
## C++
### Blink Revisted
#### Assignment
Creat a version of LED_Blink, but it dradually goes up in brightness and back down in brightness.
#### Code
int ledPin = 5;
int x = 0;

void setup() {
  Serial.begin(9600);
  pinMode(ledPin, OUTPUT);

}

void loop() {
  for (x = 0; x < 255; x++) {
  Serial.println(x);
    analogWrite(ledPin, x);

    delay (25);
  }
  for (x = 255; x > 0; x--) {
  Serial.println(x);
    analogWrite(ledPin, x);

    delay (25);
}
}
### Reflection 
This was a one of the harder assignments this year due to forgetting how to do Aurduino code. At first it was alright but then I had to make it gradullay increase and decrease, I had the code down I was just not putting the wire in the right pin that could be used with analog write.
