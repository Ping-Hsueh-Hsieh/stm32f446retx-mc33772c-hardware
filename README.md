# TODO

- [x] fill region: In1.Cu with GND
- [x] change 16MHz crystal to 8MHz, since 8MHz is cheaper and more available.
- [x] USB OTG FS: VBUS senisng
- [ ] stitching & fencing vias
- [x] shrink the board

# Sources

- [step-by-step tutorial](https://github.com/gt-marine-robotics-group/kicad-tutorial)
- [video](https://fedevel.com/blog/kicad-stm32-hardware-design-an-overview-in-20-minutes-phils-lab-15)
- [kicad footprints](https://gitlab.com/kicad/libraries/kicad-footprints)
- [reverse engineering KiCad Project from Gerber file](https://forum.kicad.info/t/reverse-engineering-kicad-project-from-gerber-files/30903)
- [STM32H742Vx 144 template](https://github.com/dmitrystu/nuco-v/blob/master/nuco-v.pdf)
- [STM32F446RETx sample](https://github.com/r4hulrr/stm-32-bms)

# ST-LINK

Test on NUCLEO-F446ZE with [configuration](./figs/how-to-connect-external-stlink-to-nucleo-f446ze.png) from [post](https://community.st.com/stm32-mcus-products-25/debugging-stm32f446ze-nucleo-swd-with-external-st-link-v2-155755?utm_source=chatgpt.com).
```
CN4.2 --> SWCLK
CN4.4 --> SWDIO
CN6.3 --> GND
```
with these pins connected, external ST-LINK V2 can be connected, debugging, even SWD with ITM.

# USB OTG FS

[VBUS sensing](https://community.st.com/stm32-mcus-60/management-of-vbus-sensing-for-usb-device-design-93)
