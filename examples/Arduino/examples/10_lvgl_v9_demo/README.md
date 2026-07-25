# LVGL v9.5.0 Adapter Example

This example demonstrates how to run `LVGL 9.5.0` on the
`Waveshare ESP32-S3-Touch-LCD-4.3` board with `ESP32_Display_Panel`
through a local Arduino-side adapter layer.

## Required Libraries

- `ESP32_Display_Panel`
- `LVGL v9.5.0`

The repository already provides `Arduino/libraries/LVGL_v9.5.0.zip`.

## Notes

- This example uses the supported board configuration file
- The current demo is `lv_demo_widgets()`
- The example now uses `esp_lv_adapter_*` style APIs on Arduino
- RGB path uses full-screen double frame buffers when available
