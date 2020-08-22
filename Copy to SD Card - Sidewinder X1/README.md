## Sidewinder X1 TFT Update Instructions

### Configuration Update (this can be done without updating the firmware, images, or fonts)
1. Copy the `config.ini` file to the root of the SD card.
2. Put the SD card into the Sidewinder X1's TFT SD card slot and turn on the printer.

### Firmware Update (only required if the code changed)
1. Build the `MKS_32_V1_4 config` using Platform IO.
2. Copy `.pio/build/MKS_32_V1_4/MKS_32_VX.X.X.x.bin` file to `Copy to SD Card - Sidewinder X1` folder.
3. Rename the `MKS_32_VX.X.X.x.bin` file to `mkstft28.bin`
4. Copy the `mkstft28.bin` file to the root of the SD card.
5. Put the SD card into the Sidewinder X1's TFT SD card slot and turn on the printer.

### Image(s) Update (only required if changed)
1. Update the files in the `Copy to SD Card - Sidewinder X1/bmp` folder with the latest files from the `Copy to SD Card root directory to update - Unified Menu Material theme/TFT28/bmp` folder, leaving the customized Sidewinder `Logo.bmp` file in place.
2. Create a folder called `MKS` in the root of the SD card.
3. Copy the `Copy to SD Card - Sidewinder X1/MKS/bmp` folder to the `MKS` folder on the SD card.
4. Put the SD card into the Sidewinder X1's TFT SD card slot and turn on the printer.

NOTE: While it's possible to copy only the changed files to the SD card, it will update much slower as it will check for the existence of each image. It's best to copy the whole `bmp` folder and it will automatically skip any images that haven't changed.

### Font(s) Update (only required if changed)
1. Update the files in the `Copy to SD Card - Sidewinder X1/font` folder with the latest files from the `Copy to SD Card root directory to update - Unified Menu Material theme/TFT28/font` folder
2. Create a folder called `MKS` in the root of the SD card.
3. Copy the `Copy to SD Card - Sidewinder X1/font folder to the `MKS` folder on the SD card.
4. Put the SD card into the Sidewinder X1's TFT SD card slot and turn on the printer.

### Update Everything
1. Copy all files from the `Copy to SD Card - Sidewinder X1` folder to the root of the SD card.
2. Put the SD card into the Sidewinder X1's TFT SD card slot and turn on the printer.

-------

Any combination of the above can be done at once, including any subset of the images and fonts. Once the firmware, images, and fonts have been updated, changing the configuration can be done using only the `config.ini` file without needing to reflash everything else.