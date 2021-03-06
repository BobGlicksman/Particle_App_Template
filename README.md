﻿# Particle_App_Template
## MIT App Inventor 2 program that serves as a template for creating apps that communicate with a Particle Photon or Electron.

This project provides a template for creating apps that can communicate with Particle devices (e.g. Photon, Electron) over the Internet, 
via the Particle Cloud.  The template, as well as apps that will be created from it, is written in MIT App Inventor 2 
(http://ai2.appinventor.mit.edu).  MIT App Inventor 2 (AI2) is an easy-to-use, graphical programming system that is completely web based
and requires no complex IDE installation.  At present, AI2 allows the user to create Android apps; however, the MIT team has announced 
plans to support iOS in 2018.  Furthermore, the AI2 apps can be run on Windows and Mac OSX via readily available Android emulators for 
these operating systems.

The template provides an app developer with a main screen (Screen1) that is largely blank and available for project-specific app 
development.  However, opening the app to this screen automatically retrieves the user's Particle user access_token and last
selected Particle device_ID from internal app storage (tinyDB).  The app automatically "pings" this default device and reports its
current status (online or offline).  A "Refresh" button is provided on Screen1 for the user to ping this device at any time to ensure
that it is online and thus able to communicate with the app.

The user can also tap "Setup", which takes the user to a Device Setup Screen where the user can provide their Particle login ID
and password and use these to query the Particle Cloud for a list of all devices in the user's Particle account.  The user can then
select the device that they wish to use with the app from a pick list, and the user and device credentials are then stored in the app's
persistent storage (tinyDB) as the future default when opening the app.

The concept is for an app developer to make a copy of the source code file (.aia), name this file for their project, and open the
project in AI2.  The developer can then add their project code (in AI2) to Screen1, using the global variables for user_token
and device_ID to communicate with the selected Particle device.  An example of how to communicate with a Particle device to
read device variables from the Particle Cloud and call device functions via the Particle Cloud can be found in the project:

https://github.com/TeamPracticalProjects/MIT-App-Inventor-Particle-Photon-test

NOTE:  This project uses an AI2 extension “TaiFun Tools” from Pura Vida Apps (https://puravidaapps.com/extensions.php).  You should not need to install this extension if you download the .aia file from this repository into your MIT App Inventor 2 IDE.  However, you should definitely check out all of the amazing extensions on this site and while you are there, please make a small donation to support Pura Vida Apps (Team Practical Projects has nothing to do with this site, but we respect it immensely).

All materials contained in this repository are (c) 2018 by Bob Glicksman,
Jim Schrempp and Team Practical Projects and are distributed freely under
an open source, non-commercial license, see: https://creativecommons.org/licenses/by-nc/4.0/.  Use of the material in this repository is subject to the document “Terms_of_Use_License_And_Disclaimer”, included in this repository.

Enjoy,
Team Practical Projects
