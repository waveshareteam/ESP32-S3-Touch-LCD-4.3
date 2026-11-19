# Factory firmware

[简体中文](README_ZH.md)

| Date | Board variant | Firmware | Flash offset |
| --- | --- | --- | --- |
| 2026-09-02 | ESP32-S3-Touch-LCD-4.3 with capacitive touch | [ESP32-S3-Touch-LCD-4.3_FactoryOnly_20260902.bin](ESP32-S3-Touch-LCD-4.3_FactoryOnly_20260902.bin) | `0x0` |
| 2025-02-08 | ESP32-S3-LCD-4.3 without touch | [ESP32-S3-Touch-LCD-4.3_FactoryOnly_20250208.bin](ESP32-S3-Touch-LCD-4.3_FactoryOnly_20250208.bin) | `0x0` |

Choose the image that matches your board. For the touch variant, run:

```sh
esptool --chip esp32s3 write-flash 0x0 ESP32-S3-Touch-LCD-4.3_FactoryOnly_20260902.bin
```
