# stlink3-flash

Piggyback board that adds 16 mbyte flash memory to STLINK V3 MINI, for storing micropython scripts. PCB at [Oshpark](https://oshpark.com/shared_projects/O2kwQZOg).

BOM:

| Comp. | Desc          |
| ----- | ------------- |
| U1    | W25Q128JVSSIQ |
| C1    | 100n 0603     |
| R1    | 4k7 0603      |

Access through STM32F723, SPI4:

| Pin | Desc.     |
| --- | --------- |
| PE6 | SPI4_MOSI |
| PE5 | SPI4_MISO |
| PE4 | !FLASH_CS |
| PE2 | SPI4_SCK  |
