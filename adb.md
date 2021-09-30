# ADB command hacks

Android Debug Bridge is a tool used to connect android device to a PC. It also refers to the adb protocol. It enables developers to install applications and access the phone's shell from their connected computer.

You can launch the shell in the phone by running
`adb shell`

## To connect to adb over tcpip protocol

1. Connect the phone to the PC over the cable first
2. Enable ADB over tcpip.
   `adb tcpip port` where port is e.g 5555

3. Then unplug the device.
4. Connect to adb
   `adb connect PHONE_IP:PORT` PHONE_IP is the local ip address; PORT is the port number you set above.

Note: The phone and the PC must be connected to the same local network.

## To copy files from the phone to computer

`adb pull path_to_file path_to_store_the_file`

## To copy files from computer to phone

`adb push path_to_file path_to_store_the_file`
