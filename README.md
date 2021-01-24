# tasmota-pir-case
* Learn Tasmota with ESP32 and a PIR sensor

## PIR
HC-SR501 - sensor för rörelsedetektering

Pinout

### Läge H
Jumper settings
Det finns två verioner av HC-SR501
* Utan jumper pins - Läge H är standard.
* Med jumper pins - Välj läge H/L med jumper

<figure class="image"><img src="https://lastminuteengineers.com/wp-content/uploads/arduino/PIR-Sensor-Retriggering-Repeat-Mode-Jumper-Setting.png" alt="H - Hold-Repeat-Retrigger mode"><figcaption>H - Utgången fortsätter vara H så länge rörelse är detekterad (källa - https://lastminuteengineers.com/pir-sensor-arduino-tutorial/)</figcaption></figure>

### Läge L

<figure class="image"><img src="https://lastminuteengineers.com/wp-content/uploads/arduino/PIR-Sensor-Non-Retriggering-No-Repeat-Mode-Jumper-Setting.png" alt="L No-Repeat mode/non-retrigger mode"><figcaption>L - Utgången är hög under perioden för TIME (källa - https://lastminuteengineers.com/pir-sensor-arduino-tutorial/)</figcaption></figure>

## Tasmota

* Tasmota är ett robust monitorprogram för alla ESP8266- och ESP32(beta)baserade enheter
* Tasmota är ett webbaserat GUI som kommunicerar med hjälp av WiFi och har direktstöd för MQTT, Serial och/eller Domotics
* Fungerar med utvecklingskort och t.ex. SONOFF's produkter men också många mer (https://templates.blakadder.com/)
* Tasmota tillåter HTTP kontroll - kommandon via URL
* Tasmota 

## Installera Tasmota på ESP8266

## Installera Tasmota på ESP32

## Tethering to WiFi

## Konfigurera Tasmota

## Tasmota Mallar (templates)

tasmota esp32 vill ha 36 i template

org
ESP32-DevKit
{"NAME":"ESP32-DevKit","GPIO":[1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,0,1,1,1,0,1,1,1,0,0,0,0,1,1,1,1,1,0,0,1],"FLAG":0,"BASE":1}

{"NAME":"ESP32 DEVKIT V1 (36pins)","GPIO":[416,0,418,0,417,2720,0,0,2624,32,2656,224,0,0],"FLAG":0,"BASE":45}
{"NAME":"WT-ESP32-CAM","GPIO":[4992,1,1,1,1,5088,0,0,1,1,1,1,1,0,5089,5090,0,5091,5184,5152,0,5120,5024,5056,0,0,0,0,4928,0,5094,5095,5092,0,0,5093],"FLAG":0,"BASE":2}
{"NAME":"AITHINKER CAM","GPIO":[4992,1,1,1,1,5088,1,1,1,1,1,1,1,1,5089,5090,0,5091,5184,5152,0,5120,5024,5056,0,0,0,0,4928,1,5094,5095,5092,0,0,5093],"FLAG":0,"BASE":1}
{"NAME":"WT32-ETH01","GPIO":[1,1,1,1,1,1,0,0,1,0,1,1,3840,576,5600,0,0,0,0,5568,0,0,0,0,0,0,0,0,1,1,0,1,1,0,0,1],"FLAG":0,"BASE":1}
in tasmota esp32
{"NAME":"ESP32-DevKit","GPIO":[1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,0,1,1,1,0,1,1,1,0,0,0,0,1,1,1,1,1,0,0,1],"FLAG":0,"BASE":1}
mine
0 ,1,2  ,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,21,22,23,25,26,27,32,33,34,35,36,39 (20, 24, 28, 29, 30, 31, 37, 38 not exist)
32,0,288,0,1,1,0,0,0,0,0 ,0 ,0 ,1 ,1 ,1 ,1 ,1 ,1 ,1 ,1 ,1 ,1, 1 ,1 ,1 ,1 ,1 ,0 ,0 ,0 ,0 

0 ,1,2  ,3,4,5,9,10,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,39 (20, 24, 28, 29, 30, 31, 37, 38 not exist)
32,0,288,0,1,1,0,0 ,0 ,1 ,1 ,1 ,1 ,1 ,1 ,1 ,0, 1 ,1 ,1, 0, 1 ,1 ,1 ,0 ,0 ,0, 0, 1 ,1 ,0 ,0 ,0 ,0 

GPIO0 - Button Boot
GPIO2 - Led Builtin
0 ,1,2  ,3,4,5,9,10,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39
32,0,288,0,1,1,0,0 ,0 ,1 ,1 ,1 ,1 ,1 ,1 ,1 ,0 ,1 ,1 ,1 ,0 ,1 ,1 ,1 ,0 ,0 ,0 ,0 ,1 ,1 ,0 ,0 ,0 ,0 ,0 ,0

32,0,288,0,1,1,0,0,0,1,1,1,1,1,1,1,0,1,1,1,0,1,1,1,0,0,0,0,1,1,0,0,0,0,0,0


{"NAME":"ESP32 DEVKIT V1 (36pins)","GPIO":[32,0,288,0,1,1,0,0,0,0,0,0,0,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,0,0,0,0],"FLAG":0,"BASE":18}

## 
