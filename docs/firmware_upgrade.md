## Upgrading firmware with apk

- Download the firmware file [eagle_oad_2.10.1.bin](/firmware/eagle_oad_2.10.1.bin) onto your mobile device.
- Install the Android apk [android_dev.apk](apk/android_dev.apk) on your mobile device. See section [Downloading and installing Android apk](docs/download_install_apk.md) above.
- Connect Cove to the development app. See [Connecting Cove to Android development app](docs/connecting.md) above.
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

### Notes
- See [Troubleshooting](docs/troubleshooting) section if you experience any issues after upgrading the device to firmware version 2.10.1.
