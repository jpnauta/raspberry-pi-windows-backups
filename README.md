> Tips and tricks to backup your computer(s) using Raspberry Pi

## Summary

This simple tutorial uses [Raspberry Pi][raspberrypi], [Open Media Vault][openmediavault] and [Windows Backup and Restore][windowsbackuprestore] to create a low-cost backup server comparable to Apple's [Time Machine][timemachine].

## The Hardware 

To build your NAS server, you will need:

- 1x Raspberry Pi 3 with SD card (<$100)
- 1x External backup drive ($50)
- 1x USB hub with bus power ($20)

You will also need a Windows 10 or MacOS computer to setup your Raspberry Pi, and one or more Windows 10 computers to back up to.

## Procedure

### Step 1: Install Open Media Vault on Raspberry Pi

To back up our files, we will need to mount a network drive to your Windows computer(s). [Open Media Vault][openmediavault] is a simple OS for hosting network files you can install on a Raspberry Pi that can help accomplish this.

To set up Open Media Vault on your Pi, follow [The Pi's great tutorial][the-pi-tutorial]. It is recommended that you use a USB hub with bus power to connect your external hard drive to your Raspberry Pi, as the Pi's bus power typically does not provide enough power to power most hard drives, and will cause errors during setup.

### Step 2: Configure Windows Backup Restore

Once you have your Raspberry Pi mounted as a network drive, you can use [Windows Backup and Restore][windowsbackuprestore] to back up your computer. Be sure to use your network drive (e.g. `Z://`) as your backup drive.

[raspberrypi]: https://www.raspberrypi.org/
[openmediavault]: https://www.openmediavault.org/
[windowsbackuprestore]: https://support.microsoft.com/en-ca/help/17127/windows-back-up-restore
[timemachine]: https://www.apple.com/ca/airport-time-capsule/
[the-pi-tutorial]: https://thepi.io/how-to-use-your-raspberry-pi-as-a-nas-box/
