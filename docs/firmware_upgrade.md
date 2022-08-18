## Upgrading firmware with Android development app

1. Download the firmware file [eagle_oad_2.10.1.bin](../firmware/eagle_oad_2.10.1.bin) onto your mobile device.
2. Install the Android apk [android_dev.apk](../apk/android_dev.apk) on your mobile device. See section [Downloading and installing Android apk](download_install_apk.md).
3. Connect Cove to the development app. See [Connecting Cove to Android development app](connecting.md).
4. After connecting Cove to the app, tap the gear icon in the top-left corner to access the menu.
5. At the bottom of the menu, locate the option to “Perform OAD with External File”

  <img src="/images/flash_reset_version_oad.png" width="200" height="400">

6. To begin the upgrade, select the eagle_oad_2.10.1.bin file to you previously downloaded.
  - If the app is not allowing you to select the bin file, navigate to other paths in the folder, and then go back to where the file is located.
  - The LED will blink white for 2-4 minutes while the upgrade installs.
  - During the upgrade process, do not navigate away from this screen, and do not allow the phone to enter sleep mode.
  - Once complete, the LED will return to pulsing green.


7. Reconnect Cove to the app.

8. At the bottom of the menu, tap “GET VERSION” to confirm the upgrade succeeded.  The correct version is 2.10.1.

  <img src="/images/get_version.png" width="200" height="400">

9. Finally, at the bottom of the menu, tap “FLASH RESET”.  Cove will begin blinking white while resetting.  Upon returning to a green LED, Cove is ready for use.

<img src="/images/flash_reset.png" width="200" height="400">

See [Troubleshooting](troubleshooting.md) section if you experience any issues after upgrading the device to firmware version 2.10.1.
