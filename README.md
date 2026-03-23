# UAI — AIO Tester Installer

Web-based firmware installer for the AIO Tester ESP32 device.

Open [the installer page](https://bebezinbtc-droid.github.io/UAI-installer/) in Chrome/Edge, connect your ESP32, and click Install.

## Updating firmware files

After building a new firmware version:

1. Copy these files from `build/` to `firmware/`:
   - `bootloader/bootloader.bin` → `firmware/bootloader.bin`
   - `partition_table/partition-table.bin` → `firmware/partition-table.bin`
   - `ota_data_initial.bin` → `firmware/ota_data_initial.bin`
   - `aio-tester-final.bin` → `firmware/firmware.bin`
   - `storage.bin` → `firmware/storage.bin`

2. Update version in `manifest.json`

3. Commit and push
