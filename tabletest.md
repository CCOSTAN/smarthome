<table><tr><th>Automation</th><th>Trigger</th><th>Condition</th><th>Action</th><th>Link</th></tr><tr><td>Outdoor Turn Lights ON 15 minutes before sunset</td><td>
			sun is below horizon or event is sunset
      offset -15 minutes
		</td><td><li>None</li></ul></td><td><ul><li>Turn Light(s) ON</li><li>Send an alert</li></ul><ul></td><td>tbd</td></tr><tr><td>Outdoor Turn Lights OFF 15 minutes after sunrise</td><td>
			sun is 'above horizon' or event is sunrise
      offset +15 minutes
		</td><td><li>Every day</li></ul></td><td><ul><li>Turn Light(s) OFF</li></ul><ul></td><td>tbd</td></tr><tr><td>Turn Home Security System ON at Sunset</td><td>
			event is sunset
		</td><td><li>Do it only when people are at home</li><li>Weekdays ONLY</li><li>Home Security System is Disarmed</li></ul></td><td><ul><li>Turn ON Home Security System in 'Home' mode</li><li>Send an alert</li><li>Drop a message in the announcement queue</li></ul><ul></td><td>tbd</td></tr><tr><td>Kitchen Lights on early morning during school days</td><td>
			exactly at 5:30 AM
		</td><td><li>Weekdays (mon, tue, wed, thu, fri)</li><li>Only during school days check (if school days input_boolean is ON)</li></ul></td><td><ul><li>turn kitchen lights ON</li></ul><ul></td><td>tbd</td></tr><tr><td>Master Bedroom lights ON (wife's side)at 5:20</td><td>
			Exactly at 5:20 AM
		</td><td><li>Only during Weekdays (mon, tue, wed, thu, fri)</li><li>Only during school days check (if school days input_boolean is ON)</li></ul></td><td><ul><li>Turn ON wife's side of the bed lamp at 10% brightness with transition of 1 minute from 0 to 10% brightness</li></ul><ul></td><td>tbd</td></tr><tr><td>Master Bedroom lights OFF (wife's side)at 5:45</td><td>
			Exactly at 5:45 AM
		</td><td><li>Only during Weekdays (mon, tue, wed, thu, fri)</li><li>Only during school days check (if school days input_boolean is ON)</li></ul></td><td><ul><li>Turn OFF wife's side of the bed lamp with no transition</li></ul><ul></td><td>tbd</td></tr><tr><td>Master Bedroom lights ON at 6:59 AM</td><td>
			Exactly at 6:59 AM
		</td><td><li>Only during Weekdays (mon, tue, wed, thu, fri)</li></ul></td><td><ul><li>Turn ON Master Bedroom lights with transition of 2 minutes at 25% brightness</li><li>Announce daily weather updates, commute to work...etc on home audio system</li></ul><ul></td><td>tbd</td></tr><tr><td>Master Bedroom Lights OFF at 9:00 AM</td><td>
			Only during Weekdays (mon, tue, wed, thu, fri)
		</td><td><li>Week days</li></ul></td><td><ul><li>Turn off master bedroom lights</li><li>TODO: Check device_tracker and the location, When Suresh leaves home, turn off master bedroom lights immediately</li></ul><ul></td><td>tbd</td></tr><tr><td>Turn Kitchen Lights OFF at 8:15 AM</td><td>
			Exactly at 8:15 AM
		</td><td><li>Everyday - it is usually bright enough in Kitchen at 8:15 AM</li></ul></td><td><ul><li>Turn OFF kitchen lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Dim Kitchen lights 15 minutes before bed time</td><td>
			Exactly at 9:45 PM. (Our bed time is at 10:00 PM)
		</td><td><li>Make sure the light is ON before dimming</li></ul></td><td><ul><li>Turn ON the light and set the brightness of the light to 15%</li></ul><ul></td><td>tbd</td></tr><tr><td>Turn ON Home Security System at Bedtime</td><td>
			Exactly at 10:00 PM
		</td><td><li>People MUST be home</li><li>Home Security System cannot be in AWAY mode</li><li>Home Security System MUST BE Disarmed</li></ul></td><td><ul><li>Turn ON Home Security System in HOME mode</li><li>Send an alert</li><li>Make an annnouncement inside the house</li></ul><ul></td><td>tbd</td></tr><tr><td>Good Night</td><td>
			Exactly at 10:00 PM
		</td><td><li>TODO: Check for summer hours Vs Winter hours</li></ul></td><td><ul><li>Turn OFF Family Room Lights</li><li>Turn OFF Kitchen Lights</li><li>Turn OFF Guest Bedroom Lights</li><li>Turn OFF Master Bedroom Lights</li><li>Turn OFF Office Room Lights</li><li>Turn OFF Basement Lights (TBD)</li><li>KEEP Front yard and Backyard lights for security reasons</li><li>Play 'Soft Kitty Warm Kitty Little Ball of Fur' Song :)</li></ul><ul></td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>
			motion sensor state changed
		</td><td><li>It is Dark outside</li><li>TV is ON</li><li>TV Room Lights are ON</li></ul></td><td><ul><li>Dim TV Lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>
			motion sensor state changed
		</td><td><li>It is Dark outside</li><li>TV is ON</li><li>TV Room Lights are ON</li></ul></td><td><ul><li>Dim TV Lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>
			motion detected
		</td><td><li>It is Dark outside</li><li>TV is ON</li><li>TV Room Lights are ON</li></ul></td><td><ul><li>Dim TV Lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Motion Detected - 2</td><td>
			motion detected
		</td><td><li>It is Dark outside</li><li>TV is ON</li><li>TV Room Lights are OFF</li></ul></td><td><ul><li>Dim TV Lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Motion Detected - 3</td><td>
			motion detected
		</td><td><li>It is Dark outside</li><li>TV is OFF</li><li>TV Room Lights are ON</li></ul></td><td><ul><li>Set the light brightness to 100%.</li></ul><ul></td><td>tbd</td></tr><tr><td>Motion Detected - 4</td><td>
			motion detected
		</td><td><li>It is Dark outside</li><li>TV is OFF</li><li>TV Room Lights are OFF</li></ul></td><td><ul><li>Set the light brightness to 100%.</li></ul><ul></td><td>tbd</td></tr><tr><td>NO motion sensed - 1</td><td></td><td><li>It is Dark outside</li><li>TV is ON</li><li>TV Room Lights are ON</li></ul></td><td><ul><li>Turn Lights OFF</li></ul><ul></td><td>tbd</td></tr><tr><td>NO motion sensed - 2</td><td></td><td><li>It is Dark outside</li><li>TV is OFF</li><li>TV Room Lights are ON</li></ul></td><td><ul><li>Turn Lights OFF</li></ul><ul></td><td>tbd</td></tr><tr><td>MQTT Announcements</td><td>
			When a message arrives in a specific topic
		</td><td><li>None</li></ul></td><td><ul><li>Read the text, call amazon polly to convert to audio/mp3 and Play the mp3 using media player</li></ul><ul></td><td>tbd</td></tr><tr><td>Check Battery Level of Phone</td><td>
			Battery level is below 30%
      device_tracker.suresh_suresh
      device_tracker.mallika_mallika
      device_tracker.hasika_hasika
      device_tracker.srinika_srinika
		</td><td><li>None</li></ul></td><td><ul><li>Send a notification</li></ul><ul></td><td>tbd</td></tr><tr><td>Check Battery Levels of Motion Sensors</td><td>
			Battery level is below 30%
      upstairs_motion_sensor
      downstairs_motion_sensor
		</td><td><li>None</li></ul></td><td><ul><li>Send a notification</li></ul><ul></td><td>tbd</td></tr><tr><td>Notify Home Security Status</td><td>
			Home Alarm system status changed
		</td><td><li>None</li></ul></td><td><ul><li>Send a notification</li></ul><ul></td><td>tbd</td></tr><tr><td>Home Security</td><td>
			Turn ON Home Alarm System when no one home
		</td><td><li>when all the members of family are "not home"</li></ul></td><td><ul><li>Turn ON home Security System</li></ul><ul></td><td>tbd</td></tr><tr><td>Flash Lights When Someone at the door</td><td>
			motion detected at the front door
		</td><td><li>when people are home</li></ul></td><td><ul><li>flash lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Play Dog Sounds</td><td>
			motion detected at the front door or back door
		</td><td><li>when no one at home</li></ul></td><td><ul><li>play dog barking sounds</li></ul><ul></td><td>tbd</td></tr><tr><td>Turn Humidifier ON automatically</td><td>
			Indoor humidity level is below threshold (30)
		</td><td><li>When people are home</li></ul></td><td><ul><li>Turn Humidifier On</li><li>Notify that the humidifier is turned ON, and remind to check water level</li></ul><ul></td><td>tbd</td></tr><tr><td>Turn Humidifier OFF automatically</td><td>
			Indoor humidity level is above threshold (30)
		</td><td><li>None</li></ul></td><td><ul><li>Turn Dehumidifier ON</li></ul><ul></td><td>tbd</td></tr><tr><td>Notify when someone arrives home</td><td>
			device_tracker.mallika_mallika
      device_tracker.suresh_suresh
      device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td><li>entered zone</li></ul></td><td><ul><li>Send an alert</li></ul><ul></td><td>tbd</td></tr><tr><td>Notify when someone arrives home</td><td>
			device_tracker.mallika_mallika
      device_tracker.suresh_suresh
      device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td><li>leave zone</li></ul></td><td><ul><li>Send an alert</li></ul><ul></td><td>tbd</td></tr><tr><td>Notify when Kids reach school</td><td>
			device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td><li>enter school zone</li></ul></td><td><ul><li>send an alert</li></ul><ul></td><td>tbd</td></tr><tr><td>Notify when Kids reach school</td><td>
			device_tracker.srinika_srinika
      device_tracker.hasika_hasika
		</td><td><li>leaves schol zone</li></ul></td><td><ul><li>Send an alert</li></ul><ul></td><td>tbd</td></tr><tr><td>Alert when everyone is away</td><td>
			group.all_devices
		</td><td><li>state changed to "not home"</li></ul></td><td><ul><li>Send an alert</li><li>Turn ON Home Security System</li><li>Turn down temperature?</li></ul><ul></td><td>tbd</td></tr><tr><td>Home Assistant Startup</td><td>
			event_type is homeassistant_start
		</td><td><li>None</li></ul></td><td><ul><li>Send an alert</li></ul><ul></td><td>tbd</td></tr><tr><td>New Home Assistant Update</td><td>
			updater.updater
		</td><td><li>None</li></ul></td><td><ul><li>Send an alert with link to HA</li></ul><ul></td><td>tbd</td></tr><tr><td>Timer enabled smart Switch</td><td>
			light status is On
		</td><td><li>for a certain time</li><li>during day time</li></ul></td><td><ul><li>Turn off light</li></ul><ul></td><td>tbd</td></tr><tr><td>Weather - Heavy Wind Alerts</td><td>
			Entity - sensor.dark_sky_wind_speed
		</td><td><li>Wind speed is aboive 20 and below 40</li></ul></td><td><ul><li>Send an alert</li><li>flash lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Weather - Super Heavy Winds</td><td>
			sensor.dark_sky_wind_speed
		</td><td><li>Wind speed is aboive 40</li></ul></td><td><ul><li>Send an alert to stay indoors</li><li>Announce in the house</li><li>Flash lights</li></ul><ul></td><td>tbd</td></tr><tr><td>Provide Daily Weather Update</td><td>
			at 7:00 AM
		</td><td><li>None</li></ul></td><td><ul><li>Send an Alert</li><li>Announce in the house</li></ul><ul></td><td>tbd</td></tr><tr><td>Greet Family Members</td><td>
        device_tracker.mallika_mallika
        device_tracker.suresh_suresh
        device_tracker.srinika_srinika
        device_tracker.hasika_hasika
		</td><td><li>for 2 minutes</li></ul></td><td><ul><li>Announce, Welcome, family member!</li></ul><ul></td><td>tbd</td></tr><tr><td>Z-wave</td><td>
			at 4:30 in the morning
		</td><td><li>None</li></ul></td><td><ul><li>Heal Z-Wave network</li></ul><ul></td><td>tbd</td></tr></table>
