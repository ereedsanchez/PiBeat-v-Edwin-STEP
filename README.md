# PiBeat v. STEP Summer

A browser based Drum Sequencer to control your Raspberry Pi robotic drum machine from your computer, tablet, mobile etc.

#### Original Instruction

[See the Instructable](https://www.instructables.com/id/A-Raspberry-Pi-Powered-Junk-Drum-Machine/) on how to
create your own drum machine and how to use this project, or take a look [here](http://www.banjowise.com/post/automabeat/) for additional documentations.  Links are from orginal creator of the PiBeat, 

The PiBeat software is standard Angular app communicating with a Python backend using Web Sockets pn the Raspberry Pi. The Python server is found in server.py. Pi-Beat also a physical computing robot that plays real everyday items as drums. 

#### Kits
Each student group receives a PiBeat kit that includes the following. 
[Link to kit Student Kits - Part List](PiBEAT-Parts)
- 1 - Raspberry Pi
- 1 - MicroSD Card
- 1 - 5v 8 channel relay
- 1 - Pack of female to female jumper wires (10 wires needed)
- 2 - 3 Amp Terminal strips
- 1 - 12v 10a Power Supply
- 8 - 12v 2a Solenoids
- 8 - 1N5401 Rectifier diodes

- 3 - Mini Screwdrivers

#### Misc Classroom Materials
- 5 - MicroSD Card Reader



### Class Sessions 


#### Session 1 - Raspberry Pi
- Download Raspberry Pi Imager [Link](https://www.raspberrypi.com/software/)
- On SDcard install Raspberry Pi OS Legacy (Buster with Desktop Environment)
  - In the Setting add the following:
  - Set hostname [your group's name]
  - Enable SSH
  - setup username: pi  password: pipi
  - configure wireless lab:  SSID: [ask professor]  Password: [ask professor]
  - Set local settings: New York
 
- SSH into Pi, using Terminal(Mac) or CMD(Windows)
  - Ask the professor for your IP address, by telling him what hostname you used.
  - In Terminal/CMD type the following command:    `ssh pi@[ip-address]`
  - You should receive: `Are you sure you want to continue connecting (yes/no/[fingerprint])?`
  - type `yes`
  - You should receive: `password:`
  - type `pipi`   (you will not see pipi on screen and the cursor will not move)
 
Enable VNC 
VNC will allow you to remotely see the desktop of your raspberry pi computer. 
- In the Pi terminal type: `sudo raspi-config`
- you will get a visual menu (Use the arrow keys and enter to navigate)
- Navigate to `interface options` , `P3 VNC` , enable `yes`

Connect to Pi with VNC
- Download and install VNC Viewer on your computer. [Link](https://www.realvnc.com/en/connect/download/viewer/)
- Open VNC Viewer
  - In the top bar it will say: `Enter a VNC server Address`
  - Enter: `[your IP address]`
  - You will be asked again if you trust the connection. Press `yes`
  - input Login: `pi`, Password: `pipi`
You should now be able to see your Pi's desktop.

#### Pi First configurations
- Welcome to Raspberry Pi,
- Next: Set the country to NY, USA,
- Change Password, `pipi`
- Setup screen, just press `next`
- Select Wifi Network: Skip
- Update software: Skip
- Setup complete: Done

#### Session 2 - Connect Pi to Relay

#### Session 3 - Relay to Solenoids

#### Session 4 - Sounds 


#### Session 5 - Server
to ru the server u zip the piBeatServer.tar file.






#### Edwin's WIP notes

- Angular app not working on RPi 3B+
- Added additional python rythem scripts.

#### Beat Tools
- https://drumbit.app/
- https://drumbit.club/
- https://io808.com/
