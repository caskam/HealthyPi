The board is pre-loaded with the firmware which works stand alone with the Rpi with fewer setup. However you will need some software. Here's what we're using:

* **Atmel Studio 7** :
Please note that Atmel Studio 7 does not support Mac and Linux . This is the IDE software that can do step & memory debugging and its only for Windows. Also you have to make an account on Atmel's site. The IDE can be downloaded from [Atmel Studio's Official Website](http://www.atmel.com/tools/atmelstudio.aspx)

**Load the Healthy Pi Source Code**

* **Step 1 :** Start by launching Atmel Studio 7.

* **Step 2 :** Open the Project [navigate the path where the project is saved].

* **Step 3 :** You'll see the following, where the sketch is in a window, you can edit the code here if you like.

**Debugger**

You need a debugger to load the code into the SAMD21G18A. Atmel-ICE will help get from here http://www.atmel.com/tools/atatmel-ice.aspx

**Step 1 : Set Up and Check Interface**
* Attach the chip & debugger

**Step 2 : Identify Interface**
* OK now you have your debugger plugged in, its good to check that it works, select Device Programming.
* Choose "Device Programmer" from "Tools" Menu
* Programming window will be open.
* Select the programmer from the drop down box. Select interface as “SWD”. Click on “Apply”.
* Now read the Power and Device ID. If you are able to read the Device ID then the interface is fine.

**Step 3 : Build & Start Debugging**
* Ok close out the modal programming window and build the program. If there are no error, then your build will be successful.

**Step 4 : Run & Upload**
* You will see a window appearing to select a debugging tool. Select the tool and interface.
* Once done, go back and Re-run Program without debugging.