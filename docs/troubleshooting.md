# Troubleshooting

| Problem     | Solution      |
| ------------- | ------------- |
| LED blinks amber for a few secs after single pressing the power button          | See [Unlocking the Cove device](device_unlocking.md)         |
| LED blinks red for a second or so after single pressing the power button           | This means that the device battery doesn't have enough charge to run a session. Please fully charge the device to clear this error. The LED will change from blinking green to solid green when fully charged, and it will automatically turn off after 3 mins in this state         |
|The device will not power ON with a long press (~3 secs) of the power button or when plugging in the USB charger | This may be an issue with the battery being depleted, but the issue may be fixed by a 1) soft reset, 2) factory restore. See [Device Reset](device_reset.md)|
|The device remains ON even after 3 minutes of the session ending or when long pressing the power button (~3 secs) | This could mean that the firmware is unresponsive. Wait at least 30 secs, and if the issue doesn't clear on its own, then perform a device soft reset. See [Device Reset](device_reset.md)|
| Cannot feel the vibrations even though device is snug on the back of your head| a) Remove the device, and check if you can feel the vibrations with your fingers. b) If you can feel the vibrations with your fingers then you need to make sure there are no gaps between the vibration points and the back of your ears. c) If you cannot feel the vibrations with your fingers then try performing a soft reset. See [Device Reset](device_reset.md). d) If the soft reset doesn't fix the issue the issue may be hardware related |
|Cannot connect to the development app | Remove Cove from your list of Bluetooth devices under the phone Bluetooth settings. See [Connecting Cove to Android development app](connecting.md) for more information on how to connect Cove to the development app|
|For other unexplained behavior not covered above|If you are experiencing any other issues that may be causing the device to become unresponsive, then perform a factory restore. See [Device Reset](device_reset.md) for details|

### Notes
- If you wish to downgrade your device to the latest firmware released to customers (2.10.0) then follow the same steps described under [Upgrading firmware](firmware_upgrade.md), but using the [eagle_oad_2.10.0.bin](../firmware/eagle_oad_2.10.0.bin) image instead.
