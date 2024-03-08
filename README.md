code:
// the setup routine runs once when you press reset:
void setup() {
  // initialize serial communication at 9600 bits per second:
  Serial.begin(9600);
  // initialize digital pin LED_BUILTIN as an output.
}

// the loop routine runs over and over again forever:
void loop() {
  // read the input on analog pin 0:
  int knobValue = analogRead(A0);
   // print out the value you read:
  Serial.println(knobValue);

  if(analogRead(0) >= 400)
  {
    digitalWrite(2, HIGH);
  }
  else
  {
    digitalWrite(2, LOW);
  }

}
