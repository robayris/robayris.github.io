# Radian
Garmin Connect IQ Radian WatchFace

There are a lot of great watch faces on the Garmin app store and I have a few favourites. However, I couldn't find one that had everything I wanted, so I created this one. Key aspects:
1) Displays the battery remaining as the tick marks around the watch face - in a choice of two formats - lines or circles - and choice of colour.

2) Displays a second hand if watch hardware permits (1hz). Second hand can be triggered to stop displaying by making it the same colour as watchface background.

3) Displays 3 dials, one of which can be configured to display Calories (and percentage of calorie target), Altitude, or distance moved today, but also the ability to cycle between these three displays. Dial display cycle will occur every 20 seconds in full-power mode, or every minute in low-power mode. The gauge hand in the dials can be turned off by making it the same colour as the dial background colour.

4) Can be configured to reduce data displayed when in "Do Not Disturb" mode, watch not being worn, or when HR is below resting heart rate (within 5%). By reducing data display in this way, battery life can be conserved during periods when the watch isn't in active use (like, when it's not on your wrist, or you might be asleep). Resting Heart rate comes from your Garmin profile, or if it is not set, then Max HR divided by 3. When configured to reduce display based on resting HR, if you're wearing the watch, your HR needs to be less than Resting HR + 5% for 5 or more minutes. If you're not wearing the watch its 30 seconds.

5) There are 22 different colour settings that can be applied to the watch face, with colours chosen from the available 64 palette colours, as per the attached image. The attached colour palette shows 64 numbered colours. Just enter this number (1-64) into the colour fields in settings. Please be aware that colours on the watch face will not be as vibrant as those in the colour palette, due to the backlight differences between watch and computer.

6) Displays a graph showing your steps history (from left to right, with left being yesterday and the next to the right being the day before yesterday, and so on). The graph highlights when your steps were above your goal for the day.

7) Displays Floors climbed graphic as an ARC between 7 and 8 on the watch face. The display shows floors climbed as a percentage of goal. The number of floors climbed is also displayed in the Steps dial (above the steps count), once some floors have actually been climbed.

8) Shows the current day number of the month as well as a Phone connected icon, an alarm icon (if you've set an alarm this icon will display) and a "do not disturb" icon which displays when in do not disturb mode.

9) The HR dial shows HR as well as percentage of maximum HR, if you've defined this in your Garmin profile or created any heart rate zones. if no maximum HR is set it will default to using the old standard "220 - your age", so long as your age is set in your Garmin profile.

10) The steps dial shows steps as well as percentage of steps goal.

NOTES:

- All the functionality of this watch face will no doubt drain the battery more than a simple watch face that just shows the time (or the Garmin watch faces that are not developed in Connect IQ). Please be aware of that and make use of the battery saving functions.

- If after updating from an earlier release of this watch face it stops working, please uninstall and install again

- If you are experiencing app crashes, please ensure you have updated to the latest firmware on your device. The app crashes are due to a known issue in the Garmin SDK that occurs with older firmware.

- Support for other watch devices coming soon...


# What's New


1.1.0 - Added support for full range of Fenix6 devices.
- Added AntiAlias improvements for devices that support it - currently Fenix 6, D2 and MARQ series devices.

1.0.4.0 - Added support fo MARQ Golfer

1.0.30

- Add support for MARQ Adventurer and Commander

1.0.29

- Better handling of heart rate zones and current sport for max HR calculation. Better handling of Altitude to ensure numerical data
