# charging-sdl-dtg

Charging screen for the initramfs. Fork with Deb-to-go compatibility

![photo](https://wiki.postmarketos.org/images/d/d8/Charging-sdl.jpg)



## TODOs

- [x] display whether or not the device is charging
- [ ] add option to boot rest of system from it using built-in buttons
- [ ] backlight control
- [ ] display charging type
- [ ] display battery temperature

## build

1. `cd charging-sdl`
2. `make` or if you want fancy features `make LIBBATTERY=true`

## run

- without text `./charging_sdl -t`
- with text `./charging_sdl -tpcf path/to/font`

## usage

- `-t` test mode, keep the application open until explicitly closed and is not in full screen
- `-p` display the percent charged the battery is
- `-c` display current when charging (if available - see build section)
- `-o` display a square, and move it randomly around the screen to prevent burn-in on OLED screens
- `-f` font used to display all text
