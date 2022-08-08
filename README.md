# CoveApp

This document explains how to manually upgrade the firmware on your Cove device. This requires the installation of the Cove development application (apk).

Because we are no longer providing support for the Cove production app, there is no need to have the sensors and data logging active in your Cove device as this will decrease the battery life on the device. Both firmware images located under [/firmware](/firmware/) do not require the use of the production app. However, the [eagle_oad_2.10.1.bin](/firmware/eagle_oad_2.10.1.bin) firmware is the image that disables the sensors and data logging to extend battery life.

## Downloading and installing Android development apk

- Download the android_dev.apk file from /apk folder to your mobile device.
- Locate the apk file on your mobile device after downloading it.
- Select the file and choose “Install”.
- Find and tap the 'Cove DEV' app icon; the main screen is shown below. No need to login to the app, as we just want to get to the development console.
<img src="/images/main_screen.png" width="200" height="400">

- To open the development console tap 5 times on the main screen with 2 fingers, and then select 'START' button next to 'Eagle Command Client' as shown below.
<img src="/images/eagle_command_client.png" width="200" height="400">

- After selecting 'START', the development app will request the necessary permissions, choose 'While using the app' option.
<img src="/images/alllow_permissions.png" width="200" height="400">

- The development console is now active (as shown below), and we can now connect to the Cove device. See next section: [Upgrading firmware with apk](#upgrading-firmware-with-apk) to follow the instructions for connecting and upgrading the firmware on your Cove device.
<img src="/images/development_console.png" width="200" height="400">

## Connecting Cove to Android development app

- Install the Android apk [android_dev.apk](apk/android_dev.apk) on your mobile device. See section [Downloading and installing Android apk](#downloading-and-installing-android-apk) above.

- If you have multiple Cove devices then ensure that all other Cove devices, except for the one that you wish to upgrade, are off or far away from the area in which you'll be working.

- Connect the Cove device to the USB charger. The LED should start blinking green. However, the LED may remain solid green if the device is fully charged.

- From the development console, swipe right to open the menu and press on the 'CONNECT' button, as shown below. While the device and phone are trying to connect, Android will ask you to if you want to 'Pair and Connect' to Cove, choose 'Yes'.
<img src="/images/dev_console_menu_connect.png" width="200" height="400">

- The connection state should be shown as 'Registering' when the phone and Cove are trying to connect:
<img src="/images/device_connecting.png" width="200" height="400">

- You may need to repeat the 'Connect' step twice, if Cove gets disconnected by the phone. When the phone and Cove are connected the development console will look as follows:
<img src="/images/device_connected.png" width="200" height="400">

## Unlocking the Cove device
- Install the Android apk [android_dev.apk](apk/android_dev.apk) on your mobile device. See section [Downloading and installing Android apk](#downloading-and-installing-android-apk) above.

- Connect Cove to the development app. See [Connecting Cove to Android development app](#connecting-cove-to-android-development-app) above.

## Upgrading firmware with apk

- Download the firmware file [eagle_oad_2.10.1.bin](/firmware/eagle_oad_2.10.1.bin) onto your mobile device.
- Install the Android apk [android_dev.apk](apk/android_dev.apk) on your mobile device. See section [Downloading and installing Android apk](#downloading-and-installing-android-apk) above.
- Connect Cove to the development app. See [Connecting Cove to Android development app](#connecting-cove-to-android-development-app) above.
- Swipe right to open the console menu again, scroll down all the way to the bottom and select 'PERFORM OAD WITH EXTERNAL FILE'.
<img src="/images/flash_reset_version_oad.png" width="200" height="400">
- Select the eagle_oad_2.10.1.bin file downloaded (on the first step above) to upgrade the device to this version. The Cove LED should start blinking white when upgrading the firmware. It is advised not to switch away from the app screen to another app during this process and not allow your phone to fall asleep, as it could disrupt the upgrade process. This process should take 2 - 4 minutes. Upon successful upgrade, the device will disconnect, turn off, and then turn back on.
- Also, if the OAD process was successfully started, then it should say so in the console window as shown below:
<img src="/images/oad_started.png" width="200" height="400">

- To reconnect to the device, swipe right to open the app menu, select 'Connect' and wait until the phone and Cove are connected. Swipe right again to open the menu, scrolling all the way to the bottom, select "GET VERSION" to confirm successful update to version 2.10.1.
<img src="/images/get_version.png" width="200" height="400">

- Next, erase Cove external flash to delete any old session files. To do this swipe right again to open the menu, scroll down all the way to the bottom and select 'FLASH RESET'. The Cove LED should start blinking white. Please wait until LED stops blinking white to start using the device.
<img src="/images/flash_reset.png" width="200" height="400">

- You can now start using your Cove!

### Troubleshooting

### Notes
- If you experience any issues with firmware version 2.10.1, then you can follow the same steps to downgrade to version 2.10.0, which is the latest firmware version released to customers. See [Upgrading firmware with apk](#upgrading-firmware-with-apk).
