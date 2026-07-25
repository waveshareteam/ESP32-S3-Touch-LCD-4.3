| Supported Targets | ESP32-S3 |
| ----------------- | -------- |

# LVGL v9.5.0 Porting Example

This example demonstrates how to run `LVGL 9.5.0` on `Waveshare ESP32-S3-Touch-LCD-4.3`
through the local `ESP32_Display_Panel` adapter component.

## Features

- Uses local `Arduino/libraries/ESP32_Display_Panel`
- Uses supported board config `BOARD_WAVESHARE_ESP32_S3_TOUCH_LCD_4_3`
- Uses a simple LVGL v9 partial-buffer port

## Build

1. Open the example directory:

   ```bash
   cd ESP-IDF/09_lvgl_v9.5.0_Porting
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

- This example is intentionally simple and uses partial rendering for LVGL v9
- The example currently starts `lv_demo_widgets()`
