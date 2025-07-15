# Home-Automation-IOT
#define BLYNK_TEMPLATE_ID "YourTemplateID"
#define BLYNK_TEMPLATE_NAME "HomeAutomation"
#define BLYNK_AUTH_TOKEN "YourAuthToken"

#include <ESP8266WiFi.h>
#include <BlynkSimpleEsp8266.h>

char auth[] = "YourAuthToken";
char ssid[] = "YourWiFiName";
char pass[] = "YourWiFiPassword";

void setup() {
  Blynk.begin(auth, ssid, pass);
  pinMode(D1, OUTPUT);
  pinMode(D2, OUTPUT);
}

BLYNK_WRITE(V1) {
  digitalWrite(D1, param.asInt()); // Light
}

BLYNK_WRITE(V2) {
  digitalWrite(D2, param.asInt()); // Fan
}

void loop() {
  Blynk.run();
}
