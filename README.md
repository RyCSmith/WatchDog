# WatchDog
Overview: WatchDog app for Pebble Watch.

Design: This app was designed by Ryan Smith, Theresa Breiner and Brad Thompson.

Use: Application for Pebble watch. Allows the user to monitor temperature and a motion sensor remotely by using a custom server and Arduino microcontroller. 

Server is run from the command line from file WatchDog.cpp. It takes the desired port number as a command line argument. 

Pebble files are installed directly or via CloudPebble.net. The app will then appear in the scrolling menu on the watch.

App allows users to view most recent temp reading (uses automatic polling), change display on watch and Arduino between celsius and fahrenheit, view high/low/avg temperatures for the last hour, put the Arduino in standby mode and stop reading and motion sensor monitoring, receives an alert if motion sensor is tripped, send scrolling warning message to display on the Arudino 7-segment display, reset alarm remotely. See the user guide in the Docs folder for details.

Other Info: Technical documentation and user guide included.