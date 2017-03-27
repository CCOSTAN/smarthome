## This is a test table.

| Automation   |   Trigger   |   Conditions   |  Action   |  Url Link    |
| ----------   |   -------   |   -----------  |  -------  |  ---------   |
| Outdoor Turn Lights ON 15 minutes before sunset| 
 			sun is 'below horizon' or event is sunset
 			offset -15 minutes
 		| 
         None
 		| 
 			Turn Light(s) ON
 		| TBD| 
| Outdoor Turn Lights OFF 15 minutes after sunrise| 
 			sun is 'above horizon' or event is sunrise
 			offset +15 minutes
 		| 
 			Every day
 		| 
 			Turn Light(s) OFF
 		| TBD| 
| Turn Home Security System ON at Sunset| 
 			event is sunset
 		| 
 			Do it only when people are at home
 			Weekdays ONLY
 			Home Security System is Disarmed
 		| 
 			Turn ON Home Security System in 'Home' mode
 			Send an alert
 			Drop a message in the announcement queue
 		| TBD| 
| Kitchen Lights on early morning during school days| 
 			exactly at 5:30 AM
 		| 
 		    Weekdays (mon, tue, wed, thu, fri)
 			Only during school days check (if school days input_boolean is ON)
 		| 
 			turn kitchen lights ON
 		| TBD| 
| Master Bedroom lights ON (Mallika side)at 5:20| 
 			Exactly at 5:20 AM
 		| 
 			Only during Weekdays (mon, tue, wed, thu, fri)
 			Only during school days check (if school days input_boolean is ON)
 		| 
 			Turn ON Mallika's side of the bed lamp at 10% brightness with transition of 1 minute from 0 to 10% brightness
 			Do not disturb Suresh
 		| TBD| 
| Master Bedroom lights OFF (Mallika side)at 5:45| 
 			Exactly at 5:45 AM
 		| 
 			Only during Weekdays (mon, tue, wed, thu, fri)
 			Only during school days check (if school days input_boolean is ON)
 		| 
 			Turn OFF Mallika's side of the bed lamp with no transition
 			Do not disturb Suresh
 		| TBD| 
| Master Bedroom lights ON at 6:59 AM| 
 			Exactly at 6:59 AM
 		| 
 			Only during Weekdays (mon, tue, wed, thu, fri)
 		| 
 			Turn ON Master Bedroom lights with transition of 2 minutes at 25% brightness
 			Suresh's wake up alarm will go off at 7:00 AM
 			Suresh would like to snooze a couple of times, while he is in bed, make announcements of daily weather, commute to work, temperature on bluetooth speaker
 		| TBD| 
| Master Bedroom Lights OFF at 9:00 AM| 
 			Only during Weekdays (mon, tue, wed, thu, fri)
 		| 
 			Week days
 		| 
 			Suresh is most likely at work, turn off master bed room lights.
 			TODO: Check device_tracker and the location, When Suresh leaves home, turn off master bedroom lights immediately
 		| TBD| 
| Turn Kitchen Lights OFF at 8:15 AM| 
 			Exactly at 8:15 AM
 		| 
 			Everyday - it is usually bright enough in Kitchen at 8:15 AM
 		| 
 			Turn OFF kitchen lights
 		| TBD| 
| Dim Kitchen lights 15 minutes before bed time| 
 			Exactly at 9:45 PM. (Our bed time is at 10:00 PM)
 		| 
 			Make sure the light is ON before dimming
 		| 
 			Turn ON the light and set the brightness of the light to 15%
 		| TBD| 
| Turn ON Home Security System at Bedtime| 
 			Exactly at 10:00 PM
 		| 
 			People MUST be home
 			Home Security System cannot be in AWAY mode
 			Home Security System MUST BE Disarmed
 		| 
 			Turn ON Home Security System in HOME mode
 			Send an alert
 			Make an annnouncement inside the house
 		| TBD| 
| Good Night| 
 			Exactly at 10:00 PM
 		| 
 			TODO: Check for summer hours Vs Winter hours
 		| 
 			Turn OFF Family Room Lights
 			Turn OFF Kitchen Lights
 			Turn OFF Guest Bedroom Lights
 			Turn OFF Master Bedroom Lights
 			Turn OFF Office Room Lights
 			Turn OFF Basement Lights (TBD)
 			KEEP Front yard and Backyard lights for security reasons
 			AND
 			Play 'Soft Kitty Warm Kitty Little Ball of Fur' Song :)
 		| TBD| 
| Motion Detected - 1| 
 			motion sensor state changed
 		| 
 			It is Dark outside
 			TV is ON
 			TV Room Lights are ON
 		| 
 			Dim TV Lights
 		| TBD| 
| Motion Detected - 1| 
 			motion sensor state changed
 		| 
 			It is Dark outside
 			TV is ON
 			TV Room Lights are ON
 		| 
 			Dim TV Lights
 		| TBD| 
| Motion Detected - 1| 
 			motion detected
 		| 
 			It is Dark outside
 			TV is ON
 			TV Room Lights are ON
 		| 
 			Dim TV Lights
 		| TBD| 
| Motion Detected - 2| 
 			motion detected
 		| 
 			It is Dark outside
 			TV is ON
 			TV Room Lights are OFF
 		| 
 			Dim TV Lights
 		| TBD| 
| Motion Detected - 3| 
 			motion detected
 		| 
 			It is Dark outside
 			TV is OFF
 			TV Room Lights are ON
 		| 
 			Set the light brightness to 100%.
 		| TBD| 
| Motion Detected - 4| 
 			motion detected
 		| 
 			It is Dark outside
 			TV is OFF
 			TV Room Lights are OFF
 		| 
 			Set the light brightness to 100%.
 		| TBD| 
| NO motion sensed - 1| | 
 			It is Dark outside
 			TV is ON
 			TV Room Lights are ON
 		| 
 			Turn Lights OFF
 		| TBD| 
| NO motion sensed - 2| | 
 			It is Dark outside
 			TV is OFF
 			TV Room Lights are ON
 		| 
 			Turn Lights OFF
 		| TBD| 
| MQTT Announcements| 
 			When a message arrives in a specific topic
 		| 
 			None
 		| 
 			Read the text, call amazon polly to convert to audio/mp3 and Play the mp3 using media player
 		| TBD| 
| Check Battery Level of Phone| 
 			Battery level is below 30%
 			device_tracker.suresh_suresh
 			device_tracker.mallika_mallika
 			device_tracker.hasika_hasika
 			device_tracker.srinika_srinika
 		| 
 			None
 		| 
 			Send a notification
 		| TBD| 
| Check Battery Levels of Motion Sensors| 
 			Battery level is below 30%
 			upstairs_motion_sensor
 			downstairs_motion_sensor
 		| 
 			None
 		| 
 			Send a notification
 		| TBD| 
| Notify Home Security Status| 
 			Home Alsrm system status changed
 		| 
 			None
 		| 
 			Send a notification
 		| TBD| 
| Home Security| 
 			Turn ON Home Alarm System when no one home
 		| 
 			when all the members of family are "not home"
 		| 
 			Turn ON home Security System
 		| TBD| 
| Flash Lights When Someone at the door| 
 			motion detected at the front door
 		| 
 			when people are home
 		| 
 			flash lights
 		| TBD| 
| Play Dog Sounds| 
 			motion detected at the front door or back door
 		| 
 			when no one at home
 		| 
 			play dog barking sounds
 		| TBD| 
| Turn Humidifier ON automatically| 
 			Indoor humidity level is below threshold (30)
 		| 
 			When people are home
 		| 
 			Turn Humidifier On
 			Notify that the humidifier is turned ON, and remind to check water level
 		| TBD| 
| Turn Humidifier OFF automatically| 
 			Indoor humidity level is above threshold (30)
 		| 
 			None
 		| 
 			Turn Dehumidifier ON
 		| TBD| 
| Notify when someone arrives home| 
 			- device_tracker.mallika_mallika
 			- device_tracker.suresh_suresh
 			- device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika
 		| 
 			entered zone
 		| 
 			Send an alert
 		| TBD| 
| Notify when someone arrives home| 
 			- device_tracker.mallika_mallika
 			- device_tracker.suresh_suresh
 			- device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika
 		| 
 			leave zone
 		| 
 			Send an alert
 		| TBD| 
| Notify when Kids reach school| 
 			- device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika
 		| 
 			enter school zone
 		| 
 			send an alert
 		| TBD| 
| Notify when Kids reach school| 
 			- device_tracker.srinika_srinika
 			- device_tracker.hasika_hasika
 		| 
 			leaves schol zone
 		| 
 			Send an alert
 		| TBD| 
| Alert when everyone is away| 
 			group.all_devices
 		| 
 			state changed to "not home"
 		| 
 			Send an alert	
 			Turn ON Home Security System
 			Turn down temperature?
 		| TBD| 
| Home Assistant Startup| 
 			event_type is homeassistant_start
 		| 
 			None
 		| 
 			Send an alert
 		| TBD| 
| New Home Assistant Update| 
 			updater.updater
 		| 
 			None
 		| 
 			Send an alert with link to HA
 		| TBD| 
| Timer enabled smart Switch| 
 			light status is On
 		| 
 			for a certain time
 			during day time
 		| 
 			Turn off light
 		| TBD| 
| Weather - Heavy Wind Alerts| 
 			Entity - sensor.dark_sky_wind_speed
 		| 
 			Wind speed is aboive 20 and below 40
 		| 
 			Send an alert
 			flash lights
 		| TBD| 
| Weather - Super Heavy Winds| 
 			sensor.dark_sky_wind_speed
 		| 
 			Wind speed is aboive 40
 		| 
 			Send an alert to stay indoors
 			Announce in the house
 			Flash lights
 		| TBD| 
| Provide Daily Weather Update| 
 			at 7:00 AM
 		| 
 			None
 		| 
 			Send an Alert
 			Announce in the house
 		| TBD| 
| Greet Family Members| 
         - device_tracker.mallika_mallika
         - device_tracker.suresh_suresh
         - device_tracker.srinika_srinika
         - device_tracker.hasika_hasika
 		| 
 			for 2 minutes
 		| 
 			Announce, Welcome, family member!
 		| TBD| 
| Z-wave| 
 			at 4:30 in the morning
 		| 
 			None
 		| 
 			Heal Z-Wave network
 		| TBD| 
