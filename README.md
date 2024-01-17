# EE-Fundamentals-Lab
const int analogPin = 34; // Change this to the pin you're using

void setup() {
  Serial.begin(115200);
}

void loop() {
  int adcValue = analogRead(analogPin);


  float voltage = (adcValue / 4095.0) * 3.3;

  
  Serial.print("Voltage: ");
  Serial.print(voltage);
  Serial.println(" V");

  delay(1000);
}
