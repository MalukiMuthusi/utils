# Emulator command in the android command line tools

Emulator tool is used to manager virtual android emulators. It can start a virtual device, list all the virtual devices installed in the computer and perform other tasks.

1. Start an emulator from the command line.
   `emulator -avd {avd-name} [options]`
   or
   `emulator @avd-name [options]`
   example
   `emulator @Pixel_2_API_30`

2. To list avd names
   `emulator -list-avds`
