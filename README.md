# Android TV on Raspberry Pi

## What you need

- Raspberry Pi
  - I'm using a Raspberry Pi 4 Model B with 2 GB RAM. You can use Raspberry Pi 4 Model B or Raspberry Pi 400. I recommend at least 4 GB RAM for better performance.

- Micro SD Card (at least 16 GB)

- Micro SD to USB adapter

- Power Supply for Raspberry Pi (recommended to use official power supply)

- Ethernet Cable or Wi-Fi

- USB (at least 4 GB)

- Mouse & Keyboard

- Monitor
  - If you don't have a monitor, you can use your TV.

- micro-HDMI to HDMI cable

- Raspberry Pi case with fan (optional)

## Software
  
  - Raspberry Pi Imager
    - Go to [this link](https://www.raspberrypi.com/software/).
    - Scroll down to _Install Raspberry Pi OS using Raspberry Pi Imager_.
    - Download and install using the appropriate file for your operating system.
  
  - LineageOS 18.1
    - This is a custom build of LineageOS made by KonstaKang, optimised for larger screens and remotes.
    1. Go to [this link](https://konstakang.com/devices/rpi4/LineageOS18-ATV/).
    2. Scroll down and press the _first_ download link, not the second.  
    ![LineageOS Screenshot](https://user-images.githubusercontent.com/73562639/185755231-0e25899d-5963-4b30-894b-eeba4c0e4ebb.png)
  
  - GApps
    - This is a way to get Google apps for the LineageOS build.
    1. Go to [this link](https://opengapps.org/).
    2. Under _Platform_, choose ARM64.
    3. Under _Android_, choose 11.0.
    4. Under _Variant_, choose tvstock.  
    ![GApps Screenshot](https://user-images.githubusercontent.com/73562639/185755318-926d500e-bfd7-4953-8549-8f97a5982b0a.png)
    5. Press the download button.
    6. After download is completed, move the file to your USB.

## Flash LineageOS onto SD card

1. Plug your SD card into your computer.
2. Open Raspberry Pi Imager.
3. Click _Choose OS_.
4. Scroll down and choose the _Use custom_ option.
5. Select the LineageOS file and press _Open_.
6. Click _Choose Storage_.
7. Select your SD card.
8. Click _Write_.  
**WARNING: All data previously on the SD card will be lost!**
. After it's done, insert SD card into Raspberry Pi. (The SD card automatically ejects after it's done)

## Set up LineageOS

1. Connect your Raspberry Pi with your monitor, plug it in, and wait for it to boot.
2. When it boots, you'll get a message saying _Searching for accessories_. Press F2 (or fn + F2) on your keyboard to get rid of it.
3. Click the _Start_ button.
4. Click _Accept_.
5. Keep all the settings as default.
If connected by Ethernet, skip to step 15.
6. Choose your Wi-Fi network and enter the password to connect to it.  
You can use either the physical keyboard or the on-screen keyboard.
The _Next_ button won't work if you try to press it. Press Enter on your keyboard to go to the next step.
7. You can select or deselect the diagnostics option based on your preferences. Press _Next_.
8. Click _Start_.

## Flash GApps to LineageOS

The next steps require a keyboard.
The keyboard controls are:
- Arrow keys to navigate the interface
- Enter to click on something
- F1 to go to the home page
- F2 to go back
- F5 to turn off the screen
- F11 to decrease the volume
- F12 to increase the volume  

1. Insert the USB that has GApps into the Pi.
2. Use the arrow keys to click the settings icon. (up, right, right, enter)
3. Click _System_. (down until you neach _System_, enter)
4. Click on _Buttons_. (down, enter)
5. Press Enter to enable the _Advanced reboot_ option.
6. Press F2 and go down to the _Reboot_ option and press Enter.
7. Choose the _Recovery option_ and press Enter.
8. Wait for it to reboot.  

The next few steps require a mouse.
9. Click _Install_.
10. Click _Select Storage_.
11. Click _USB_ and then _OK_.
12. Click on the GApps file.
13. Leave everything as default and swipe the blue arrows.
14. Wait for it to complete.
15. Click _Reboot_ and choose _System_.

## Setting up Android TV

1. You will get a prompt for setting up a remote. Press F2 to ignore it, or you can set up an IR remote if you have one.
2. Choose your language from the options.
3. You will get a prompt to quickly set up your TV with your Android phone. You can continue with this option, but I will skip it in this tutorial.
4. The Wi-Fi should be connected automatically so press _Continue_.  
If you want to change the Wi-Fi, press _Change network_, otherwise press _Continue_.
5. Press _Sign in_ and sign in with your Google account using either the physical keyboard or the on-screen keyboard.
6. Accept Google's _Terms of Service_.
7. You can allow or deny access to location based on your preferences.
8. You can allow or deny diagnostics based on your preferences.
9. Press _Continue_.
10. Press _Continue_ again.
11. You can allow or deny personal results with Google Assistant based on your preferences.
12. You can allow or deny emails about Google Assistant based on your preferences.
13. Press the arrow at the bottom of the screen to go through the features of Android TV.  
Due to limitations in the Raspberry Pi, Chromecast Built-in unfortunately isn't available.

14. You're done setting up Android TV!

## Get started using Android TV

- You can use your phone as a remote for Android TV using [this guide](https://support.google.com/googletv/answer/11136134).
- If you have a case with a fan for your Raspberry Pi, you can enable overclocking to get the most out of the Pi's CPU.
  - Go to Settings.
  - Click on _System_.
  - Click on _Raspberry Pi settings_.
  - Under the _Overclock_ section, press _Maximum CPU frequency_ and change it to whatever you see fit.

### Thank you for reading my guide. For any suggestions, please make an issue.
