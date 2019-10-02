---------- Welcome to BlueSn0w ----------

This pre-release is a Bluetooth Stumbler that will find the MAC address of any discoverable Bluetooth device within the area. This is the first stage of development at www.iBluetoothProject.tk and as we continue to work to create the ultimate Bluetooth solution for the iPhone.


PLEAE NOTE THE FOLLOWING BEFORE USE:

**It does not have an icon**
As of yet, there is no icon or GUI for this app, you can only run it through Terminal. 

**You cannot run this app via remote SSH**
When using Bluetooth on the iPhone, it uses the same channel as the phone's WiFi. When running the app, the phones WiFi is disabled. Because of this the app will not show expected results over remote SSH, and must be done locally.


Below are step-to-step instructions on how to run this app:

1. Using SSH or your usual transfer method, transfer the bin file (named bluesn0w and is located in this folder along with this ReadMe) to the iPhone. 
You can place the file anywhere on your iPhone, but it is suggested to be placed in /var/root/

2. Install MobileTerminal via Cydia if not already done so.

3. Run Terminal from your SpringBoard.

4. SSH into the iPhone as root with this command: 
     $ SSH -l root localhost

5. Enter your password to login. If unchanged, it will be alpine.

6. You must set permissions of 777 to the bluesn0w file using chmod. Use this command, but if your didn't place bluesn0w in the root directory, replace the location with your own:
     $ chmod -R 777 ./bluesn0w

7. You are now ready to run the app! Use this command, or if you palce the file in another locations, once again, replace it with your own:
     $ ./bluesn0w


There you go, they app will scan for 10 seconds and print the MAC address any devices in close range. 

Please sign up to out forum at www.iBluetoothProject.tk and if you can spare some cash, donate to the project to help further development and creating a better iPhone Bluetooth solution



**CREDITS**
App coded by: Schmave
ReadMe written by: MattMac
Forum hosted by: luiz
Thenk-you too all our donors so far!