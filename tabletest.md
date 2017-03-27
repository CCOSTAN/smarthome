<table><tr><th>Automation</th><th>Trigger</th><th>Condition</th><th>Action</th><th>Link</th></tr><tr><td>Outdoor Turn Lights ON 15 minutes before sunset</td><td>
			sun is below horizon or event is sunset
      offset -15 minutes
		</td><td>
        None
		</td><td><ul><li>Turn Light(s) ON</li><li>Send an alert</li></ul></td><td>tbd</td></tr><tr><td>Outdoor Turn Lights OFF 15 minutes after sunrise</td><td>
			sun is 'above horizon' or event is sunrise
      offset +15 minutes
		</td><td>
			Every day
		</td><td><ul><li>Turn Light(s) OFF</li></ul></td><td>tbd</td></tr><tr><td>Turn Home Security System ON at Sunset</td><td>
			event is sunset
		</td><td>
			Do it only when people are at home
      Weekdays ONLY
      Home Security System is Disarmed
		</td><td><ul><li>Turn ON Home Security System in 'Home' mode</li><li>Send an alert</li><li>Drop a message in the announcement queue</li></ul></td><td>tbd</td></tr><tr><td>Kitchen Lights on early morning during school days</td><td>
			exactly at 5:30 AM
		</td><td>
		    Weekdays (mon, tue, wed, thu, fri)
        Only during school days check (if school days input_boolean is ON)
		</td><td><ul><li>turn kitchen lights ON</li></ul></td><td>tbd</td></tr><tr><td>Master Bedroom lights ON (Mallika side)at 5:20</td><td>
			Exactly at 5:20 AM
		</td><td>
			Only during Weekdays (mon, tue, wed, thu, fri)
      Only during school days check (if school days input_boolean is ON)
		</td><td><ul><li>Turn ON Mallika's side of the bed lamp at 10% brightness with transition of 1 minute from 0 to 10% brightness</li><li>Do not disturb Suresh</li></ul></td><td>tbd</td></tr><tr><td>Master Bedroom lights OFF (Mallika side)at 5:45</td><td>
			Exactly at 5:45 AM
		</td><td>
			Only during Weekdays (mon, tue, wed, thu, fri)
      Only during school days check (if school days input_boolean is ON)
		</td><td><ul><li>Turn OFF Mallika's side of the bed lamp with no transition</li><li>Do not disturb Suresh</li></ul></td><td>tbd</td></tr><tr><td>Master Bedroom lights ON at 6:59 AM</td><td>
			Exactly at 6:59 AM
		</td><td>
			Only during Weekdays (mon, tue, wed, thu, fri)
		</td><td><ul><li>Turn ON Master Bedroom lights with transition of 2 minutes at 25% brightness</li><li>Suresh's wake up alarm will go off at 7:00 AM</li><li>Suresh would like to snooze a couple of times, while he is in bed, make announcements of daily weather, commute to work, temperature on bluetooth speaker</li></ul></td><td>tbd</td></tr><tr><td>Master Bedroom Lights OFF at 9:00 AM</td><td>
			Only during Weekdays (mon, tue, wed, thu, fri)
		</td><td>
			Week days
		</td><td><ul><li>Suresh is most likely at work, turn off master bed room lights</li><li>TODO: Check device_tracker and the location, When Suresh leaves home, turn off master bedroom lights immediately</li></ul></td><td>tbd</td></tr><tr><td>Turn Kitchen Lights OFF at 8:15 AM</td><td>
			Exactly at 8:15 AM
		</td><td>
			Everyday - it is usually bright enough in Kitchen at 8:15 AM
		</td><td><ul><li>Turn OFF kitchen lights</li></ul></td><td>tbd</td></tr><tr><td>Dim Kitchen lights 15 minutes before bed time</td><td>
			Exactly at 9:45 PM. (Our bed time is at 10:00 PM)
		</td><td>
			Make sure the light is ON before dimming
		</td><td><ul><li>Turn ON the light and set the brightness of the light to 15%</li></ul></td><td>tbd</td></tr><tr><td>Turn ON Home Security System at Bedtime</td><td>
			Exactly at 10:00 PM
		</td><td>
			People MUST be home
      Home Security System cannot be in AWAY mode
      Home Security System MUST BE Disarmed
		</td><td><ul><li>Turn ON Home Security System in HOME mode</li><li>Send an alert</li><li>Make an annnouncement inside the house</li></ul></td><td>tbd</td></tr><tr><td>Good Night</td><td>
			Exactly at 10:00 PM
		</td><td>
			TODO: Check for summer hours Vs Winter hours
		</td><td><ul><li>Turn OFF Family Room Lights</li><li>Turn OFF Kitchen Lights</li><li>Turn OFF Guest Bedroom Lights</li><li>Turn OFF Master Bedroom Lights</li><li>Turn OFF Office Room Lights</li><li>Turn OFF Basement Lights (TBD)</li><li>KEEP Front yard and Backyard lights for security reasons</li><li>Play 'Soft Kitty Warm Kitty Little Ball of Fur' Song :)</li></ul></td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>
			motion sensor state changed
		</td><td>
			It is Dark outside
      TV is ON
      TV Room Lights are ON
		</td><td><ul><li>Dim TV Lights</li></ul></td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>
			motion sensor state changed
		</td><td>
			It is Dark outside
      TV is ON
      TV Room Lights are ON
		</td><td><ul><li>Dim TV Lights</li></ul></td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>
			motion detected
		</td><td>
			It is Dark outside
      TV is ON
      TV Room Lights are ON
		</td><td><ul><li>Dim TV Lights</li></ul></td><td>tbd</td></tr><tr><td>Motion Detected - 2</td><td>
			motion detected
		</td><td>
			It is Dark outside
      TV is ON
      TV Room Lights are OFF
		</td><td><ul><li>Dim TV Lights</li></ul></td><td>tbd</td></tr><tr><td>Motion Detected - 3</td><td>
			motion detected
		</td><td>
			It is Dark outside
      TV is OFF
      TV Room Lights are ON
		</td><td><ul><li>Set the light brightness to 100%.</li></ul></td><td>tbd</td></tr><tr><td>Motion Detected - 4</td><td>
			motion detected
		</td><td>
			It is Dark outside
      TV is OFF
      TV Room Lights are OFF
		</td><td><ul><li>Set the light brightness to 100%.</li></ul></td><td>tbd</td></tr><tr><td>NO motion sensed - 1</td><td></td><td>
			It is Dark outside
      TV is ON
      TV Room Lights are ON
		</td><td><ul><li>Turn Lights OFF</li></ul></td><td>tbd</td></tr><tr><td>NO motion sensed - 2</td><td></td><td>
			It is Dark outside
      TV is OFF
      TV Room Lights are ON
		</td><td><ul><li>Turn Lights OFF</li></ul></td><td>tbd</td></tr><tr><td>MQTT Announcements</td><td>
			When a message arrives in a specific topic
		</td><td>
			None
		</td><td><ul><li>Read the text, call amazon polly to convert to audio/mp3 and Play the mp3 using media player</li></ul></td><td>tbd</td></tr><tr><td>Check Battery Level of Phone</td><td>
			Battery level is below 30%
      device_tracker.suresh_suresh
      device_tracker.mallika_mallika
      device_tracker.hasika_hasika
      device_tracker.srinika_srinika
		</td><td>
			None
		</td><td><ul><li>Send a notification</li></ul></td><td>tbd</td></tr><tr><td>Check Battery Levels of Motion Sensors</td><td>
			Battery level is below 30%
      upstairs_motion_sensor
      downstairs_motion_sensor
		</td><td>
			None
		</td><td><ul><li>Send a notification</li></ul></td><td>tbd</td></tr><tr><td>Notify Home Security Status</td><td>
			Home Alarm system status changed
		</td><td>
			None
		</td><td><ul><li>Send a notification</li></ul></td><td>tbd</td></tr><tr><td>Home Security</td><td>
			Turn ON Home Alarm System when no one home
		</td><td>
			when all the members of family are "not home"
		</td><td><ul><li>Turn ON home Security System</li></ul></td><td>tbd</td></tr><tr><td>Flash Lights When Someone at the door</td><td>
			motion detected at the front door
		</td><td>
			when people are home
		</td><td><ul><li>flash lights</li></ul></td><td>tbd</td></tr><tr><td>Play Dog Sounds</td><td>
			motion detected at the front door or back door
		</td><td>
			when no one at home
		</td><td><ul><li>play dog barking sounds</li></ul></td><td>tbd</td></tr><tr><td>Turn Humidifier ON automatically</td><td>
			Indoor humidity level is below threshold (30)
		</td><td>
			When people are home
		</td><td><ul><li>Turn Humidifier On</li><li>Notify that the humidifier is turned ON, and remind to check water level</li></ul></td><td>tbd</td></tr><tr><td>Turn Humidifier OFF automatically</td><td>
			Indoor humidity level is above threshold (30)
		</td><td>
			None
		</td><td><ul><li>Turn Dehumidifier ON</li></ul></td><td>tbd</td></tr><tr><td>Notify when someone arrives home</td><td>
			device_tracker.mallika_mallika
      device_tracker.suresh_suresh
      device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td>
			entered zone
		</td><td><ul><li>Send an alert</li></ul></td><td>tbd</td></tr><tr><td>Notify when someone arrives home</td><td>
			device_tracker.mallika_mallika
      device_tracker.suresh_suresh
      device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td>
			leave zone
		</td><td><ul><li>Send an alert</li></ul></td><td>tbd</td></tr><tr><td>Notify when Kids reach school</td><td>
			device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td>
			enter school zone
		</td><td><ul><li>send an alert</li></ul></td><td>tbd</td></tr><tr><td>Notify when Kids reach school</td><td>
			device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td>
			leaves schol zone
		</td><td><ul><li>Send an alert</li></ul></td><td>tbd</td></tr><tr><td>Alert when everyone is away</td><td>
			group.all_devices
		</td><td>
			state changed to "not home"
		</td><td><ul><li>Send an alert</li><li>Turn ON Home Security System</li><li>Turn down temperature?</li></ul></td><td>tbd</td></tr><tr><td>Home Assistant Startup</td><td>
			event_type is homeassistant_start
		</td><td>
			None
		</td><td><ul><li>Send an alert</li></ul></td><td>tbd</td></tr><tr><td>New Home Assistant Update</td><td>
			updater.updater
		</td><td>
			None
		</td><td><ul><li>Send an alert with link to HA</li></ul></td><td>tbd</td></tr><tr><td>Timer enabled smart Switch</td><td>
			light status is On
		</td><td>
			for a certain time
      during day time
		</td><td><ul><li>Turn off light</li></ul></td><td>tbd</td></tr><tr><td>Weather - Heavy Wind Alerts</td><td>
			Entity - sensor.dark_sky_wind_speed
		</td><td>
			Wind speed is aboive 20 and below 40
		</td><td><ul><li>Send an alert</li><li>flash lights</li></ul></td><td>tbd</td></tr><tr><td>Weather - Super Heavy Winds</td><td>
			sensor.dark_sky_wind_speed
		</td><td>
			Wind speed is aboive 40
		</td><td><ul><li>Send an alert to stay indoors</li><li>Announce in the house</li><li>Flash lights</li></ul></td><td>tbd</td></tr><tr><td>Provide Daily Weather Update</td><td>
			at 7:00 AM
		</td><td>
			None
		</td><td><ul><li>Send an Alert</li><li>Announce in the house</li></ul></td><td>tbd</td></tr><tr><td>Greet Family Members</td><td>
        device_tracker.mallika_mallika
        device_tracker.suresh_suresh
        device_tracker.srinika_srinika
        device_tracker.hasika_hasika
		</td><td>
			for 2 minutes
		</td><td><ul><li>Announce, Welcome, family member!</li></ul></td><td>tbd</td></tr><tr><td>Z-wave</td><td>
			at 4:30 in the morning
		</td><td>
			None
		</td><td><ul><li>Heal Z-Wave network</li></ul></td><td>tbd</td></tr></table>
