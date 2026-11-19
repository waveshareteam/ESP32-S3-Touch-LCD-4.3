# 出厂固件

[English](README.md)

| 日期 | 适用硬件 | 固件 | 烧录偏移 |
| --- | --- | --- | --- |
| 2026-09-02 | ESP32-S3-Touch-LCD-4.3，带电容触摸 | [ESP32-S3-Touch-LCD-4.3_FactoryOnly_20260902.bin](ESP32-S3-Touch-LCD-4.3_FactoryOnly_20260902.bin) | `0x0` |
| 2025-02-08 | ESP32-S3-LCD-4.3，不带触摸 | [ESP32-S3-Touch-LCD-4.3_FactoryOnly_20250208.bin](ESP32-S3-Touch-LCD-4.3_FactoryOnly_20250208.bin) | `0x0` |

请按实际硬件选择对应的固件。带触摸版的烧录命令如下。

```sh
esptool --chip esp32s3 write-flash 0x0 ESP32-S3-Touch-LCD-4.3_FactoryOnly_20260902.bin
```
