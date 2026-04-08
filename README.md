# Adaptive-LoRa-GSM-Hybrid-Communication-System-for-Reliable-Vehicle-Accident-Alert
Adaptive LoRa &amp; GSM Hybrid Communication System for Reliable Vehicle Accident Alert

#GSM-based Accident Detection System Works
detect Accident with __single sensor value (> Threshold) and GSM based communication__ .


#Working Flow (Step-by-step)
### 1. Accident Detection
Sensors detect:
Sudden impact (vibration sensor)
__High acceleration/deceleration &amp; Vehicle tilt (rollover detection)__
If threshold exceeds → accident assumed


### 2. Location Capture
GPS module fetches:
__Latitude &amp; Longitude__
This gives exact accident location


### 3. Decision Logic
Microcontroller checks:
Is it real accident or false trigger?
Some systems give 10 seconds delay to cancel alert


### 4. SMS Alert via GSM
GSM module sends:
__SMS to family / ambulance / police__
Includes:
Location link (Google Maps)
Time of accident
