# sensorbox-v2
3D Printer Emission Sensor Array (Sensorbox v2) Code Remix

from https://www.printables.com/model/1436008-3d-printer-emission-sensor-array-sensorbox-v2-code

# Easy integration in ESPHome Builder (Home Assistant Addon):
```
substitutions:
  # Naming
  name: sensorbox-2
  friendly_name: Sensorbox V2
  # Display orientation options and color order, see https://esphome.io/components/display/ili9xxx/#configuration-variables
  display_mirror_x: false
  display_mirror_y: false
  display_swap_xy: true
  display_color_order: rgb

packages:
  remote_package:
    url: https://github.com/ablatz/sensorbox-v2
    ref: main
    files: [sensorbox-ha.yaml]
    refresh: 300s
```
