# parkers ender-5-plus setup

This is my heavily modified ender 5 plus setup. I am also storing models here for things that I have designed for the ender 5 first.

I have listed out all the parts and software changes I have made to the printer as well.

I am still working on moving the runout sensor to right above the hotend so I get more feed before running out, as I am trying to cut back on potential waste.

## Firmware
### Klipper
[kilpper configs](/klipper/)

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
    * [3d printed mount by jingerale79](https://www.thingiverse.com/thing:4507896)

#### Hotend Hardware
* Extruder/Hotend: https://e3d-online.com/products/revo-hemera
    * Better extruder with the revo hotend for easy nozzle swapping.
* Custom X-Axis carriage
    * [using bltouch](models/x-axis/hemera-linear-mount.stl)
    * using nozzle as probe
        * [linear mount](models/x-axis/hemera-linear-mount-nozzle-probe.stl)
        * [hemera mount](models/x-axis/hemera-mount-nozzle-probe.stl)
* Part Cooling
    * Rene Jurack's hemera cooler seen here - https://rene-jurack.de/well-engineered-hemera-fan-duct-2/
        * the 4010 version needs to special mounts.
        * ebmpapst 5015 blower with bltouch [mount](models/fan-mounts/hemera-bl-touch-5015-mount.stl)
        * ebmpapst 5015 blower for nozzle probe [mount](models/fan-mounts/hemera-5015-mount.stl)

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
* Linear Rails: 3x450mm MGN12 Linear Rails https://smile.amazon.com/gp/product/B08JYC1XFK
* POM Z-axis Nuts: https://smile.amazon.com/gp/product/B08JQ65PTT
    * Quieter operation
* Drag chain - 10X20mm [Amazon Link](https://www.amazon.com/gp/product/B07SFFT1K5)
    * [drag chain mounts](models/y-axis/dragchain/)
* Custom Y-Axis carriages  
    I have gotten these cut out of aluminum to handle the heat for the chamber and stepper motor.
    * [stepper side](models/y-axis/y-axis-linear-carriage-stepper-side.stl)
        There is an issue with the stepper potentially getting hot and warping the carriage
    * [pulley side](models/y-axis/y-axis-linear-carriage-pully-side.stl)

#### Lighting
* LED channel: https://smile.amazon.com/gp/product/B078J143MN
* LEDs: https://smile.amazon.com/gp/product/B07KYP4Z3H


## 3D Printed part models
### Hotend
* BL/CR Touch mount: [bltouch mount](models/hemera-bltouch-mount.stl)
* Cooling fan duct: https://rene-jurack.de/well-engineered-hemera-fan-duct-2/
    * ebmpapst 5015 blower with bltouch [mount](models/fan-mounts/hemera-bl-touch-5015-mount.stl)
    * ebmpapst 5015 blower for nozzle probe [mount](models/fan-mounts/hemera-5015-mount.stl)

### X-Carriage
I have moved the filament runout sensor to the extruder end as well. Still working on how to handle the boden
* [linear rail mount](models/x-axis/hemera-linear-mount.stl)
* Nozzle as proble
    * [linear mount](models/x-axis/hemera-linear-mount-nozzle-probe.stl)
    * [hemera mount](models/x-axis/hemera-mount-nozzle-probe.stl)

### Y-Carriages  
I have gotten these cut out of aluminum to handle the heat for the chamber and stepper motor.
* [Stepper Side Linear Rail Adapter](models/y-axis/y-axis-linear-carriage-stepper-side.stl)
* [Tensionor Side Linear Rail Adapter](models/y-axis/y-axis-linear-carriage-pully-side.stl)

### Enclosure Lighting
Lighting for either the enclosure or printer
* [Enclosure mounting clips](models/creality-enclosure-lighting-mount.stl)
* [2020 Mounting Clips]() - In progress