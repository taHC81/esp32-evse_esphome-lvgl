# esp32-evse_esphome-lvgl
HMI for ESP32-EVSE based on ESPHome and LVGL

This is a replacement Human-Machine Interface for the Nextion screen for the excellent [ESP32-EVSE project by Miroslav Dzúrik](https://github.com/dzurikmiroslav/esp32-evse).
It is a plug and play replacement, as it relies on the original Nextion protocol implemented by the author. _Note:_ It doesn't implement the entire Nextion protocol, just the subset required by the EVSE.

The device consists of any graphical display with touch screen supported by [ESPHome](https://esphome.io/components/#display-hardware-platforms).

![Screen](images/esp32-evse_esphome-lvgl_charging.png) ![Screen](images/esp32-evse_esphome-lvgl_session.png)
![Screen](images/esp32-evse_esphome-lvgl_settings.png) ![Screen](images/esp32-evse_esphome-lvgl_info-status.png)
![Screen](images/esp32-evse_esphome-lvgl_info-about.png) ![Screen](images/esp32-evse_esphome-lvgl_info-display.png)

The example file _esp32-evse_esphome-lvgl_display.yaml_ contains working configuration for the Guition JC3248w535 display, which can be connected directly to ESP32-EVSE board, from the 4-pin JST 1.24 connector located near to the USB-C socket. The pins are 5V, TX and RX at 3.3v and GND.
