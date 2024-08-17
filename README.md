# Long Range Fixed Wing Autonomous Blood Delivery UAV

## Problem Statement
Over 12,000 people a day in India die due to the unavailability of blood. Many regions, especially remote and rural areas, lack adequate medical infrastructure. More than 40 districts in India do not have a single blood bank. [1] During natural disasters, transporting medical supplies becomes one of the greatest challenges, often requiring hard-to-access manned helicopters.

## Proposed Solution
We propose a “Long Range Fixed Wing Autonomous UAV” (Unmanned Aerial Vehicle) designed for efficient, long-distance delivery of blood and medical supplies. Unlike rotary-wing drones, our fixed-wing UAV can fly for extended periods and carry heavier payloads over greater distances. This UAV will be equipped with an autonomous navigation system and a parachute delivery mechanism to ensure safe and precise delivery of packages to inaccessible or disaster-stricken areas.

## Goals and Objectives
•	Develop a reliable UAV capable of long-range autonomous flights.

•	Ensure timely and efficient delivery of blood and medical supplies to remote and disaster-affected areas.

•	Enhance the accessibility of critical medical resources, reducing mortality rates due to the unavailability of blood.

•	Demonstrate the viability of using fixed-wing UAVs for humanitarian and medical logistics

## Target Audience
The primary beneficiaries of our solution are:

•	Healthcare providers in remote and rural areas.

•	Government and non-governmental organizations involved in disaster relief and medical logistics.

•	Patients in need of urgent blood transfusions and other critical medical supplies.

## Key Features
•	Long-Range Flight Capability: Designed to cover distances up to 100 kilometers, ensuring access to hard-to-reach areas.

•	High altitude flights: Electric BLDC motors with higher thrust can be used to deliver packages in high altitude hard to access locations.

•	Good Payload Capacity: Capable of carrying medical supplies, including blood units and essential medications.

•	Autonomous Navigation: Equipped with GPS and advanced flight control systems for autonomous operation.

•	Parachute Delivery System: Ensures safe and precise delivery of packages to the ground.

•	STOL Capabilities: Built to take off and land in small spaces with hand launch and hand catch ability.

•	Emergency Stall Parachute: With the use of Barometric altimeter and accelerometer we can detect when the aircraft go below stall speed and deploy parachute to save the aircraft and the valuable medical supplies

## Technical Approach
•	Hardware: Fixed-wing UAV for enhanced flight efficiency and range. Equipped with high-capacity batteries and efficient propulsion systems.

•	Navigation: Equipped with high accuracy accelerometer and gyroscope with Global positioning system.

•	Software: Autonomous flight software utilizing GPS for navigation and real-time flight adjustments.

•	Communication: Utilizes NRF24L01 transmitter and receiver for manual control of aircraft.

•	Delivery Mechanism: Parachute-based delivery system for accurate and safe delivery of medical supplies.

## Expected Outcomes
We anticipate our solution will:

•	Significantly reduce the time required to deliver critical medical supplies to remote areas, potentially saving thousands of lives.

•	Demonstrate the feasibility and advantages of using fixed-wing UAVs for medical logistics.

•	Enhance disaster response capabilities, providing rapid delivery of necessary medical supplies during emergencies.

•	Establish a scalable model that can be expanded to other regions and types of deliveries, promoting broader adoption of UAV technology in humanitarian efforts.

## Flight Control System Circuit Diagram
<img width="960" alt="airplane" src="https://github.com/Nahusha-Karnam/UAV/assets/171113429/55928915-8055-4a60-b7ec-269788314793">

## Transmitter Circuit Diagram
<img width="960" alt="newcontroller" src="https://github.com/Nahusha-Karnam/UAV/assets/171113429/7cd8e6f4-9f3e-43ba-bc33-8198c901aacb">

## Flight Control System Table of Connections

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
| D4 | Ch-3 Elevator |
| D2 | Ch-2 Aileron |
|  | Ch-5 Auto Pilot |
| D7 | Ch-6 Trap Door|

## Controller Table of Connections

| Arduino Nano | NRF24L01 |
|--------------|----------|
| 3v3 | VCC |
| GND | GND |
| D10 | CSN |
| D9 | CE |
| D11 | MOSI |
| D12 | MISO |
| D13 | SCK |

| Arduino Nano | Rudder & Throttle | Elevator & Aileron | Auto Pilot Switch | Trap Door Switch |
|--------------|-------------------|--------------------|--------------------|------------------|
| 5v | VCC | VCC | VCC | VCC |
| GND | GND | GND | GND | GND |
| A0 | Ch1 | | | |
| A1 | Ch2 | | | |
| A2 | | Ch3 | | | 
| A3 | | Ch4 | | |
| A6 | | | Ch5 | |
| A7 | | | | CH6 |

## Demo Video Which got us selected

https://github.com/user-attachments/assets/30eadac0-eaff-4c48-af29-2e90603a495c

Video Quality is low because GitHub only allows files within 10 Mb

## Wireless Communication

https://github.com/Nahusha-Karnam/UAV/assets/171113429/bdf43c5f-93cd-4553-adfd-113b4b87b375


## Barometric Altimeter

https://github.com/Nahusha-Karnam/UAV/assets/171113429/54cc1e7e-d0cd-4dd8-a8cf-ac373413a564

## Conclusion
The “Long Range Fixed Wing Autonomous Blood Delivery UAV” project aims to revolutionize the delivery of critical medical supplies in India by leveraging advanced UAV technology. By addressing the significant challenge of inaccessible healthcare in remote areas, this solution has the potential to save thousands of lives and improve the overall efficiency of medical logistics. Through rigorous testing, strategic partnerships, and a focus on scalability, our project will demonstrate the transformative impact of fixed-wing UAVs in humanitarian efforts. This innovation not only enhances current medical supply chains but also sets a precedent for future advancements in autonomous delivery systems worldwide.

## Future Work
•Partner with local healthcare providers and emergency response teams to identify high-need areas and optimize delivery routes.

•	Conduct rigorous testing to validate the UAV's performance and reliability in various conditions.

•	Seek regulatory approval and compliance to operate UAVs within the targeted regions.

•	Can be partnered with Indian Post to deliver more faster and efficient postal services with in any city.

•	With improved motor power and hard body design can be used in agricultural fields being less time consuming and cheaper than manpower.

•	Large-scale seeding can be implemented to accelerate afforestation efforts.

•	Making it capable in all weather conditions.

By leveraging advanced UAV technology, our project aims to address a critical public health challenge and improve the overall resilience of medical supply chains in India

## Reference
[1] https://www.newindianexpress.com/cities/delhi/2019/Jul/15/tracking-every-drop-of-donated-blood-2004103.html#:~:text=%22Every%20day%2012%2C000%20people%20in,have%20a%20single%20blood%20bank.



