### My Automation Catalogue:

<table><tr><th>Automation</th><th>Platform</th><th>Trigger</th><th>Condition</th><th>Action</th><th>Link</th></tr><tr><td>Outdoor Turn Lights ON 15 minutes before sunset</td><td>sun</td><td>sun is below horizon or event is sunset
      offset -15 minutes</td><td></td><td><ul><li>Turn Light(s) ON</li><li>Send an alert</li></ul></td><td>tbd</td></tr><tr><td>Outdoor Turn Lights OFF 15 minutes after sunrise</td><td>sun</td><td>sun is 'above horizon' or event is sunrise
      offset +15 minutes</td><td>Every day</td><td>Turn Light(s) OFF</td><td>tbd</td></tr><tr><td>Turn Home Security System ON at Sunset</td><td>Sun</td><td>event is sunset</td><td>Do it only when people are at home
      Weekdays ONLY
      Home Security System is Disarmed</td><td><ul><li>Turn ON Home Security System in 'Home' mode</li><li>Send an alert</li><li>Drop a message in the announcement queue</li></ul></td><td>tbd</td></tr><tr><td>Kitchen Lights on early morning during school days</td><td>time</td><td>exactly at 5:30 AM</td><td>Weekdays (mon, tue, wed, thu, fri)
        Only during school days check (if school days input_boolean is ON)</td><td>turn kitchen lights ON</td><td>tbd</td></tr><tr><td>Master Bedroom lights ON (wife's side)at 5:20</td><td>time</td><td>Exactly at 5:20 AM</td><td>Only during Weekdays (mon, tue, wed, thu, fri)
      Only during school days check (if school days input_boolean is ON)</td><td>Turn ON wife's side of the bed lamp at 10% brightness with transition of 1 minute from 0 to 10% brightness</td><td>tbd</td></tr><tr><td>Master Bedroom lights OFF (wife's side)at 5:45</td><td>time</td><td>Exactly at 5:45 AM</td><td>Only during Weekdays (mon, tue, wed, thu, fri)
      Only during school days check (if school days input_boolean is ON)</td><td>Turn OFF wife's side of the bed lamp with no transition</td><td>tbd</td></tr><tr><td>Master Bedroom lights ON at 6:59 AM</td><td>time</td><td>Exactly at 6:59 AM</td><td>Only during Weekdays (mon, tue, wed, thu, fri)</td><td>Turn ON Master Bedroom lights with transition of 2 minutes at 25% brightness
      Announce daily weather updates, commute to work...etc on home audio system</td><td>tbd</td></tr><tr><td>Master Bedroom Lights OFF at 9:00 AM</td><td>time</td><td>Only during Weekdays (mon, tue, wed, thu, fri)</td><td>Week days</td><td>Turn off master bedroom lights
      TODO: Check device_tracker and the location, When Suresh leaves home, turn off master bedroom lights immediately</td><td>tbd</td></tr><tr><td>Turn Kitchen Lights OFF at 8:15 AM</td><td>time</td><td>Exactly at 8:15 AM</td><td>Everyday - it is usually bright enough in Kitchen at 8:15 AM</td><td>Turn OFF kitchen lights</td><td>tbd</td></tr><tr><td>Dim Kitchen lights 15 minutes before bed time</td><td>time</td><td>Exactly at 9:45 PM. (Our bed time is at 10:00 PM)</td><td>Make sure the light is ON before dimming</td><td>Turn ON the light and set the brightness of the light to 15%</td><td>tbd</td></tr><tr><td>Turn ON Home Security System at Bedtime</td><td>time</td><td>Exactly at 10:00 PM</td><td>People MUST be home
      Home Security System cannot be in AWAY mode
      Home Security System MUST BE Disarmed</td><td>Turn ON Home Security System in HOME mode
      Send an alert
      Make an annnouncement inside the house</td><td>tbd</td></tr><tr><td>Good Night</td><td>time</td><td>Exactly at 10:00 PM</td><td>TODO: Check for summer hours Vs Winter hours</td><td><ul><li>Turn OFF Family Room Lights</li><li>Turn OFF Kitchen Lights</li><li>Turn OFF Guest Bedroom Lights</li><li>Turn OFF Master Bedroom Lights</li><li>Turn OFF Office Room Lights</li><li>Turn OFF Basement Lights (TBD)</li><li>KEEP Front yard and Backyard lights for security reasons</li><li>Play 'Soft Kitty Warm Kitty Little Ball of Fur' Song :)</li></ul></td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>state</td><td>motion sensor state changed</td><td>It is Dark outside
      TV is ON
      TV Room Lights are ON</td><td>Dim TV Lights</td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>state</td><td>motion sensor state changed</td><td>It is Dark outside
      TV is ON
      TV Room Lights are ON</td><td>Dim TV Lights</td><td>tbd</td></tr><tr><td>Motion Detected - 1</td><td>state</td><td>motion detected</td><td>It is Dark outside
      TV is ON
      TV Room Lights are ON</td><td>Dim TV Lights</td><td>tbd</td></tr><tr><td>Motion Detected - 2</td><td>state</td><td>motion detected</td><td>It is Dark outside
      TV is ON
      TV Room Lights are OFF</td><td>Dim TV Lights</td><td>tbd</td></tr><tr><td>Motion Detected - 3</td><td>state</td><td>motion detected</td><td>It is Dark outside
      TV is OFF
      TV Room Lights are ON</td><td>Set the light brightness to 100%.</td><td>tbd</td></tr><tr><td>Motion Detected - 4</td><td>state</td><td>motion detected</td><td>It is Dark outside
      TV is OFF
      TV Room Lights are OFF</td><td>Set the light brightness to 100%.</td><td>tbd</td></tr><tr><td>NO motion sensed - 1</td><td>state</td><td></td><td>It is Dark outside
      TV is ON
      TV Room Lights are ON</td><td>Turn Lights OFF</td><td>tbd</td></tr><tr><td>NO motion sensed - 2</td><td>state</td><td></td><td>It is Dark outside
      TV is OFF
      TV Room Lights are ON</td><td>Turn Lights OFF</td><td>tbd</td></tr><tr><td>MQTT Announcements</td><td>MQTT</td><td>When a message arrives in a specific topic</td><td></td><td>Read the text, call amazon polly to convert to audio/mp3 and Play the mp3 using media player</td><td>tbd</td></tr><tr><td>Check Battery Level of Phone</td><td>numeric_state</td><td>Battery level is below 30%
      device_tracker.suresh_suresh
      device_tracker.mallika_mallika
      device_tracker.hasika_hasika
      device_tracker.srinika_srinika</td><td></td><td>Send a notification</td><td>tbd</td></tr><tr><td>Check Battery Levels of Motion Sensors</td><td>numeric_state</td><td>Battery level is below 30%
      upstairs_motion_sensor
      downstairs_motion_sensor</td><td></td><td>Send a notification</td><td>tbd</td></tr><tr><td>Notify Home Security Status</td><td>state</td><td>Home Alarm system status changed</td><td></td><td>Send a notification</td><td>tbd</td></tr><tr><td>Home Security</td><td>state</td><td>Turn ON Home Alarm System when no one home</td><td>when all the members of family are "not home"</td><td>Turn ON home Security System</td><td>tbd</td></tr><tr><td>Flash Lights When Someone at the door</td><td>state</td><td>motion detected at the front door</td><td>when people are home</td><td>flash lights</td><td>tbd</td></tr><tr><td>Play Dog Sounds</td><td>state</td><td>motion detected at the front door or back door</td><td>when no one at home</td><td>play dog barking sounds</td><td>tbd</td></tr><tr><td>Turn Humidifier ON automatically</td><td>state</td><td>Indoor humidity level is below threshold (30)</td><td>When people are home</td><td>Turn Humidifier On
      Notify that the humidifier is turned ON, and remind to check water level</td><td>tbd</td></tr><tr><td>Turn Humidifier OFF automatically</td><td>state</td><td>Indoor humidity level is above threshold (30)</td><td></td><td>Turn Dehumidifier ON</td><td>tbd</td></tr><tr><td>Notify when someone arrives home</td><td>zone</td><td>device_tracker.mallika_mallika
      device_tracker.suresh_suresh
      device_tracker.srinika_srinika
      device_tracker.hasika_hasika</td><td>entered zone</td><td>Send an alert</td><td>tbd</td></tr><tr><td>Notify when someone arrives home</td><td>zone</td><td>device_tracker.mallika_mallika
      device_tracker.suresh_suresh
      device_tracker.srinika_srinika
      device_tracker.hasika_hasika</td><td>leave zone</td><td>Send an alert</td><td>tbd</td></tr><tr><td>Notify when Kids reach school</td><td>zone</td><td>device_tracker.srinika_srinika
      device_tracker.hasika_hasika</td><td>enter school zone</td><td>send an alert</td><td>tbd</td></tr><tr><td>Notify when Kids reach school</td><td>zone</td><td>device_tracker.srinika_srinika
      device_tracker.hasika_hasika</td><td>leaves schol zone</td><td>Send an alert</td><td>tbd</td></tr><tr><td>Alert when everyone is away</td><td>state</td><td>group.all_devices</td><td>state changed to "not home"</td><td>Send an alert	
      Turn ON Home Security System
      Turn down temperature?</td><td>tbd</td></tr><tr><td>Home Assistant Startup</td><td>event</td><td>event_type is homeassistant_start</td><td></td><td>Send an alert</td><td>tbd</td></tr><tr><td>New Home Assistant Update</td><td>state</td><td>updater.updater</td><td></td><td>Send an alert with link to HA</td><td>tbd</td></tr><tr><td>Timer enabled smart Switch</td><td>state</td><td>light status is On</td><td>for a certain time
      during day time</td><td>Turn off light</td><td>tbd</td></tr><tr><td>Weather - Heavy Wind Alerts</td><td>state</td><td>Entity - sensor.dark_sky_wind_speed</td><td>Wind speed is aboive 20 and below 40</td><td><ul><li>Send an alert</li><li>flash lights</li></ul></td><td>tbd</td></tr><tr><td>Weather - Super Heavy Winds</td><td>state</td><td>sensor.dark_sky_wind_speed</td><td>Wind speed is aboive 40</td><td>Send an alert to stay indoors
      Announce in the house
      Flash lights</td><td>tbd</td></tr><tr><td>Provide Daily Weather Update</td><td>time</td><td>at 7:00 AM</td><td></td><td>Send an Alert
      Announce in the house</td><td>tbd</td></tr><tr><td>Greet Family Members</td><td>state</td><td>device_tracker.mallika_mallika
        device_tracker.suresh_suresh
        device_tracker.srinika_srinika
        device_tracker.hasika_hasika</td><td>for 2 minutes</td><td>Announce, Welcome, family member!</td><td>tbd</td></tr><tr><td>Z-wave</td><td>time</td><td>at 4:30 in the morning</td><td></td><td>Heal Z-Wave network</td><td>tbd</td></tr></table>
