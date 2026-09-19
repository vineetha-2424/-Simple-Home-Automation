int button1 = 2;
int button2 = 3;

int light = 8;
int fan = 9;

void setup() {
  pinMode(button1, INPUT);
  pinMode(button2, INPUT);

  pinMode(light, OUTPUT);
  pinMode(fan, OUTPUT);
}

void loop() {

  if (digitalRead(button1) == HIGH) {
    digitalWrite(light, HIGH);
  } else {
    digitalWrite(light, LOW);
  }

  if (digitalRead(button2) == HIGH) {
    digitalWrite(fan, HIGH);
  } else {
    digitalWrite(fan, LOW);
  }
}
# -Simple-Home-Automation
