# Getting the Software

There are two pieces of (free) software you'll need, along with the default code I've written for you. Our first battle will be successfully programming your Teensy with the code I provide. Once you've succeeded, make sure to take a moment and be proud of this! It isn't a small thing.

## Arduino IDE (integrated development environment)
Follow this link and download the latest version of the Arduino IDE for your operating system.

_If you are on a Mac, make sure to move the downloaded app to your **Applications** folder._
_For Windows, I recommend the Installer version, so follow installation instructions after download._
(**Arduino Download Page**)[https://www.arduino.cc/en/Main/Software]

Got it? Great! Next task!

## Teensyduino Addon
Again, follow the link and download the version for your operating system. For Windows and Mac you'll want to double-click the download and run the installer.

(**Teensyduino Download Page**)[https://www.pjrc.com/teensy/td_download.html]

_For Mac, it will ask you to **Select Arduino Folder**. Assuming you moved it to the **Applications** folder, you can scroll down until you fine **Arduino.app/**, select it, and click next._

Allow it to install all the options it wants and close it once it is complete.

Just one more thing to download!

## The Code
This is a direct link, so it will download a zip file to your computer.

[**TeensyLC Code Download**](keyboard-default-teensylc.zip)

Find wherever it downloads and unzip the file. It should create a folder called _keyboard-default-teensylc_ with a file inside called _keyboard-default-teensylc.ino_.

You **must** leave that file in the folder. Arduino requires that the code files (they call them sketches) is always named the same as the folder it in inside.

Nervous yet? Time to fire things up!

## Uploading the Code

1. Hopefully you still have the _keyboard-default-teensylc.ino_ file visible. If not, find it again.
1. Oh, don't worry about the code for now. You don't even need to think about changing the code, not until after we have some buttons working!
1. Double-click it. That should trigger the Arduino software to open (if it warns you about it being an application downloaded from the internet, just click _open_).
1. Find your Teensy and a micro-USB cable.
1. Plus the small end of the cable into the Teensy, the large end into your computer.
1. With the Arduino IDE in focus, and the _keyboard-default-teensylc.ino_ file open, you are ready to select the appropriate settings to write the code.
1. Click the Tools menu, then hover over Boards, and select **Teensy LC**. This should stay the default from now on, but if you are ever having problems, it is worth double checking.
1. Click the Tools menu, then hover over USB Type, and select Serial + Keyboard + Mouse + Joystick. This should encompass all of the types of controls we will be emulating over the semesters. Again, this should stay default, but if you have problems, double check the setting.
1. Do you see the check mark in the upper left? And the arrow next to it? If you click the check mark it will try to _compile_ the code and let you know if it is valid. If it isn't, it'll spit out some error messages. Clicking the arrow compiles and then tries to put the code on the Teensy.
1. Let's start with just verifying the code compiles. Click the check mark! It should be since I already wrote and tested it! Watch the console (the bottom black space), and if all goes well you shouldn't get any errors.
1. If you **do** get errors, make sure you set the board type properly (step 6) and the USB type properly (step 7).
1. Compiled ok (you think)? Let's try to write the code to the Teensy! It's time to click the **arrow** in the upper-left next to the check mark.
1. If it seems to wait and then prints an error in the console like, _"Teensy did not respond to a USB-based request to automatically reboot. Please press the PROGRAM MODE BUTTON on your Teensy to upload your sketch."_, try pressing the tiny white button on your Teensy, and click the arrow button again.
1. If it still doesn't work, make sure the USB cable is properly connected from the computer to the Teensy.
1. Still nothing? Try another cable! They are made cheaply and I've lost a lot of time on bad cables in the past!
1. When it _does_ upload to the Teensy, another small application called _Teensy_ might pop open for a moment, or stay open. Don't worry about this little helper, it is your friend. You can safely close it at any time if you aren't using the Arduino IDE.
1. If successful, it should say _Done Uploading._ on the greenish bar above the console (the bottom dark space with text).

Did it work?!? Holy crap! This is huge! Seriously, if you haven't done much or anything with electronics, getting your environment properly set up to code tiny computers is a big deal! Be proud of yourself because you now have a tiny HID emulator pretending to be a keyboard!

Let's hook up a button and see something **happen**! After that, we'll take a step back to learn more about the Teensy and what else we can do with the code, but you deserve to experience the fruits of your labor. <3