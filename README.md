# dell chromebook 11 wolf

## Enable dev mode
* To enable dev mode follow steps from https://www.chromium.org/a/chromium.org/dev/chromium-os/developer-information-for-chrome-os-devices/dell-chromebook-11
* If your device is locked, that means enterprise enrolled. Try to login via google account because there is a chance that previous owner let device off. It is necessary because information is stored in bios so making your account an owner gives you permission to enable dev mode
* If device is **still owned by another company** then you have to contact them and ask for enabling it

## Installing coreboot and seabios
* After sucessfully enabling dev mode, setup root password, login as guest and hit alt+ctrl+f2 (or forward arrow). 
* In terminal login as root using previous password.
* enter:  `cd; curl -LO https://mrchromebox.tech/firmware-util.sh && sudo bash firmware-util.sh`
* choose: `Install/Update Custom coreboot Firmware (Full ROM)`
* Install Gnu/Linux :) (**do not** runubiquity with -b flag)

### sudo usermod -a -G dialout $USER
