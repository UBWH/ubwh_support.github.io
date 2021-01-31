# Using the Ubiquiti airGateway Pro-Installer as a PoE Powered WiFi Access Point (AP)
![AGProIns Image](../images/AGproINS.png)

The [airGateway Pro-Installer](https://ubwh.com.au/Ubiquiti/Accessories/AG-PRO-INS) can be easily configured as standard WiFi AP, making it suitable for applications that need:
* A small, cheap AP
* PoE powered (24V PoE)

## Instructions
1. Download the [config file](../AGinsAP.cfg) to your laptop/tablet
1. Start with the unit in Factory Default mode
1. Connect an ethernet cable between:
   * A 24V PoE supply (Pins 4,5 (+DC)  7,8 (-DC)
   * The POE OUT socket on the unit. (That is not a type: Yes - connect to POE OUT)
1. Using a laptop/tablet: Connect using WiFi to the SSID that looks like `airGateway:xxxxxxxxxxxx`  (xxx=MAC address)
1. Using a web browser, visit `http://192.168.1.1`
   * Login:    ubnt
   * Password: ubnt
   * Country: select as needed
   * I Agree to .... : checked
   * Login
1. Go to the SYSTEM Tab
   * Upload the AGinsAP.cfg file downloaded above
   * Apply
   * Wait until unit reboots. It will reboot with an IP address aquired from the local DHCP server.
1. Using a laptop/tablet: Connect using WiFi to the SSID that looks like `www.ubnt.com`
   * Login:    ubnt
   * Password: ubnt
1. Go to the WIRELESS tab
   * SSID: Change to the WiFi SSID you want
   * Security: Enabled
   * Password: Change to the WiFi password you want
   * Apply
   * Wait until unit reboots
1. Login again and go to the SYSTEM tab
   * System Accounts: Click the picture of the key
   * Current password: `ubnt`
   * New password: enter new password
   * Verify New password: enter new password
   * Click: Channge
   * Click: Apply
  
The unit should now behave as a simple AP. 

  
