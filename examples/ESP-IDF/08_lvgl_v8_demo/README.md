| Supported Targets | ESP32-S3 |
| ----------------- | -------- |

# LVGL v8 Porting Example

This example now uses the local `ESP32_Display_Panel` adapter component instead of the old
project-local RGB LCD and LVGL port implementation. It targets the supported board
`Waveshare ESP32-S3-Touch-LCD-4.3` and runs the LVGL v8 demo on top of the board adapter.

## Features

- Uses local `Arduino/libraries/ESP32_Display_Panel` through `idf_component.yml`
- Uses supported board config `CONFIG_BOARD_WAVESHARE_ESP32_S3_TOUCH_LCD_4_3`
- Keeps LVGL v8 anti-tearing mode support through `lvgl_v8_port`

## Build

1. Open the example directory:

   ```bash
   cd ESP-IDF/08_lvgl_Porting
   ```

2. Configure the target:

   ```bash
   idf.py set-target esp32s3
   ```

3. Build, flash and monitor:

   ```bash
   idf.py -p PORT build flash monitor
   ```

## Notes

- Board selection is already enabled in `sdkconfig.defaults`
- LVGL anti-tearing mode and rotation options are under `Example Configuration`
- The example currently starts `lv_demo_widgets()`
