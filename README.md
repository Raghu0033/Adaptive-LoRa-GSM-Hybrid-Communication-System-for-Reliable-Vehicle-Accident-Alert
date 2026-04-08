# Adaptive-LoRa-GSM-Hybrid-Communication-System-for-Reliable-Vehicle-Accident-Alert
Adaptive LoRa &amp; GSM Hybrid Communication System for Reliable Vehicle Accident Alert

#GSM-based Accident Detection System Works
detect Accident with __single sensor value (> Threshold) and GSM based communication__ .


#Working Flow (Step-by-step)
### 1. Accident Detection 
Sensors detect: \
Sudden impact (vibration sensor) \
__High acceleration/deceleration &amp; Vehicle tilt (rollover detection)__ \
If threshold exceeds → accident assumed 


### 2. Location Capture 
GPS module fetches: \
__Latitude &amp; Longitude__ \
This gives exact accident location 


### 3. Decision Logic 
Microcontroller checks: \ 
Is it real accident or false trigger? \
Some systems give 10 seconds delay to cancel alert 
 

### 4. SMS Alert via GSM 
GSM module sends: \
__SMS to family / ambulance / police__ \
Includes: \
Location link (Google Maps) \
Time of accident 




# ⚠️ Limitations 


## 🚫 1. False Positives (Biggest Problem)
Sudden braking / potholes → triggers accident \
Mobile-based systems especially suffer from this

👉 Example: \
Speed breaker → system thinks crash

## 🚫 2. GSM Network Dependency
In remote areas: \
No signal → no SMS sent \
Communication failure = system useless

👉 Research clearly mentions weak GSM signal issue


## 🚫 3. No Real-Time Monitoring
SMS is: \
Store-and-forward system \
Not continuous tracking

👉 No live updates like:

Fail to get GPS Coordinates \
Use Previous Coordinates and Communicate with Direction of Coordinates.

## 🚫 4. No Communication Between Vehicles
Only sends SMS to humans \
Does NOT: \
Warn nearby vehicles \
Prevent secondary accidents
