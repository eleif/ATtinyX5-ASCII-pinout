# ATtinyx5 ASCII pinout
Microchip (ex Atmel) AVR 8 bit microcontroller ASCII pinout for 8 pin packages (PDIP, SOIC)

## Product pages
- https://www.microchip.com/wwwproducts/en/ATtiny25
- https://www.microchip.com/wwwproducts/en/ATtiny45
- https://www.microchip.com/wwwproducts/en/ATtiny85

## PDFs
- ATtiny25/45/85 - Complete Datasheet: https://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-2586-AVR-8-bit-Microcontroller-ATtiny25-ATtiny45-ATtiny85_Datasheet.pdf (4 MB)
- AVR Instruction Set Manual: https://ww1.microchip.com/downloads/en/DeviceDoc/AVR-InstructionSet-Manual-DS40002198.pdf (1 MB)

## by bit
    // PB0 5 MOSI/DI/SDA/AIN0/OC0A/#OC1A/AREF/PCINT0
    // PB1 6 MISO/DO/AIN1/OC0B/OC1A/PCINT1
    // PB2 7 SCK/USCK/SCL/ADC1/T0/INT0/PCINT2
    // PB3 2 PCINT3/XTAL1/CLKI/#OC1B/ADC3
    // PB4 3 PCINT4/XTAL2/CLKO/OC1B/ADC2
    // PB5 1 PCINT5/#RESET/ADC0/dW

## by pin
    // PB5 1 PCINT5/#RESET/ADC0/dW
    // PB3 2 PCINT3/XTAL1/CLKI/#OC1B/ADC3
    // PB4 3 PCINT4/XTAL2/CLKO/OC1B/ADC2
    // GND 4
    // PB0 5 MOSI/DI/SDA/AIN0/OC0A/#OC1A/AREF/PCINT0
    // PB1 6 MISO/DO/AIN1/OC0B/OC1A/PCINT1
    // PB2 7 SCK/USCK/SCL/ADC1/T0/INT0/PCINT2
    // VCC 8

## by package
    //                                    +---u---+
    // PCINT5/#RESET/ADC0/dW PB5        1 |       | 8 VCC
    // PCINT3/XTAL1/CLKI/#OC1B/ADC3 PB3 2 |       | 7 PB2 SCK/USCK/SCL/ADC1/T0/INT0/PCINT2
    // PCINT4/XTAL2/CLKO/OC1B/ADC2 PB4  3 |       | 6 PB1 MISO/DO/AIN1/OC0B/OC1A/PCINT1
    // GND                              4 |       | 5 PB0 MOSI/DI/SDA/AIN0/OC0A/#OC1A/AREF/PCINT0
    //                                    +-------+

    //                                               +-------+
    // MOSI/DI/SDA/AIN0/OC0A/#OC1A/AREF/PCINT0 PB0 5 |       | 4 GND
    // MISO/DO/AIN1/OC0B/OC1A/PCINT1           PB1 6 |       | 3 PB4  PCINT4/XTAL2/CLKO/OC1B/ADC2
    // SCK/USCK/SCL/ADC1/T0/INT0/PCINT2        PB2 7 |       | 2 PB3  PCINT3/XTAL1/CLKI/#OC1B/ADC3
    //                                         VCC 8 |       | 1 PB5  PCINT5/#RESET/ADC0/dW
    //                                               +---n---+


