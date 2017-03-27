Automation   |   Trigger   |  Action  |
----------   |   -------   |  ------- |
Outdoor Turn Lights ON 15 minutes before sunset | sun is below horizon or event is sunset; offset -15 minutes | Turn Light(s) ON |
Outdoor Turn Lights OFF 15 minutes after sunrise | sun is 'above horizon' or event is sunrise; offset +15 minutes | Turn Light(s) OFF |
Turn Home Security System ON at Sunset | event is sunset | Turn ON Home Security System in 'Home' mode;Send an alert;Drop a message in the announcement queue |
Kitchen Lights on early morning during school days | exactly at 5:30 AM | turn kitchen lights ON |
Master Bedroom lights ON (Mallika side)at 5:20 | Exactly at 5:20 AM | Turn ON Mallika's side of the bed lamp at 10% brightness with transition of 1 minute from 0 to 10% brightness;Do not disturb Suresh |
Master Bedroom lights OFF (Mallika side)at 5:45 | Exactly at 5:45 AM | Turn OFF Mallika's side of the bed lamp with no transition
 			Do not disturb Suresh |
Master Bedroom lights ON at 6:59 AM | Exactly at 6:59 AM | Turn ON Master Bedroom lights with transition of 2 minutes at 25% brightness
 			Suresh's wake up alarm will go off at 7:00 AM
 			Suresh would like to snooze a couple of times, while he is in bed, make announcements of daily weather, commute to work, temperature on bluetooth speaker |
Master Bedroom Lights OFF at 9:00 AM | Only during Weekdays (mon, tue, wed, thu, fri) | Suresh is most likely at work, turn off master bed room lights.
 			TODO: Check device_tracker and the location, When Suresh leaves home, turn off master bedroom lights immediately |
Turn Kitchen Lights OFF at 8:15 AM | Exactly at 8:15 AM | Turn OFF kitchen lights |
Dim Kitchen lights 15 minutes before bed time | Exactly at 9:45 PM. (Our bed time is at 10:00 PM) | Turn ON the light and set the brightness of the light to 15% |
Turn ON Home Security System at Bedtime | Exactly at 10:00 PM | Turn ON Home Security System in HOME mode
 			Send an alert
 			Make an annnouncement inside the house |
Good Night | Exactly at 10:00 PM | Turn OFF Family Room Lights
 			Turn OFF Kitchen Lights
 			Turn OFF Guest Bedroom Lights
 			Turn OFF Master Bedroom Lights
 			Turn OFF Office Room Lights
 			Turn OFF Basement Lights (TBD)
 			KEEP Front yard and Backyard lights for security reasons
 			AND
 			Play 'Soft Kitty Warm Kitty Little Ball of Fur' Song :) |
Motion Detected - 1 | motion sensor state changed | Dim TV Lights |
Motion Detected - 1 | motion sensor state changed | Dim TV Lights |
Motion Detected - 1 | motion detected | Dim TV Lights |
Motion Detected - 2 | motion detected | Dim TV Lights |
Motion Detected - 3 | motion detected | Set the light brightness to 100%. |
Motion Detected - 4 | motion detected | Set the light brightness to 100%. |
NO motion sensed - 1 |  | Turn Lights OFF |
NO motion sensed - 2 |  | Turn Lights OFF |
MQTT Announcements | When a message arrives in a specific topic | Read the text, call amazon polly to convert to audio/mp3 and Play the mp3 using media player |
Check Battery Level of Phone | Battery level is below 30%
 			device_tracker.suresh_suresh
 			device_tracker.mallika_mallika
 			device_tracker.hasika_hasika
 			device_tracker.srinika_srinika | Send a notification |
Check Battery Levels of Motion Sensors | Battery level is below 30%
 			upstairs_motion_sensor
 			downstairs_motion_sensor | Send a notification |
Notify Home Security Status | Home Alsrm system status changed | Send a notification |
Home Security | Turn ON Home Alarm System when no one home | Turn ON home Security System |
Flash Lights When Someone at the door | motion detected at the front door | flash lights |
Play Dog Sounds | motion detected at the front door or back door | play dog barking sounds |
Turn Humidifier ON automatically | Indoor humidity level is below threshold (30) | Turn Humidifier On
 			Notify that the humidifier is turned ON, and remind to check water level |
Turn Humidifier OFF automatically | Indoor humidity level is above threshold (30) | Turn Dehumidifier ON |
Notify when someone arrives home | - device_tracker.mallika_mallika
 			- device_tracker.suresh_suresh
 			- device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika | Send an alert |
Notify when someone arrives home | - device_tracker.mallika_mallika
 			- device_tracker.suresh_suresh
 			- device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika | Send an alert |
Notify when Kids reach school | - device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika | send an alert |
Notify when Kids reach school | - device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika | Send an alert |
Alert when everyone is away | group.all_devices | Send an alert	
 			Turn ON Home Security System
 			Turn down temperature? |
Home Assistant Startup | event_type is homeassistant_start | Send an alert |
New Home Assistant Update | updater.updater | Send an alert with link to HA |
Timer enabled smart Switch | light status is On | Turn off light |
Weather - Heavy Wind Alerts | Entity - sensor.dark_sky_wind_speed | Send an alert
 			flash lights |
Weather - Super Heavy Winds | sensor.dark_sky_wind_speed | Send an alert to stay indoors
 			Announce in the house
 			Flash lights |
Provide Daily Weather Update | at 7:00 AM | Send an Alert
 			Announce in the house |
Greet Family Members | - device_tracker.mallika_mallika
         - device_tracker.suresh_suresh
         - device_tracker.srinika_srinika
         - device_tracker.hasika_hasika | Announce, Welcome, family member! |
Z-wave | at 4:30 in the morning | Heal Z-Wave network |
