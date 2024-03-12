# Irrigation Controller powered by Home Assistant and ESPHome Sprinkler Controller integration By Andrea Guarnerio (frieduser)

I’ve done a tailored irrigation system on my needs, leveraging on:
12321

14121qq

•	Esphome sprinkler controller platform
•	Home Assistant Automation
•	Irrigation Dashboard with some HACS addons
•	Single package file with all configurations (input_*, statistics and automation)
I’ve a 4 zones lawn and two other zones: flowerbed and strawberries.

The goals I’ve pursued:
•	Schedule with a time for a single irrigation in the day
•	Frequency in days: every day, every two days and so on
•	Disable a specific day, for example on Saturday if I know I’ll have a barbecue with friends; the irrigation will be done the following day
•	For lawn, that has 4 zones, leveraging on Auto Advance option available in esphome/sprinkler, we can schedule just the lawn, not every single zone

Other options:
•	There’s a system to count rainfall in order to avoid watering (postponed) or decrement irrigation time
•	There’s a flag to enable a zone – or the lawn – to be rain aware for what available in previous point
•	It’s possible to enable/disable scheduler
•	The chance to watering manually
•	Set up irrigation time in minutes with limits (60 min in my setup)

Please see:
•	Lovelace screenshots
o	Irrigation
o	Rain section (with some controls for testing)
o	Maintenance dashboard
•	Notification examples
•	Esphome code (I’ve used POE ESP32 platform)
o	Rain gauge (reed switch to count every tip) has been used with 3.3V/12V Optocoupler – no need to debounce pulses
o	I’ve not used counter integration because I’ve preferred to leverage on home assistant statistics
Happy to answer to your questions.

![alt text](screenshots/hass02.png "Screenshot Example")

- View Example
![alt text](screenshots/hass01.png "Screenshot Example")

