# Linux-Battery-Notification
Receive an alert, when the battery level is above 95% or below 20%

This shell script runs in the background on startup and checks the battery status every minute and then sends a notification when the battery level is charged above 95% or discharged less than 20%.

The alert will not get turned off, until your battery is over 20% or less than 95% charged.

Once the script is ready, set the executable permission.


Steps to install:

1. $ sudo chmod +x /opt/scripts/battery-status.sh


Finally, add the script to the bottom of the user profile file. For system-wide users, add the script on the /etc/profile file. This profile file will allows the system to kick the script when the system starts.


2. $ vi ~/.profile 

sh /opt/scripts/battery-status.sh &


Reboot your Linux system to verify the notification status.

3. $ sudo reboot

