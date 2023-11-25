# ARM.Chromebook

# Development Mode
Enable:
- https://www.wikihow.com/Enable-USB-Booting-on-Chromebook

# Information: **`Ctrl + I`**

# Boot from SD Card or USB: **`Ctrl + U`**
works!: `Ctrl + U`
sch: https://www.google.com/search?q=chromebook+arm+boot+linux+sd+card
- guide: https://www.reddit.com/r/chrultrabook/comments/ov0t5s/keeping_chrome_os_and_booting_linux_from_an_sd/
- https://www.reddit.com/r/chromeos/comments/rzy4py/how_to_boot_linux_from_usb_on_arm_chormebook/


Enable:
- https://www.wikihow.com/Enable-USB-Booting-on-Chromebook
- sch: https://www.google.com/search?q=chromebook+enable+usb+boot
- discuss: https://groups.google.com/a/chromium.org/g/chromium-os-discuss/c/UEIwMszxxpM?pli=1

```
# press Ctrl + Alt + T
shell
sudo su -
crossystem dev_boot_usb=1
```

# Restore: ChromeOS
https://support.google.com/chromebook/answer/1080595


# Enable: Sudo
- sch: https://www.google.com/search?q=The+%22no+new+privileges%22+flag+is+set%2C+which+prevents+sudo+from+running+as+root.

## Problem: Ver. 117.n Removed sudo!
### Solution:
- https://github.com/dnschneid/crouton/discussions/5005

>Sudo commands will not succeed by default. If you want to use sudo commands, use the VT-2 shell (Ctrl-Alt-{F2/Right arrow/Refresh}) or build the image with the login_enable_crosh_sudo USE flag:
>
>`$ USE=login_enable_crosh_sudo emerge-$BOARD chromeos-login`
>or
>`$ USE=login_enable_crosh_sudo cros build-packages --board=$BOARD`
  https://www.reddit.com/r/Crouton/comments/15aiy80/sudo_cant_enter_chroot_after_update_26_july_2023/
- https://support.google.com/chromebook/thread/238102666/sudo-does-not-work

