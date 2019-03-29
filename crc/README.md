# CRC Library

 A module for calculating Cyclic Redundancy Check (CRC).

## Features

- Provides support for the following CRC algorithms:
  - CRC8
  - CRC8_SAE_J1850
  - CRC8_SAE_J1850_ZERO
  - CRC8_8H2F
  - CRC8_CDMA2000
  - CRC8_DARC
  - CRC8_DVB_S2
  - CRC8_EBU
  - CRC8_ICODE
  - CRC8_ITU
  - CRC8_MAXIM
  - CRC8_ROHC
  - CRC8_WCDMA
  - CRC16_CCITT_FALSE
  - CRC16_CCIT_ZERO
  - CRC16_ARC
  - CRC16_AUG_CCITT
  - CRC16_BUYPASS
  - CRC16_CDMA2000
  - CRC16_DDS_110
  - CRC16_DECT_R
  - CRC16_DECT_X
  - CRC16_DNP
  - CRC16_EN_13757
  - CRC16_GENIBUS
  - CRC16_MAXIM
  - CRC16_MCRF4XX
  - CRC16_RIELLO
  - CRC16_T10_DIF
  - CRC16_TELEDISK
  - CRC16_TMS37157
  - CRC16_USB
  - CRC16_A
  - CRC16_KERMIT
  - CRC16_MODBUS
  - CRC16_X_25
  - CRC16_XMODEM
  - CRC32
  - CRC32_BZIP2
  - CRC32_C
  - CRC32_D
  - CRC32_MPEG2
  - CRC32_POSIX
  - CRC32_Q
  - CRC32_JAMCRC
  - CRC32_XFER

# Installing

Just include the javascript file to your project.

```
<script type="text/javascript" src="kepat-crc-library.js"></script>
```

# Functions

## Methods

- [calculateCRC](#calculateCRC)

## calculateCRC

Calculate the CRC.

    CRC.calculateCRC(data, type, crcWidth, crcAlgorithm);

### Description

Function `calculateCRC ` calculates the CRC based on the paremeters passed.

### Parameters

- __data__: (string) The data to calculate CRC for.
- __type__: (string) The type of the data passed ( _string_ | _bytes_ ).
- __crcWidth__: (integer) The crc width to be used ( _8_ | _16_ | _32_ ).
- __crcAlgorithm__: (string) The data to calculate CRC for ([Algorithms](#Features)).

### Quick Example

    // Calculate the crc
    var calculatedValue = CRC.calculateCRC('value', 'string', 16, 'CRC16_CCITT_FALSE');

    // Display in the console log
    // Returns 0xCBCC
    console.log(calculatedValue);

## Thanks!

[CRC Calculator](http://www.sunshine2k.de/coding/javascript/crc/crc_js.html) which helped me to create this library and where some of the codes are based on.

# License
[MIT License](../LICENSE)
