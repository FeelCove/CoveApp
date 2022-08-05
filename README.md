# CoveApp
Cove application and firmware.

This document explains how to manually upgrade the firmware on your Cove device. This requires the installation of the Cove development application (apk).

Because we are no longer providing support for the Cove application, there is no need to have the sensors and data logging active in your device as this will decrease the battery life.

## Downloading and installing Android apk

- Download the android_dev.apk file from /apk folder to your mobile device.
- Locate the apk file on your mobile device after downloading it.
- Select the file and choose “Install”.
- Find and tap the 'Cove DEV' app icon; the main screen is shown below. No need to login to the app, as we just want to get to the development console.
![Main Screen](/images/main_screen.png)


- To open the development console tap 5 times on the main screen with 2 fingers, and then select 'START' button next to 'Eagle Command Client' as shown below.
![Command Client](/images/eagle_command_client.png)


- After selecting 'START', the development app will request the necessary permissions, choose 'While using the app' option.
![App permissions](/images/alllow_permissions.png)

- The development console is now active (as shown below), and we can now connect to the Cove device. See next section: [Upgrading firmware with apk](#upgrading-firmware-with-apk) to follow the instructions for connecting and upgrading the firmware on your Cove device.
![Dev Console](/images/development_console.png)

## Upgrading firmware with apk

- Download the firmware file [eagle_oad_2.10.1.bin](/firmware/eagle_oad_2.10.1.bin) onto your mobile device.
- Install the Android apk [android_dev.apk](apk/android_dev.apk) on your mobile device. See section [Downloading and installing Android apk](#downloading-and-installing-android-apk) above.
- If you have multiple Cove devices then ensure that all over Cove devices, except for the one that you wish to upgrade, are off or far away from the area in which you'll be working.
- From the development console, swipe right to open the menu and press on the 'CONNECT' button, as shown below. While the device and phone are trying to connect, Android will ask you to if you want to 'Pair and Connect' to Cove, choose 'Yes'.
![Dev Console Connect](/images/dev_console_menu_connect.png)
- The connection state should be shown as 'Registering' when the phone and Cove are trying to connect:
![Connecing](/images/device_connecting.png)
- You may need to repeat the 'Connect' step twice, if Cove gets disconnected by the phone. When the phone and Cove are connected the development console will look as follows:
![Connected](/images/device_connected.png)

- Swipe right to open the console menu again, scroll down all the way to the bottom and select 'PERFORM OAD WITH EXTERNAL FILE'.
![OAD](/images/flash_reset_version_oad.png)
- Select the eagle_oad_2.10.1.bin file downloaded (on the first step above) to upgrade the device to this version. The Cove LED should start blinking white when upgrading the firmware. It is advised not to switch away from the app screen to another app during this process and not allow your phone to fall asleep, as it could disrupt the upgrade process. This process should take 2 - 4 minutes. Upon successful upgrade, the device will disconnect, turn off, and then turn back on.
- Also, if the OAD process was successfully started, then it should say so in the console window as shown below:
![OAD started](/images/oad_started.png)

- To reconnect to the device, swipe right to open the app menu, select 'Connect' and wait until the phone and Cove are connected. Swipe right again to open the menu, scrolling all the way to the bottom, select "GET VERSION" to confirm successful update to version 2.10.1.
![Get version](/images/get_version.png)

- Next, erase Cove external flash to delete any old session files. To do this swipe right again to open the menu, scroll down all the way to the bottom and select 'FLASH RESET'. The Cove LED should start blinking white. Please wait until LED stops blinking white to start using the device.
![Flash reset](/images/flash_reset.png)

- You can now start using your Cove!
