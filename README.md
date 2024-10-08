# DIY Weather Station

This tutorial will guide you through setting up a system to measure and track humidity and temperature levels. You'll use the DHT11 sensor to gather data, the NodeMCU to process it, and ThingSpeak to store and visualize the information online.

## Hardware

| S.No | Components Name       | Quantity |
| ---- | --------------------- | -------- |
| 1    | NodeMCU ESP8266 Board | 1        |
| 2    | DHT11 Sensor          | 1        |
| 3    | Jumper Cables         | 3        |
| 4    | Breadboard            | 1        |
## Software Requirements

1. Download the [Arduino IDE](https://support.arduino.cc/hc/en-us/articles/360019833020-Download-and-install-Arduino-IDE)
2. Install Drivers for ESP8266

		'http://arduino.esp8266.com/stable/package_esp8266com_index.json'
		
	1. Copy the above path.
	2. Open your Arduino IDE.
	3. File > Preferences > Additional boards manager URLs.
	4. To add another URL code, seperate the existing URL with a comma.
	5. Tools > Board > Boards Manager.
	6. Search for esp8266 and install esp8266 by ESP8266 Community.

3. Search for the DHT Sensor library by Adafruit and Install it.

### ESP8266 Pin Out


![ESP8266 PinOut](https://github.com/gowshi0212/WeatherStation/blob/ce0d975bee8f4204550cda13907ed7cda86d887a/Images-WS/Pasted%20image%2020240925072929.png)


### DHT11 Humidity and Temperature Sensor


![DHT11 Pin Out](https://github.com/gowshi0212/WeatherStation/blob/ce0d975bee8f4204550cda13907ed7cda86d887a/Images-WS/Pasted%20image%2020240925073053.png)


### Circuit Diagram


![Circuit Diagram](https://github.com/gowshi0212/WeatherStation/blob/ea62318ade5669902c9af51a25ee087e3645b278/Images-WS/Pasted%20image%2020240925072533.png)



### Getting Started with Thingspeak

1. Go to [Thingspeak](https://thingspeak.com/) and create an account if you do not have one. Login to your account.  
2. Create a new channel by clicking on the button. Enter the basic details of the channel. Then Scroll down and save the channel. 
	- You will need two channels, one for Humidity and one for Temperature
3. Then go to API keys copy the 'Write API Key' and paste this key to a separate notepad file. You will need it later while programming.
### MQTT Protocol

![MQTT](https://github.com/gowshi0212/WeatherStation/blob/ce0d975bee8f4204550cda13907ed7cda86d887a/Images-WS/Pasted%20image%2020240925080608.png)

Visit this website to learn more -> https://mqtt.org/

### Coding Tasks

Task 1: Connect the ESP8266 to Wifi

Task 2: Try getting values from DHT11

Task 3: Connect to thingspeak
