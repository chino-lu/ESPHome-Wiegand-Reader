<!DOCTYPE html>
<html>
<head>
</head>
<body>
<h1>ESPHome Wiegand Reader for Garage Keypad 🔑</h1>

<h2>Overview 🏠</h2>
<p>This ESPHome configuration sets up a D1 Mini board to read Wiegand data from a keypad 🔢 and send the scanned tags to Home Assistant 🏡.</p>

<h2>Hardware 🛠️</h2>
<ul>
<li>ESP8266 D1 Mini development board ⚡</li>
<li>Wiegand keypad (connected to D1 and D2 pins) 🔌</li>
<li>Power supply (5V) 🔋</li>
</ul>

<h2>Installation 🚀</h2>
<ol>
<li><strong>Install ESPHome:</strong> Follow the official ESPHome installation instructions: [invalid URL removed]</li>
<li><strong>Create a new project:</strong> Use the ESPHome CLI to create a new project directory. 📁</li>
<li><strong>Copy configuration:</strong> Replace the placeholder values (SSID, password, etc.) in the provided ESPHome configuration file with your specific details. 📝</li>
<li><strong>Flash the device:</strong> Use the ESPHome CLI to flash the compiled firmware to your D1 Mini board. 🔥</li>
</ol>

<h2>Configuration ⚙️</h2>
<p>The provided ESPHome configuration includes the following components:</p>
<ul>
<li><strong>ESP8266:</strong> Specifies the board type. 🖥️</li>
<li><strong>Logger:</strong> Enables logging for debugging purposes. 🐛</li>
<li><strong>API:</strong> Enables the Home Assistant API for communication. 🤖</li>
<li><strong>OTA:</strong> Enables Over-the-Air updates for the device. 📡</li>
<li><strong>WiFi:</strong> Configures WiFi connection and a fallback hotspot. 🌐</li>
<li><strong>Captive Portal:</strong> Provides a captive portal for WiFi configuration. 🔗</li>
<li><strong>Wiegand:</strong> Defines the Wiegand reader, connected to pins D1 and D2. On tag scan, a lambda function is triggered to send the tag data to Home Assistant. RFID</li>
</ul>

<h2>Home Assistant Integration 🏠</h2>
<p>This project relies on the Home Assistant integration to handle the received tag data. You will need to create automations or scripts in Home Assistant to process the tag information and perform desired actions (e.g., open garage door 🚗, trigger alarms 🚨).</p>

<h2>Customization 🔧</h2>
<ul>
<li><strong>WiFi credentials:</strong> Replace `YOUR_SSID` and `YOUR_PASSWORD` with your WiFi network credentials. 📶</li>
<li><strong>OTA password:</strong> Set a strong password for OTA updates. 🔒</li>
<li><strong>Fallback hotspot password:</strong> Set a password for the fallback hotspot. 🔑</li>
<li><strong>Wiegand reader pins:</strong> Adjust the `d0` and `d1` pins if your keypad is connected differently. 🔌</li>
<li><strong>Home Assistant integration:</strong> Customize the lambda function or create additional components to handle the tag data as needed. 🤖</li>
</ul>

<h2>Troubleshooting 🛠️</h2>
<ul>
<li><strong>Verify wiring:</strong> Ensure the Wiegand keypad is correctly connected to the D1 and D2 pins. 🔌</li>
<li><strong>Check power supply:</strong> Make sure the board is receiving adequate power. 🔋</li>
<li><strong>Enable logging:</strong> Use the logger component to troubleshoot issues. 🐛</li>
<li><strong>Review ESPHome documentation:</strong> Refer to the official ESPHome documentation for detailed explanations and troubleshooting tips. 📚</li>
</ul>

<h2>Additional Notes 📝</h2>
<ul>
<li>The provided configuration is a basic example. You may need to add additional components or modify the existing ones based on your specific requirements. 🏗️</li>
<li>Consider using more descriptive names for components and variables to improve code readability. 👓</li>
<li>For security reasons, it is recommended to use strong passwords for WiFi and OTA. 🔒</li>
</ul>

<p>By following these steps and customizing the configuration to your needs, you should be able to successfully set up your ESPHome Wiegand reader for garage keypad control. 🚗🔑</p>

</body>
</html>
