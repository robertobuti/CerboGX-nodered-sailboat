# CerboGX-nodered-sailboat
User interface for nodered on sailboat with Victron CerboGX
I have realized this simple UI using large image with node-red on CerboGX, my sailboat use Victron system, this project can easy adapted on your requirements.
Interface use : Raspberry with WiFi (in my case PiB+ it's enought) with wifi connection, but if your prefere also wired Ethernet can be used as well.
Display it's classic Pi 5" MipiDSI IPS with touch screen, like this one : https://www.amazon.it/Ingcool-Raspberry-Touchscreen-Capacitivo-Supporta/dp/B0B4W7TB9J/ref=sr_1_4_pp?dib=eyJ2IjoiMSJ9.p8W85TfMX3fecv2KTSoro-e1RTQWaWp3jMnG3YekElsJRgfGS-GjaA5TIBXWfiyEThWuTuPV9uzgMDlOyJbKBrRKmFr_Ch7EbwX3y2l7FErkFVSPXXNmH-lGdkcKmVii.5lLGI_H4KVJDFnyesT8jvCgABeWj9iJJltSsIgOlabw&dib_tag=se&keywords=Ingcool&qid=1749720719&sr=8-4&th=1
Glass is very thin, touch have some working problem when glued to the panel, so a palstic chassis 3D printed has been added, on that i apply also a switch to power-on /off the unit.
Note, PI work at 5V only, so a dc/Dc converter need to  be used from 12V to 5V, any one you have / find can be used.

steps : install raspi on your PI, you will need to install :
Install chromium (browser), x11 server utils and unclutter (hide the cursor from the screen)
You find many guide on google to make this, then add on autostart the batch kiosk.sh , here i have used mDNS name to call Nodered ui, but depend from your local lan, if direct connection without router you will  need to set fixed ip on CerboGX and change "venus.local" on batch file with CerboGX Ip.
I have used portrait layout for display, but this it's again a yoru choise.

Nodered project is very simple, obviously is for my boat configuration, it's easy to adapt on your system.
Enjoy.
![20250424_224849](https://github.com/user-attachments/assets/97a7e817-3c49-479f-a38a-c65ad2ae0ea4)
