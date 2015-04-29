# WatchDog
Overview: WatchDog app for Pebble Watch.

Design: This app was designed by Ryan Smith, Theresa Breiner and Brad Thompson.

Use: Application for Pebble watch. Allows the user to monitor temperature and a motion sensor remotely by using a custom server and Arduino microcontroller. 

Server is run from the command line from file WatchDog.cpp. It takes the desired port number as a command line argument. 

Pebble files are installed directly or via CloudPebble.net. The app will then appear in the scrolling menu on the watch.

App allows users to view most recent temp reading (uses automatic polling), change display on watch and Arduino between celsius and fahrenheit, view high/low/avg temperatures for the last hour, put the Arduino in standby mode and stop reading and motion sensor monitoring, receives an alert if motion sensor is tripped, send scrolling warning message to display on the Arudino 7-segment display, reset alarm remotely. See the user guide in the Docs folder for details.

Other Info: Technical documentation and user guide included.

Citations by file:
WatchDog.cpp: Fundamental server operations were borrowed from the following 2 sources: 1 - http://www.prasannatech.net/2008/07/socket-programming-tutorial.html
2 - http://www.binarii.com/files/papers/c_sockets.txt
This is mostly found in function server_thread between lines 320-355 and in function main between lines 498-503.
main.c: The majority of this code come from I2C_7SEG_Temperature.pde, Copyright 2008, Gravitech. Original file modified to contain all functionality mentioned in description except reading and transmitting the temperature and displaying celsius temp reading on 7-Seg display. The majority of these alterations occur within the infinite loop in the loop() function.
lab.js: Initial skeleton and onload method provided by Dr. Chris Murphy in this assignment.
WatchDog.ino: Initial skeleton for app_event_loop and basic send/receive functions provided by Dr. Chris Murphy in this assignment.