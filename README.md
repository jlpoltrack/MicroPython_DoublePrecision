# MicroPython_DoublePrecision

Micropython builds with Double Precision support for ESP32 and Raspberry Pi Pico

# Build Notes

ESP32: 
* Built with 4.3.2 SDK
* Build guide: https://github.com/micropython/micropython/blob/master/ports/esp32/README.md
* Updates for Double Precision:
    * Change line in mpconfigport.h (Found in /ports/esp32/)
    * #define MICROPY_FLOAT_IMPL (MICROPY_FLOAT_IMPL_DOUBLE)
* Fix IRAM0 Error:
    * Add / change line in sdkconfig (Found in /ports/esp32/build*)
    * CONFIG_FREERTOS_PLACE_FUNCTIONS_INTO_FLASH=y

Pi Pico:
* Built with 1.3.0 SDK
* Build guide: https://community.element14.com/products/raspberry-pi/b/blog/posts/pi-pico-rp2040-micropython-double-precision




