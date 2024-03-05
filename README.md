# wifi_check
Check whether a particular wifi is connected and reconnect if it isn't connected.  

The raspberry pi is already connected to a wpa2 enterprise network, but keeps disconnecting frequently.  
So, I wrote this script to check if the wifi is connected. If it is not, then we use nmcli to reconnect to it. 
This script is added to crontab with sudo permissions after giving it executable rights, so that it runs continuously in the background.  

You will have to replace expected ssid, wifi interface, as required.
