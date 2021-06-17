# TrainingPower
Garmin Connect IQ TrainingPower App

When I'm training I'm particularly focussed on monitoring Power and ensuring I'm sitting in particular zones. I wanted a single data field that could display everything I needed to know, related to power.


**REQUIREMENTS:**

** This data field requires a power meter and cadence sensor to be connected to your Garmin device. **

** There is also a configuration option to display the rear cassette gear, which requires electronic shifting on your bike, linked with your Garmin device. **

** Your data recording interval should be set to 1 second in your Garmin device. That is, not using Smart Recording, and you should TURN OFF auto-pause. Normalised Power and Strava Weighted Power calculations require these settings for accuracy. **


See Screen shots, below, for details regarding information and layout.


**INFORMATION DISPLAYED:**
  (depending on device and screen configuration)

- Display certain metrics as Bars (default) or Circles.  Unfortunately (due to memory constraints) the Edge520 device cannot display in circles mode.
- Battery Status indicator for Edge and Watch devices (except for Edge 520/130, Fenix 5/5x/6) Battery Level: 75-100% Green, 50-75% Blue, 20-50% Orange, less than 20% Red, Level checked every 20 mins and then every 5 mins once below 10%
- Current Power Watts (with a configurable 1-30 second moving average)
- Average Power, Strava Weighted Average (SWA) Power, or Normalized Power (NP) (option to also display as W/Kg).  If NP is chosen you may also choose to display Intensity Factor (IF) and Training Stress Score (TSS), but only in 1 & 2 field layouts (Edge 130/130+/520+/820/530/830); 1,2 & 3 field layouts (Edge 1000); 1,2, 3A, 3B, 4B, 5B, 6B & 7B layouts (Edge 1030) in Circles mode.
- Watt Prime Balance (See below)
- Power Zone (See below)
- Average Power Zone (See below)
- Cadence (RPM)
- Average cadence (RPM)
- Speed, Average Speed and Distance (Kilometres or Miles, depending on Garmin profile)
- Gradient %
- Rear Cassette gear (for supported devices). Front Chain Ring is also highlighted on Edge 530/830/1000/1030x devices in circles display mode.


**POWER ZONES (Coggan - FTP based):**

- Z1 = Less than 56% (Recovery - Grey)
- Z2 = 56 - 75% (Endurance - Blue)
- Z3 = 76 - 90% (Tempo - Green)
- Z4 = 91 - 105% (Threshold - Orange)
- Z5 = 106 - 120% (Vo2Max - Red)
- Z6 = 121 - 150% (Anaerobic - Pink)
- Z7 = 151 - MAX% (Neuromuscular - Purple)
- Z2 - Z7 are configurable in the App (MAX is derived). The app displays the percentage your power is within the respective zone.


**Watt Prime (W') BALANCE:**

An App setting lets you choose between the W Prime Balance DIFFERENTIAL calculation (Froncioni and Clarke - App default, which recovers quicker when power dips below threshold) or the INTEGRAL calculation (Skiba, et al.). Either setting requires 2 settings - Functional Threshold Power (FTP) and W Prime (in Joules). If your W' Balance goes negative (a breakthrough occurred) the app will automatically adjust your W PRIME and record it in Settings.

- The Watt Prime bar (or circle) will display in Blue for values 50-100%, Orange for values 20-50% and Red for less than 20%.
- For a Breakthrough (WP less than zero) it will be the colour purple.
- Set W' to zero if not required.


**Watt PRIME (W') AUTO DECAY:**

The app can track when you last did an activity and automatically decay your W Prime setting by a daily percentage. You can set a decay of between 0.1% and 2.5% (between 1 and 25 in App Settings). Example, if my WPrime is 20000 and I set a decay of 5 (equating to 0.5%), then each day of inactivity, my W Prime will decay by 0.5% (in this case, 100J) of the current value. It checks the last activity date and calculates the the new WPrime each App start. If you don't want your W Prime to automatically decay, set the decay to zero (default setting).


**TrainingPower is designed to be used in two-field screen layouts with my other App - TrainingHR.**


# What’s New

**v1.8.8:**
- Remove useUpdateInterval function which was a yes/no setting that allowed the app to only update the Power display every interval (1-30 seconds depending on setting) as it causes issues in settings when updating the App
- Code optimizations to better support Fenix5 and Forerunner 935

**v1.8.7:**
- Add new Circles mode Layouts: Layout 4A (Edge 530/830), Layout 3 (Edge 820) and Layouts 3A, 3B, 4B, 5B, 6B, 7B (Edge 520+)

**v1.8.6:**
- NEW: Display IF (Intensity Factor) and TSS (Training Stress Score) via App setting BUT only when Normalized Power (NP) Averaging has also been set.  Please note, IF and TSS are only available in 1 & 2 field layouts (Edge 130/130+/520+/820/530/830); 1,2 & 3 field layouts (Edge 1000); 1,2, 3A, 3B, 4B, 5B, 6B & 7B layouts (Edge 1030)
- FIX:  Improve the smoothing speed and reactivity of the Filter for the calculation of Gradient (all devices)
- Optimise 2 field layout for the Edge1030 device to make it consistent with other layouts

**v1.8.5:**
- FIX:  If your power output matched your zone 7 power and also matched your maximum power for the activity, the app would crash
- FIX:  WPrime balance could show a large negative number in certain situations - such as, high power output for long periods during a long activity
- Support the new Garmin AntiAlias feature on supported devices.  With this, graphics are rendered more smoothly, when drawing circles and angular lines
- Add FTP setting to the in-app settings function, for supported devices

**v1.8.4:**
- Add optional (through app settings) battery status indicator for Edge and Watch devices (except for Edge 520/130, Fenix 5/5x/6) Battery Level: 75-100% Green, 50-75% Blue, 20-50% Orange, less than 20% Red - Level checked every 20 mins and then every 5 mins once below 10%.
- Added New Circles Mode B for Edge devices (except Edge520/130) - Displays Watt Prime as the bar within the left, main Power circle and Average Power (whichever calculation you chose) as the right, large circle.
- Power Zone calculation optimisations

**v1.8.3:**
- No longer need to supply a Maximum Power setting in App Properties, this is now derived.

**v1.8.2:**
- NEW: Getting ready to support "In App Settings" (that is, not having to use Garmin Connect or your phone to change App settings). This is currently device firmware dependent, to which Garmin does not provide advice on which devices will receive firmware updates or when updates will be made available. Currently, only the Fenix6, D2 and MARQ devices have the firmware to support this functionality. I'm hopeful the Edge devices (at least some) will soon too. Once a device receives a firmware update that supports in app settings, Training Power "In App Settings" will just start working.
- NEW: W Prime Automatic decay (via App Setting)
- Support for new Forerunner 745 device
- Improve efficiency of drawing circles and ARCs
- Improve accuracy of Strava Weighted Average and Normalized Power calculations
- Remove App specific LAP function (from All devices except: original Edge 520, original Fenix5 and FR935) as Garmin and Strava do this better

**v1.7.5.2:**
- Fix: Distance display now follows the units selected in your Garmin Profile (Metric or Imperial)

**v1.7.5.1:**
- Fix: TrainingPower can only support 1 and 2 field layouts on on Fenix5, Fenix6 and FR935 specific devices due to memory constraints.
- Highlight downhill gradient green in Edge devices using Circles mode.

**v1.7.5.0:**
- Increase the font size in use for Average Power and Average Cadence in Circles view on supported Edge devices.
- Compiled under v3.2.1 of Connect IQ SDK

**v1.7.4.0:**
- Added Settings option to display Normalized Power (isoPower) All supported devices except original Edge 520, FR935 and Original Fenix5. Normalized power will only begin to display 30 seconds after an activity starts.
- Standardize colours used to be from 64 colour pallette (except Edge130, which is only Black and White)
- Fix an issue with W/Kg calculation on Average Power

**v1.7.3.0:**
- Added support for Edge 130/130+ with the following caveats: 1) There are no colours, black and white only - as such the datafield now displays the Power Zones (as numbers - "PowerZone : AvgPowerZone"); 2) There is no support for di2 (so no di2 gears will be displayed); and 3) The datafield only suppoprts circles mode.
- Remove superfluous Power Z1 setting from App settings.
