Heart rate monitoring video capture device instructions

author: @arii

To run the heart rate software you need to have a Bluetooth capable device.  Open the following website in chrome to see if you can pair with your heart rate monitor:

[Heartrate demo app](/heart-rate-sensor)

The rest of the instructions describe how to make the chrome window show up side by side with the video camera to use in zoom.

----


Install OBS studio and OBS virtual camera.  You will also need to install a virtual studio runtime sdk provided by micorsoft for free.  

Direct links for windows 10  (accessed June 2020):
* [Windows OBS Studio 25.0.8](https://cdn-fastly.obsproject.com/downloads/OBS-Studio-25.0.8-Full-Installer-x64.exe)
* [OBS Virtual camera plugin]( https://github.com/Fenrirthviti/obs-virtual-cam/releases/download/2.0.5/obs-virtualcam-2.0.5-Windows-installer.exe)


Open up OBS studio but skip the auto streaming setup wizard.

In the upper toolbar select tools -> virtual camera
 --> select auto start and target camera to OBS Camera 

In the upper toolbar select Scene collection.  A pop will ask if you want it to auto import select yes. 
 In the second window press the '...' button to navigate to this folder.  Choose the json file titled "cameranchrome.json"

In the lower left corner there should be a box called "scenes" and "sources".  These are the two main boxes you will use.

# step 1 configure your camera, logo, and chrome

under sources in the lower left side of OBS studio (next to scenes) choose the "video capture device". 
 Click the gear tab to choose your video camera input

# Put up a fancy icon
Under the image within sources choose a file path to a cool image

Open a chrome window. If it doesn't show up within the obs studio screen, 
then select Window capture and configure the window selection.  You should be able to choose a different application.


# choosing sceens	

You can cycle through camera + small right chrome, 
camera + large right chrome
camera
and chrome only by clicking the scene name


# open the bluetooth application
In this folder open the "heart-rate-sensor" folder and click on index.html.  If chrome is your default browser, it should
open automatically; otherwise right click to open with chrome.  
On the chrome window click the heart. Assuming your computer/phone has ble it will try to pair with a heart rate device

# In zoom choose the camera titled 'OBS studio'

Enjoy your workout!

----

Original bluetooth application created by [WebBluetoothCG](https://github.com/WebBluetoothCG/demos).

[OBS Studio](https://obsproject.com/)

[OBS virtual cam](https://github.com/Fenrirthviti/obs-virtual-cam)

