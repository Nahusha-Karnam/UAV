# Long Range Fixed Wing Autonomous Blood Delivery UAV

## Flight Control System Circuit Diagram
<img width="960" alt="airplane" src="https://github.com/Nahusha-Karnam/UAV/assets/171113429/55928915-8055-4a60-b7ec-269788314793">

## Transmitter Circuit Diagram
<img width="960" alt="newcontroller" src="https://github.com/Nahusha-Karnam/UAV/assets/171113429/7cd8e6f4-9f3e-43ba-bc33-8198c901aacb">


| Arduino Nano | NRF24L01 |
|--------------|----------|
| 3v3 | VCC |
| GND | GND |
| D10 | CSN |
| D9 | CE |
| D11 | MOSI |
| D12 | MISO |
| D13 | SCK |

| Arduino Nano | GPS neo M7 | MPU 6050 | BME280 |
|----------|-----------|----------|------------|
| 5V | VCC | VCC | VCC |
| GND | GND | GND | GND |
|A0 | RX | | |
| A1 | TX | | |
| A2 | | SDA | |
| A3 | | SCL | |
| A4 | | | SCL |
| A5 | | | SDA |

| Arduino Nano | Channel Connections |
|--------------|---------------------|
| D5 | Ch-1 Throttle |
| D3 | Ch-2 Rudder |
| D4 | Ch=3 Elevator |
| D2 | Ch-2 Aileron |
|  | Ch-5 Auto Pilot |
| D7 | Ch-6 Trap Door|



## Wireless Communication

https://github.com/Nahusha-Karnam/UAV/assets/171113429/bdf43c5f-93cd-4553-adfd-113b4b87b375

## Radio Controller

https://github.com/Nahusha-Karnam/UAV/assets/171113429/c3370593-40ad-4e63-9de5-a95092f226b5

## Barometric Altimeter

https://github.com/Nahusha-Karnam/UAV/assets/171113429/54cc1e7e-d0cd-4dd8-a8cf-ac373413a564

## BLDC Motor

https://github.com/Nahusha-Karnam/UAV/assets/171113429/e7094903-fe04-44c8-b0a1-08e37ec09b53


