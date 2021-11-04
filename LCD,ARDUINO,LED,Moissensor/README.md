#include <FastLED.h>
#include <LiquidCrystal.h>

#define NUM_LEDS 60      /* The amount of pixels/leds you have */
#define DATA_PIN 7       /* The pin your data line is connected to */
#define LED_TYPE WS2812B /* I assume you have WS2812B leds, if not just change it to whatever you have */
#define BRIGHTNESS 100   /* Control the brightness of your leds */
#define SATURATION 255   

const int AirValue = 600;   //you need to replace this value with Value_1
const int WaterValue = 350;  //you need to replace this value with Value_2
int soilMoistureValue = 0;
int soilmoisturepercent=0;

CRGB leds[NUM_LEDS];
LiquidCrystal lcd(12, 11, 5, 4, 3, 2);
void setup () {
  FastLED.addLeds<LED_TYPE, DATA_PIN>(leds, NUM_LEDS);  
  Serial.begin(9600); // open serial port, set the baud rate to 9600 bps
  lcd.begin(16, 2);
}

void loop () {
  for (int j = 0; j < 255; j++) {
    for (int i = 0; i < NUM_LEDS; i++) {
      leds[i] = CHSV(i - (j * 2), SATURATION, BRIGHTNESS); /* The higher the value 4 the less fade there is and vice versa */ 
    }
    FastLED.show();
    delay(200); 
  }
 { 
  soilMoistureValue = analogRead(A0);  //put Sensor insert into soil
}
Serial.println(soilMoistureValue);
soilmoisturepercent = map(soilMoistureValue, AirValue, WaterValue, 0, 100);
if(soilmoisturepercent >= 100)
{
  Serial.println("100 %");
  lcd.setCursor(0, 0);
  lcd.print("Soil Moisture");
  lcd.setCursor(0, 1);
  lcd.print("100 %");
  delay(100);
  lcd.clear();
}
else if(soilmoisturepercent <=0)
{
  Serial.println("0 %");
  lcd.setCursor(0, 0);
  lcd.print("Soil Moisture");
  lcd.setCursor(0, 1);
  lcd.print("0 %");
  delay(250);
  lcd.clear();
}
else if(soilmoisturepercent >0 && soilmoisturepercent < 100)
{
  Serial.print(soilmoisturepercent);
  Serial.println("%");
  lcd.setCursor(0, 0);
  lcd.print("Soil Moisture");
  lcd.setCursor(0, 1);
  lcd.print(soilmoisturepercent);
  lcd.print(" %");
  delay(250);
  lcd.clear();/* Change this to your hearts desire, the lower the value the faster your colors move (and vice versa) */
  }
  }
