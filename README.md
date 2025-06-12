**User Interface for Node-RED on a Sailboat with Victron CerboGX**

I created this simple user interface using a large background image and Node-RED running on a CerboGX. My sailboat uses a Victron energy system, but this project can be easily adapted to your specific needs.

**Components Used:**

* **Raspberry Pi with WiFi**: I used a Pi B+, which is more than enough. If you prefer, you can also use a wired Ethernet connection.
* **Display**: A standard 5" MIPI DSI IPS touchscreen display, easily found on Amazon.
* **Display Mount**: The touchscreen glass is very thin and may have responsiveness issues when glued directly to a panel. To solve this, I designed a 3D-printed plastic chassis. I also added a power switch to this mount for turning the unit on and off.
* **Power Supply**: The Raspberry Pi operates at 5V, so you’ll need a DC/DC converter to step down from 12V to 5V. Any model you have or can find will work fine.

**Setup Steps:**

1. Install Raspberry Pi OS on your Pi.
2. Install the following software packages:

   * Chromium browser
   * X11 server utilities
   * Unclutter (to hide the mouse cursor)
3. You can find many guides online for setting this up.
4. Add your `kiosk.sh` script to the autostart configuration.
5. In the script, I used the mDNS name `venus.local` to reach the Node-RED UI, but this depends on your network setup.

   * If you're using a direct connection without a router, you’ll need to set a static IP on the CerboGX and replace `venus.local` in your script with that IP address.
6. I’ve set the display to portrait mode, but you can choose the orientation that best fits your layout.

**About the Node-RED Project:**

The Node-RED flow is very simple and tailored to my boat’s configuration. However, it can be easily modified to suit your own setup.

**Enjoy!**

![20250424_224849](https://github.com/user-attachments/assets/97a7e817-3c49-479f-a38a-c65ad2ae0ea4)
<img width="824" alt="Cattura" src="https://github.com/user-attachments/assets/a47abd8d-2923-4c8f-921d-e5b0164b1166" />
