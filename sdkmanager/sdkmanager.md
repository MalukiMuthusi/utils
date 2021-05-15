# sdkmanager

sdkmanager is command line tool used to install update, upgrade and uninstall tools that are used in developing android applications.

1. To install a list of tools from a text file
   `sdkmanager --package_file=opensource\utils\sdk-install.txt`
   The items to be installed should be written each on its own line.

2. To view list of items available for installation
   `sdkmanager --list`

3. To install a single item
   `sdkmanager "ndk;20.0.5594570"`
   `"ndk;20.0.5594570"` refers to the path column when you run `sdkmanager --list`
