MARS - McNeese Augmented Reality Sandbox
The McNeeese Augmented Reality Sandbox is an interactive sandbox with an augmented-reality topology map and water simulation. This project is based on the original UC Davis AR sandbox.

Links to documentation on the original UC Davis AR sandbox
Link to the UC Davis-hosted instructions and software setup.

https://arsandbox.ucdavis.edu/instructions/

Link to the UC Davis-hosted AR sandbox forum.

https://arsandbox.ucdavis.edu/forums/forum/ar-sandbox-forum/

Link to a step-by-step software setup video.

http://youtu.be/R0UyMeJ2pYc

Extremely detailed step-by-step software installation instructions:

https://web.cs.ucdavis.edu/~okreylos/ResDev/SARndbox/LinkSoftwareInstallation.html

Differences between original UC Davis AR sandbox and MARS
MARS is currently using Linux Mint 19.3 (MATE desktop). Like the original, we are using a first-generation Kinect unit as the IR camera.

(Unverified) MARS is running on an HP Z4/Z6 Workstation, link here.

Special documentation
All USB devices must be plugged into the BACK of the computer tower, not in the front.
Previous versions of the rig used a mirror, and a command was used to flip the screen display. Hopefully, the new rig won't require any mirrors, but for documentation's sake, the command(s) were listed here. https://askubuntu.com/questions/19936/how-can-i-mirror-flip-display-output
On Linux Mint 19.3 Mate, there is a freezing issue that occurs in the VRUI when holding down a key. Possible solutions include switching to 19.1 Mate, 19.3 Cinnamon, or editing the VRUI config to disable pointer grabbing. To disable pointer grabbing:
Edit the VRUI config:
sudo nano /usr/local/etc/Vrui-4.6/Vrui.cfg
Find the section called "MouseAdapter" and insert the following line:
grabPointer false
Then save the file.
If getting an "Interface 0 is already claimed","Error while setting alternate setting", or a LIBUSB error after hanging, see the following links:
https://arsandbox.ucdavis.edu/forums/topic/usb-or-kinect-error-interface-0-is-already-claimed/#post-102835
https://arsandbox.ucdavis.edu/forums/topic/error-when-running-kinectutil/
https://stackoverflow.com/questions/6365314/libusb-interface-already-claimed
