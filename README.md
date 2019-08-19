# CR10S-Pro-BL-Touch-Install-Guide
How to flash the LCD and Firmware for the BL touch on the CR10S-Pro

### IMPORTANT: On our youtube video of this installation, there is no prompt for flashing the Marlin firmware required for this modification. You may flash Marlin using the instructions below at any time, and it is mandatory for this modification to work. 

## Flashing The LCD

1) Visit InsanityAutomation's Marlin Creality_DWINTEST Github branch here: https://github.com/InsanityAutomation/Marlin/tree/Creality_DWINTest
2) At the top right hand of the page, click "Clone or Download" - download the zip file to your computer 
3) Unzip the Folder
4) Insert your MicroSD card into your computer. Format the drive with an 'Allocation Unit Size' of 4096. 
5) Browse the 'Marlin-Creality_DWINTest' folder,  then '10sPro_1.70_ScreenFiles'. You will find a folder called 'DWIN_SET'. Copy the 'DWIN_SET' folder on your SD card (folder and all).
6) Eject your SD card. Return to the YouTube video. 

## Flashing Marlin 

### Download and Configure Arduino 
1) Download and install the Arduino IDE from: https://www.arduino.cc/en/Main/Software
2) Open the Arduino IDE. Under File > Preferences, tick off "Show verbose output" during both compilation and upload.  Also tick off "Display Line Numbers".
3) Plug your printer into your computer.
4) Configure for upload. From Tools > Board Select "Arduino/Genuino Mega or Mega 2560". From Tools > Port select the COM port for your Arduino. It will probably be the only one listed. If there are multiple ports, try uploading to a different port if the selected one doesn't work.

### Configuring and Uploading Marlin

1) Open 'Marlin.ino' located in the 'Marlin-Creality_DWINTest' >>>> 'Marlin' folders that you downloaded in the instructions above. 
2) When the software loads, click the green 'Configuration.h' tab.
3) Around line 98, you will see '//#define ABL_BLTOUCH' - remove the two slashes in the front to enable this setting.
4) Go to Sketch > Upload.

You should see the program compile properly and upload to the board. Please return to the YouTube video. 

