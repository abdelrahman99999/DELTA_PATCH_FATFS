# DELTA_PATCH_FATFS
Delta Patching binary files using JojoDiff Algorithm with the help of FatFS For STM32 Target <br>
<br>The project will be used next, to implement DELTA OTA Update

## How to generate Patch File
To generate patch files you'll need to build [JojoDiff](http://jojodiff.sourceforge.net) or [JDiff.js](https://github.com/janjongboom/jdiff-js).

1. Install a recent version of [Node.js](https://nodejs.org).
1. Install JDiff.js:

    ```
    $ npm install jdiff-js -g
    ```

1. Generate a patch file via:

    ```
    $ jdiff old-file.bin new-file.bin old-to-new-file.patch
    ```

## Hardware Used
- STM32F439 Nucleo-144
- Micro SD Card Adapter Module
- Micro SDHC 8 GB

## Prerequisites
- Make Sure SD Card Module should get 5V. Try separate power supply if possible
- Format SD card with FAT32, 4096 bytes for allocation unit size.

## Reference
Thanks to [janpatch](https://github.com/janjongboom/janpatch)
