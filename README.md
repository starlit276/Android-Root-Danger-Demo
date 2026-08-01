# Demonstration-of-Dangerous-Commands-on-Rooted-Android-Devices

This project safely demonstrates the potential consequences of executing untrusted shell scripts with root privileges on Android devices.

The script is designed for educational and research purposes only. It does not perform any destructive operations.

## Disclaimer

This project is provided for educational and research purposes only.

This project demonstrates concepts related to Android root environments, Linux block devices, and potentially dangerous commands. It does not intentionally modify, erase, or damage any device data.

The author assumes no responsibility or liability for any damage, data loss, device malfunction, or other consequences caused by the use, modification, or misuse of this project.

Users are responsible for understanding the risks associated with root access and privileged operations.

Use this project at your own risk.

## How It Works

This script demonstrates the potential risks of running untrusted shell scripts with root privileges on Android devices.

The script works as follows:

1. Detects available block devices under `/dev/block/`.
2. Checks the number of detected partitions for each device.
3. Simulates the type of destructive commands that could be executed by a malicious or unsafe script.
4. Displays the possible consequences without actually modifying, erasing, or writing data to any storage device.

The script does not execute any `dd` commands or perform any destructive operations.

## Technical Background

Android devices expose storage devices through Linux block device interfaces.

Paths such as `/dev/block/sdX` represent storage devices, while `/dev/block/by-name/` provides human-readable names for partitions.

Commands that directly write to block devices can potentially overwrite system partitions, boot partitions, or user data partitions if misused.

## Testing

This script has been tested on my personal Android device with root privileges enabled.

The test was completed successfully, and no data loss, system damage, or device malfunction occurred during testing.

However, different Android devices may have different partition layouts and configurations. Successful testing on one device does not guarantee the same result on other devices.
