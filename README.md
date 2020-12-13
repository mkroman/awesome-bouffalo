# Awesome bouffalo

This project aims to be a primary source of awesome resources related to
the development of Bouffalo Lab's RISC-V chips.

## Contents

* [HAL implementations](#hal-implementations)
* [ROM tools](#rom-tools)
* [Board details](#board-details)

### HAL implementations

#### Rust
* [sipeed/bl602-hal](https://github.com/sipeed/bl602-hal)

#### Arduino
* [pine64/ArduinoCore-bouffalo](https://github.com/pine64/ArduinoCore-bouffalo)

### ROM tools

#### Feature matrix

| Project                           | Flash                                    | RAM                                      |
|-----------------------------------|------------------------------------------|------------------------------------------|
| [renzenicolai/bl602tool]          | ✓ Read / ✓ Write / ~~✗ Execute~~         | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |
| [stschake/bl60x-flash]            | ~~✗ Read~~ / ✓ Write[^1] / ~~✗ Execute~~ | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |
| [spacemeowx2/blflash]             | ✓ Read / ✓ Write / ~~✗ Execute~~         | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |
| [mkroman/bouffalo-cli]            | ✓ Read / ~~✗ Write~~/ ~~✗ Execute~~      | ~~✗ Read~~ / ~~✗ Write~~ / ~~✗ Execute~~ |

[^1]: Only writes starting from the offset `0x10000`

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

* [lupyens peek of pinecone](https://lupyuen.github.io/articles/pinecone)
* [Connect PineCone BL602 to OpenOCD](https://lupyuen.github.io/articles/openocd)
* [Debug Rust on PineCone BL602 with VSCode and GDB](https://lupyuen.github.io/articles/debug)
