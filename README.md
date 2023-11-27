# pushbutton-led-

int ledPin = 16;
int buttonPin =4;

void setup()
{
  pinMode(ledPin,OUTPUT);
  pinMode(buttonPin,INPUT_PULLUP);
}

void loop()
{
  int digitalVal = digitalRead(buttonPin);
  
  if(HIGH == digitalVal)
  {
    digitalWrite(ledPin,LOW);
  }
  else
  {
    digitalWrite(ledPin,HIGH);
  }
}
