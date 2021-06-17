# TrainingHR
Garmin Connect IQ Training HR App

When I'm Base Training I'm very focussed on monitoring Heart Rate and ensuring I'm sitting in particular zones. I wanted a single datafield that could display everything I needed to know, related to Heart Rate - that being: HR, HR zone and where I am in that zone, average HR, Average HR zone and Max HR.
REQUIREMENTS:

This data field displays a number of Heart Rate related values and as such, requires a Heart Rate sensor to be connected to your Garmin device.

** The data field has been optimised for full-width display on Garmin Edge type devices. **

**CIRCLES or BARS?:**

There is a configuration option in the App Settings that will display the HR zone range and Average HR Zone range as circles instead of the default bars, as per the screen shots.  Unfortunately (due to memory constraints) the Edge520 device cannot display in circles mode.

**DISPLAY FIELDS:**

- Heart Rate (BPM)

- HR Zone (as per HR Zones note, below)

- Maximum HR (during this activity)

- Average HR (BPM)

- Average HR Zone (as per HR Zones note, below)

- Time of Day (available in larger screen configurations)

- Elapsed Time (available in larger screen configurations)

- Rolling 60 second HR Histogram (Available for Edge 130/130+/530/830/1030x/1000 devices)

**GARMIN PROFILE?:**

An App Setting lets you choose whether you want to use the HR Zone settings you've defined within your Garmin Profile OR the zones you define within the App Settings. If you choose your Garmin Profile there is no need to provide values for the HR Zones, LTHR, HRR, MaxHR and the Zone Type in the App Settings, you can leave these blank.

**HR ZONES:**

You can define up to 5 HR zones in the App Settings. The zones can be based on Lactate Threshold Heart Rate (LTHR), Maximum Heart Rate (MAXHR), or Heart Rate Reserve (HRR). You must choose which Target HR is the basis for your zones in the App Settings.

The Zones will default to the standard Coggan zones, which you can adjust. The standard Coggan HR zones are as follows:

- Z1 = Less than 68% (Recovery - Grey)
- Z2 = 68 - 83% (Endurance - Blue)
- Z3 = 84 - 94% (Tempo - Green)
- Z4 = 95 - 105% (Threshold - Orange)
- Z5 = 106 - MAX (VO2Max - Red)

**TrainingHR is designed to be used in two-field screen layouts with my other App - TrainingPower.**


# What's New

**v1.7.7:**
- Add new Circles mode Layouts: Layout 4A (Edge 530/830), Layout 3 (Edge 820) and Layouts 3A, 3B, 4B, 5B, 6B, 7B (Edge 520+)

**v1.7.6**
- Code optimisations to reduce memory and processing

**v1.7.5:**
- FIX: App crash from start for specific devices - Fenix 5 and ForeRunner 935
- Optimise 1 & 2 field layout for Edge1030 to make it more consistent with other layouts

**v1.7.4:**
- FIX: App could show an error when accessing the in-app settings on a supported device AND you had previously set "Use my Garmin Profile" to YES.

**v1.7.3:**
- NEW Settings option for "Activity Timer Display". You can now choose "LAP time" (or, Elapsed Time, Moving Time, or no Timer display).
- Support the new Garmin AntiAlias feature on supported devices. With this, graphics are rendered more smoothly, when drawing circles and angular lines

**v1.7.2:**
- Heart Rate Zone Calculation Optimisations

**v1.7.1:**
- NEW: Getting ready to support "In App Settings" (that is, not having to use Garmin Connect or your phone to change App settings). This is currently device firmware dependent, to which Garmin does not provide advice on which devices will receive firmware updates or when updates will be made available. Currently, only the Fenix6, D2 and MARQ devices have the firmware to support this functionality. I'm hopeful the Edge devices (at least some) will soon too. Once a device receives a firmware update that supports in app settings, Training HR "In App Settings" will just start working.
- Support for new Forerunner 745 device
- Improve efficiency of drawing circles and ARCs
- Remove App specific LAP function (from All devices except: original Edge 520, original Fenix5 and FR935) as Garmin and Strava do this better

**v1.6.5.0:**
- Added Settings option to turn on (default) or off the display of Seconds for Time of Day and Timer displays (All devices except original Edge 520). This has the benefit of allowing room for a larger font for Time of Day and Timer.
- Compiled under v3.2.1 of Connect IQ SDK

**v1.6.4.0:**
- Added Settings option to display Elapsed Time (since Timer Start), Moving Time (excludes time auto-paused), or No Timer
- Added Settings option to turn off display of "Time of Day"
- Added ability to set Zone1 start at zero (effectively means Zone1 can range from 0 to the start of Zone2)

**v1.6.3.0:**
- Automatically update MAXHR into settings when new maximum achieved. MAXHR will turn blue when a new maximum has been reached.
- Standardize colours used to be from 64 colour pallette (except Edge130, which is only Black and White)

**v1.6.2.0:**
- Covid-19 Lockdown Release
- New Circles layouts for configurations 3A, 3B, 4B, 5B, 6B, 7B layouts for Edge 530 / 830
- New Circles layouts for 2 field screen configurations for Edge 520+ / 820
- Added support for Fenix 6 / 6sPro / 6Pro / 6XPro in screen configurations 1, 2 and 4C
- Added support for Marq Golfer in screen configurations 1, 2 and 4B

**v1.6.0.0:**
- Added support for Garmin Edge 1030+ devices
- New Circles layouts for configurations 2, 3A, 3B, 4B, 5B, 6B, 7B layouts for Edge 1030/1030Bont/1030+
- New circles layouts for 2 datafield display in Edge 530/830
- New circles layouts for 2 & 3 datafield display in Edge 1000
- Added rolling 60 second HR histogram to the new Circles configuration for Edge 530/830/1030x/1000 devices (new property to activate this in settings - default is off)

**V1.5.6.2:**
- Support for MARQ Adventurer and Commander (in 1,2 and 4B datafield layouts) and Fenix 6S (in 1, 2 and 4C datafield layouts).

**V1.5.6:**
- Support for Edge 530/830, Forerunner 945 and Marq devices (in 1, 2 and 4 field display modes)
- Add 4 field display options to supported wearable devices
- Add LAP function. This works differently to a standard LAP function as I see the main problem with a standard LAP function is what if you want to revert back to Average HR for the entire activity? You can't. With my LAP function when you press the LAP button it starts calculating and displaying average HR from that point - a red "LAP" icon is displayed on screen - When you press the LAP button again, the display reverts back to showing Average HR for the entire activity. This way you can ride out to the bottom of a hill, press the LAP button and see your average HR up the hill, when you get to the top of the hill you can hit the LAP button again and revert to showing average HR for the entire activity. You can do this as many times as you like in an activity. You can also turn off the app's ability to respond to the LAP button in app settings.
