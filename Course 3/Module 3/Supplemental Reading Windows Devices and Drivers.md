
 For an Introduction to Plug and Play click [here](https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/introduction-to-plug-and-play).

As discussed in the previous lecture video, when Windows notices that a new device has been connected, the first thing it will do is ask the device that's been plugged in for it's Hardware ID. For more information on hardware identification click [here](https://docs.microsoft.com/en-us/windows-hardware/drivers/install/step-1--the-new-device-is-identified).

Once Windows has the Hardware ID of the new device, the OS uses that ID to search for the right driver for the device, For more information on this click [here](https://docs.microsoft.com/en-us/windows-hardware/drivers/install/hardware-ids).

It looks in a few places for the driver, starting with a local list of well-known drivers, then going onto Windows Update or the Driver Store. For more information click [here](https://docs.microsoft.com/en-us/windows-hardware/drivers/install/step-2--a-driver-for-the-device-is-selected).