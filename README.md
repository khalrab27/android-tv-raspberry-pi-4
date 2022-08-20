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
    - Scroll down to "Install Raspberry Pi OS using Raspberry Pi Imager".
    - Download and install using the appropriate file for your operating system.
  
  - LineageOS 18.1
    - This is a custom build of LineageOS made by KonstaKang, optimised for larger screens and remotes.
    1. Go to [this link](https://konstakang.com/devices/rpi4/LineageOS18-ATV/).
    2. Scroll down and press the _first_ download link, not the second.  
    ![LineageOS Screenshot](https://user-images.githubusercontent.com/73562639/185755231-0e25899d-5963-4b30-894b-eeba4c0e4ebb.png)
  
  - GApps
    - This is a way to get Google apps for the LineageOS build.
    1. Go to [this link](https://opengapps.org/).
    2. Under "Platform", choose ARM64.
    3. Under "Android", choose 11.0.
    4. Under "Variant", choose tvstock.  
    ![GApps Screenshot](https://user-images.githubusercontent.com/73562639/185755318-926d500e-bfd7-4953-8549-8f97a5982b0a.png)
    5. Press the download button.
    6. After download is completed, move the file to your USB.

## Flash LineageOS onto SD card

1. Plug your SD card into your computer.
2. Open Raspberry Pi Imager.
3. Press "Choose OS".
4. Scroll down and choose the "Use custom" option.
5. Select the LineageOS file and press "Open".
6. Press "Choose Storage".
7. Select your SD card.
_If you're using Ethernet to connect the Pi, skip to step 10._
8. Press the settings icon.
9. Here, you will need to enable some options:
  - Check "Configure wireless LAN".
  - Set "SSID" to the name of the Wi-Fi network the Pi will connect to.
  - Set "Password" to your Wi-Fi password.
  - Under "Wireless LAN country", you will need to enter your two-digit country code. (Look for your country and the corresponding code in [this list](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2#Officially_assigned_code_elements).
  - Leave all the other options to their default and press "Save".
10. Press "Write".  
**WARNING: All data previously on the SD card will be lost!**
11. After it's done, insert SD card into Raspberry Pi. (The SD card automatically ejects after it's done)

## Set up LineageOS

1. Connect your Raspberry Pi with your monitor, plug it in, and wait for it to boot.
2. 
