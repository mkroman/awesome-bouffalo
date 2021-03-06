# Awesome bouffalo

This project aims to be a primary source of awesome resources related to
the development of Bouffalo Lab's RISC-V chips.

## Contents

* [HAL implementations](#hal-implementations)
* [ROM tools](#rom-tools)
* [Board details](#board-details)
* [Software details](#software-details)

### HAL implementations

#### Rust
* [sipeed/bl602-hal](https://github.com/sipeed/bl602-hal)

#### Arduino
* [pine64/ArduinoCore-bouffalo](https://github.com/pine64/ArduinoCore-bouffalo)

### ROM tools

#### Feature matrix

| Project                           | Flash                                                   | RAM                                      |
|-----------------------------------|---------------------------------------------------------|------------------------------------------|
| [renzenicolai/bl602tool]          | ✓ Read / ✓ Write / ~~✗ Execute~~                        | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |
| [stschake/bl60x-flash]            | ~~✗ Read~~ / ✓ Write<sup>[1](#f1)</sup> / ~~✗ Execute~~ | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |
| [spacemeowx2/blflash]             | ✓ Read / ✓ Write / ~~✗ Execute~~                        | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |
| [mkroman/bouffalo-cli]            | ✓ Read / ~~✗ Write~~ / ~~✗ Execute~~                    | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |

<a name="f1" href="#f1"><sup>1</sup></a>: Only writes starting from the offset `0x10000`

#### Python
* [bl602tool by r3nz3][renzenicolai/bl602tool]
* [bl60x-flash by stschake][stschake/bl60x-flash]

[renzenicolai/bl602tool]: https://github.com/renzenicolai/bl602tool
[stschake/bl60x-flash]: https://github.com/stschake/bl60x-flash

#### Rust
* [blflash by spacemeowx2][spacemeowx2/blflash]
* [bouffalo-cli by mkroman][mkroman/bouffalo-cli]

[spacemeowx2/blflash]: https://github.com/spacemeowx2/blflash
[mkroman/bouffalo-cli]: https://github.com/mkroman/bouffalo-cli

### Board details

* [Lupyuen's Quick Peek at the PineCone](https://lupyuen.github.io/articles/pinecone)
* [Connect PineCone BL602 to OpenOCD](https://lupyuen.github.io/articles/openocd)
* [Debug Rust on PineCone BL602 with VSCode and GDB](https://lupyuen.github.io/articles/debug)
* [Flashing Firmware to PineCone BL602](https://lupyuen.github.io/articles/flash)
* [Control PineCone BL602 RGB LED with GPIO and PWM](https://lupyuen.github.io/articles/led)
* [PineCone BL602 talks to I2C Sensors](https://lupyuen.github.io/articles/i2c)
* [PineCone BL602 talks SPI too!](https://lupyuen.github.io/articles/spi)
* [PineCone BL602 Blasting Pixels to ST7789 Display with LVGL Library](https://lupyuen.github.io/articles/display)
* [PineCone BL602 Talks UART to Grove E-Ink Display](https://lupyuen.github.io/articles/uart)
* [The RISC-V BL602 Book](https://lupyuen.github.io/articles/book)
* [Connect PineCone BL602 to LoRa Transceiver](https://lupyuen.github.io/articles/lora)

### Software details
* [Porting Mynewt to PineCone BL602](https://lupyuen.github.io/articles/mynewt)
* [Mynewt GPIO ported to PineCone BL602 RISC-V Board](https://lupyuen.github.io/articles/gpio)
* [BL602 SVD description](https://github.com/pine64/bl602-svd)
