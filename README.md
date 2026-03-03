## My Slicemk Ergodox setup steps

Even though all docs can be found [here](https://docs.slicemk.com/), I'm outlining the steps I took when setting this up, for my own future reference.

1. I had to unpair the dongle and have the left half be the central: https://docs.slicemk.com/firmware/zmk/wireless/nvsclear/

2. Each half has a user button and a reset button. The reset button is on the RIGHT of the usb port when it's facing up. The user button is on the left.

3. The user button can turn off the keyboard, and pressing the reset button once can turn it on. Double pressing the reset button twice within 500 ms turns on the bootloader mode.

4. If you connect either half to a device via usb while it's in bootloader mode, it will show up as a usb media device, which can have files uploaded to / downloaded from. 

5. Right half is always a peripheral device, and left side is the central if not using a dongle.

6. Make sure to flash the right side with the right image (peripheral image) and the left side with the output from the zmk layout editor.
