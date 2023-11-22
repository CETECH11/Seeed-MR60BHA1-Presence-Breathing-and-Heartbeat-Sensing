# Seeed-MR60BHA1-Presence-Breathing-and-Heartbeat-Sensing

![alt text](https://hackster.imgix.net/uploads/attachments/1651278/_L4AO8VIYup.blob?auto=compress%2Cformat&w=900&h=675&fit=min)

The MR60BHA1 60GHz mmWave Module is a versatile sensor that utilizes Frequency Modulation Continuous Wave (FMCW) detection to accurately measure breathing rate and heart rate, ensuring a completely private and secure environment, free from external interference. Equipped with a built-in standard algorithm and onboard antenna, the unit delivers simultaneous signal output with exceptional precision. It serves as an ideal solution for developing high-accuracy, self-regulating, privacy-protected, and secure biotic radar systems in consumer electronics, healthcare, and industrial applications.

Beyond heart rate and respiration detection, the radar sensor can detect human presence in the operating area, enabling the creation of an automated device and appliance control system that conserves energy during unoccupied periods. Additionally, the system incorporates an IR temperature sensor to measure body temperature, allowing for illness and stress detection. Upon detecting significant vital variations, the buzzer activates as an alert. Simultaneously, all details are displayed on an LCD display and a mobile phone app via the ESP32 Wi-Fi module.

The project involved various components, which can be identified in the Below provided image.

![alt text](https://hackster.imgix.net/uploads/attachments/1647796/radar_heart_rate_vNAKS5zthG.jpg?auto=compress%2Cformat&w=740&h=555&fit=max)

The Seeed Studio MR60BHA1 60GHz mmWave Module is a versatile sensor module that utilizes Frequency Modulation Continuous Wave (FMCW) detection technology to accurately measure vital signs, including breathing rate and heart rate. It operates in a completely private and secure environment, free from external interference, making it an ideal solution for privacy-sensitive applications. Equipped with a built-in standard algorithm and onboard antenna, the unit delivers simultaneous signal output with exceptional precision. It serves as an ideal solution for developing high-accuracy, self-regulating, privacy-protected, and secure biotic radar systems in consumer electronics, healthcare, and industrial applications

Key Features:

Non-contact sensing for comfort and privacy
High-accuracy, self-regulating, privacy-protected, and secure
Low power consumption for extended battery life
Compact size and lightweight for easy integration
Applications:

Consumer Electronics: Smart home automation, wearable devices, sleep monitoring
Healthcare: Patient monitoring, vital signs detection, illness and stress detection
Industrial Applications: Presence detection, safety monitoring, automation control
Additional Features:

IR temperature sensor to measure human temperature
Buzzer to alert when vital variations are found
LCD display and mobile phone app for data visualization

![alt text](https://hackster.imgix.net/uploads/attachments/1647799/image_gfCU50nQrm.png?auto=compress%2Cformat&w=740&h=555&fit=max)

The project comprises an MR60BHA1 60GHz mmWave module for respiration, heart rate, and human presence detection, along with an MLX90614 sensor for contactless body temperature measurement. This project caters to two sectors: wellness monitoring and home or office automation.

The ESP32 microcontroller serves as the project's central processing unit (CPU) and WiFi module. The MR60BHA1 sensor is connected using the ESP32's UART channels and the MLX90614 sensor is connected using ESP32's I2C Channels(SDA, SCL).

To measure body temperature, the user needs to bring their hand near the sensor. A proximity sensor is deployed near the MLX90614 sensor to detect the presence of a hand and initialize the body temperature measurement. The measured temperature details will be displayed on the LCD panels and Blynk mobile application in Celsius units.

To initiate heart rate and respiration rate measurement, the user must first deactivate the human presence detection switch. Once deactivated, the user should press the measurement button, and the ESP32 will initiate the measurement process by emitting a buzzer alert. The algorithms require a few seconds to collect and process the data, so please expect some minor delays before the accurate readings are displayed on the LCD screen and the Blynk mobile application.

To activate the automation system based on human presence, the human presence detection switch must be activated. Once the switch is activated, the MR60BHA1 transitions into human presence detection mode. When human movements are detected within the radar's operating range, the ESP32 sends a pop-up notification to the Blynk app alerting the owner. Subsequently, an LED bulb will be turned on using a relay, demonstrating the MR60BHA1's capability in automating equipment. This human presence detection system also serves as a security product.

The entire project is powered by a 12-volt DC power adapter. Considering the power requirements of the sensors, microcontroller, and other components, the voltage is regulated to 5 volts using a 7805 voltage regulator and to 3.3 volts using an AMS1117 voltage regulator.

![alt text](https://hackster.imgix.net/uploads/attachments/1651031/nextpcb_4r1pEG3pxS.JPG?auto=compress%2Cformat&w=740&h=555&fit=max)

This project was successfully completed because of the help and support from [NextPCB](https://www.nextpcb.com/). Guys if you have a PCB project, please visit their website and get exciting discounts and coupons.

NextPCB offers high-quality, reliable PCB starting at $1.9, and multilayer starting at $6.9. Also, everyone can enjoy free [PCB assembly](https://www.nextpcb.com/) for 5 boards! Also, NextPCB is having a year end sale in which anyone can register through their website and get a $30 Coupon which can be used for ordering PCBs.

You can also try HQDFM free online [PCB Gerber viewer](https://www.nextpcb.com/free-online-gerber-viewer.html) to check your PCB design and avoid costly errors.
