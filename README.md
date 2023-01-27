# parkers ender-5-plus setup

This is my heavily modified ender 5 plus setup. I am also storing models here for things that I have designed for the ender 5 first.

I have listed out all the parts and software changes I have made to the printer as well.

I am still working on moving the runout sensor to right above the hotend so I get more feed before running out, as I am trying to cut back on potential waste.


the current plan is to move to [Klipper](https://github.com/Klipper3d/klipper)

## Hardware
### Base Hardware
* Ender 5 Plus: https://www.creality3dofficial.com/products/creality-ender-5-plus-3d-printer
* Creality Large Enclosure: https://www.creality3dofficial.com/products/large-3d-printer-enclosure

### Replacement Parts
#### Control Hardware
* Mainboard: https://www.biqu.equipment/products/bigtreetech-skr-2
    * Better controllability and quieter operation.
* Touchscreen: https://www.biqu.equipment/products/btt-tft35-e3-v3-0-display-touch-screen-two-working-modes
    * Stock screen isn't compatible with the skr 2

#### Hotend Hardware
* [Custom X-Axis carriage]()
* Extruder/Hotend: https://e3d-online.com/products/revo-hemera
    * Better extruder with the revo hotend for easy nozzle swapping.

#### Bed Hardware
* Bed: https://preciseprinterparts.com/creality-ender-5-plus--cast-printer-bed.html
    * Flatter base
* Bed Levelling Standoffs: https://smile.amazon.com/gp/product/B07RZKF8MB
    * More solid standoff
* Heater: https://keenovo.store/collections/custom-keenovo-silicone-heaters/products/keenovo-silicone-heater-370mm-x-375mm-for-ender-5-plus-3d-printer-build-plate-heatbed-heating-upgrade
    * Better heater for the new bed
* Heater SSR: https://keenovo.store/collections/accessories/products/delixi-ssr-40a480vac-solid-state-relay-input-3v-32vdc-40da
    * Controls the heater
* Mag Base: https://www.th3dstudio.com/product/ezflex-magnetic-base/?attribute_size=376x370mm
    * Easier to swap out beds
* Smooth Plate: https://www.th3dstudio.com/product/ezflex2-flex-plate-smooth-or-textured-pei-coating/?attribute_plate-size=376x370mm&attribute_surface-type=Smooth+PEI
* Textured Plate: https://www.matterhackers.com/store/l/layerlock-powder-coated-pei-build-plate-steel-sheet/sk/M92RDWH7


#### Motion Hardware
* [Custom Y-Axis carriages]()
* Linear Rails: 3x450mm MGN12 Linear Rails https://smile.amazon.com/gp/product/B08JYC1XFK
* POM Z-axis Nuts: https://smile.amazon.com/gp/product/B08JQ65PTT
    * Quieter operation

#### Lighting
* LED channel: https://smile.amazon.com/gp/product/B078J143MN
* LEDs: https://smile.amazon.com/gp/product/B07KYP4Z3H

## Firmware
### Klipper
[kilpper configs](/klipper/)

## 3D Printed part models
### Hotend
* Hotend mount: In Progress
* BL/CR Touch mount: (models/hemera-bltouch-mount.stl)
* Cooling fan duct: https://rene-jurack.de/well-engineered-hemera-fan-duct-2/

### X-Carriage
* Linear rail adapter with Hemera Mount

### Y-Carriage
* Motor Side Linear Rail Adapter: In Progress
* Tensionor Side Linear Rail Adapter: In Progress

### Enclosure Lighting
Lighting for either the enclosure or printer
* Enclosure mounting clips: (models/creality-enclosure-lighting-mount.stl)
* 2020 Mounting Clips: In progress