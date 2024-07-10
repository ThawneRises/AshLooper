# AshLooper

## Description:
AshLooper is a comprehensive module designed to address boot loop issues caused by problematic modules installed via KernelSU or Magisk on Android devices.

### Functionality:
- **Boot Loop Detection:** AshLooper monitors the boot process and checks for boot loops caused by malfunctioning modules.
- **Boot Attempt Count:** It keeps track of the number of boot attempts by incrementing a counter stored in the `module.prop` file.
- **Threshold Control:** AshLooper allows users to set a threshold for the number of permissible boot attempts before taking action.
- **Mode Selection:** Users can now select between two modes of operation:
  - **Disable Modules Mode:** Disables the problematic modules without rebooting into recovery mode.
  - **Disable Modules & Reboot Recovery Mode:** Disables the problematic modules and reboots the device into recovery mode.

## How it Works:
1. **Boot Process Monitoring:** AshLooper actively monitors the boot process of the device.
2. **Boot Attempt Tracking:** Upon each boot attempt, AshLooper incrementally updates the boot attempt count stored in the `module.prop` file.
3. **Threshold Check:** AshLooper compares the current boot attempt count with the predefined threshold.
4. **Threshold Exceeded:** If the boot attempt count surpasses the threshold, AshLooper takes action based on the selected mode:
   - **Disable Modules Mode:** AshLooper disables the problematic modules without rebooting into recovery mode, allowing the device to boot normally.
   - **Disable Modules & Reboot Recovery Mode:** AshLooper disables the problematic modules and reboots the device into recovery mode to prevent the device from getting stuck in a boot loop and facilitate troubleshooting.

## KernelSU and Magisk Support:
- AshLooper seamlessly integrates with both KernelSU and Magisk, ensuring comprehensive support for a wide range of Android devices and module configurations.

## Disclaimer:
Use AshLooper responsibly and at your own risk. The developer assumes no responsibility for any damage or issues arising from its use.

## Reporting Issues and Contributions:
If you encounter any problems or have suggestions for improvement, please report them by opening an issue or submitting a pull request on GitHub. Your contributions are welcome and appreciated.

## Support:
For inquiries, troubleshooting, and support, please contact [Ripper Hybrid](https://t.me/Ripper_Hybrid) on Telegram.