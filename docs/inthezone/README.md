# in the Zone
Garmin Connect IQ Zone Training App

This App has been written specifically for cycling devices that can handle the newer Connect IQ and device firmware.  It includes many new features and configuration options, particularly display of current weather conditions and a localised (depending on GPS) forecast for the next 3 hours.


**REQUIREMENTS:**

** This data field requires a power meter, HeartRate monitor and cadence sensor to be connected to your Garmin device. **

** There is also a configuration option to display the rear cassette gear, which requires electronic shifting on your bike, linked with your Garmin device. **

** Your data recording interval should be set to 1 second in your Garmin device. That is, not using Smart Recording, and you should TURN OFF auto-pause. Normalised Power and Strava Weighted Power calculations require these settings for accuracy. **


See Screen shots, below, for details regarding information and layout.


**INFORMATION DISPLAYED:**

- Battery Status indicator - Battery Level: 75-100% Green, 50-75% Blue, 20-50% Orange, less than 20% Red, Level checked every 20 mins and then every 5 mins once below 10%
- Current Power Watts (with a configurable 1-30 second moving average)
- Average Power, Strava Weighted Average (SWA) Power, or Normalized Power (NP).  If NP is chosen you may also choose to display Intensity Factor (IF) and Training Stress Score (TSS).
- Option to display Power (and Average Power/SWA/NP) as Watts/Kg
- Watt Prime Balance (See below)
- Power & Average Power Zone (See below)
- HeartRate & Average HR Zone
- Cadence (RPM).  Average Cadence may also be displayed if NP (IF and TSS) is not displayed.
- Speed, Average Speed and Distance (Kilometres or Miles, depending on Garmin profile)
- Gradient %
- Current Altitude (Metres or Feet, depending on Garmin Profile)
- Current Time and Timer display.  Configuration allows on/off display of seconds
- Rear Cassette gear (configurable on/off). Front Chain Ring is also highlighted by showing first digit of Cassette gear in Blue if smaller chainring selected, or second digit of cassette gear in blue if larger chainring seleted.
- Optional diplay of Weather (N/A on Bontrager 1030):  Current conditions plus a Forecast of next 3 hours.  This display is configurable to display all the time, every minute, for 2 minutes, 4 minutes or 8 minutes.  The weather can update every 20 minutes, or by clicking the LAP button, or both (this is configurable).  Weather information provided by GPS.  If precipitation is 50% chance or greater for a weather forecast, the forecast row will be a Blue colour.  Weather condition icons automatically adjust depending on sunrise and sunset.
- Configurable colour of outlines in the display.
- Configurable position of all four circles, plus the extra data display.  That is, each primary metric can be moved to a different circle and the extra data display can be placed either top or bottom of screen.
- Configurable display of 60 second histograms for HeartRate, Power and/or Both.
- In The Zone can only be used as a single field display in an Activity page.  


**POWER ZONES (Coggan - FTP based):**

- Z1 = Less than 56% (Recovery - Grey)
- Z2 = 56 - 75% (Endurance - Blue)
- Z3 = 76 - 90% (Tempo - Green)
- Z4 = 91 - 105% (Threshold - Orange)
- Z5 = 106 - 120% (Vo2Max - Red)
- Z6 = 121 - 150% (Anaerobic - Pink)
- Z7 = 151 - MAX% (Neuromuscular - Purple)
- Z2 - Z7 are configurable in the App (MAX is derived). *The app displays the percentage your power is within the respective zone.*


**HR ZONES:**

- Are automatically retrieved from your Garmin profile, so please ensure they are setup correctly there.
- If you are planning to display Power as Watts/KG, please also ensure you set your correct weight in your Garmin profile.
- *The app displays the percentage your HR is within the respective zone.*


**Watt Prime (W') BALANCE:**

An App setting lets you choose between the W Prime Balance DIFFERENTIAL calculation (Froncioni and Clarke - App default, which recovers quicker when power dips below threshold) or the INTEGRAL (Default) calculation (Skiba, et al.). Either setting requires 2 settings - Functional Threshold Power (FTP) and W Prime (in Joules). If your W' Balance goes negative (a breakthrough occurred) the app will automatically adjust your W PRIME and record it in Settings.

- The Watt Prime circle will display in Blue for values 50-100%, Orange for values 20-50% and Red for less than 20%.
- For a Breakthrough (WP less than zero) it will be the colour purple.
- Set W' to zero if not required.


**Watt PRIME (W') AUTO DECAY:**

The app can track when you last did an activity and automatically decay your W Prime setting by a daily percentage. You can set a decay of between 0.1% and 2.5% (between 1 and 25 in App Settings). Example, if my WPrime is 20000 and I set a decay of 5 (equating to 0.5%), then each day of inactivity, my W Prime will decay by 0.5% (in this case, 100J) of the current value. It checks the last activity date and calculates the the new WPrime each App start. If you don't want your W Prime to automatically decay, set the decay to zero (default setting).


**In The Zone is based on my other apps: TrainingPower & TrainingHR.**


# What’s New

**v1.0.1:**
- Initial Release (New combined version - with new configuration options and features - of two of my apps: TrainingPower and TrainingHR).

