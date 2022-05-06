## set baud rate for tft35 E3 V3
`define BAUDRATE_2 115200   // Enable to override BAUDRATE`

## Set drive type for all drivers
```
define X_DRIVER_TYPE  TMC2209
define Y_DRIVER_TYPE  TMC2209
define Z_DRIVER_TYPE  TMC2209
define Z2_DRIVER_TYPE TMC2209
define E0_DRIVER_TYPE TMC2209
```

## Set Z (800) and e (138) steps
`define DEFAULT_AXIS_STEPS_PER_UNIT   { 80, 80, 800, 138 }`

## Disable endstop pin and use BLTouch
```
#define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN
define USE_PROBE_FOR_Z_HOMING
```

## enabe BLTouch
`define BLTOUCH`

## Set nozzle probe X,Y offset 
`define NOZZLE_TO_PROBE_OFFSET { 44.5, -7, 0 }`

## double check z height.
`define MULTIPLE_PROBING 2`

## enable for accuracy
`define Z_MIN_PROBE_REPEATABILITY_TEST`

## fix directions for axis and extruder
```
define INVERT_Y_DIR false
define INVERT_Z_DIR true
define INVERT_E0_DIR true
```

## Set build volume
```
define X_BED_SIZE 350
define Y_BED_SIZE 350
define Z_MAX_POS 400
```

## Enable Runout Sensor
`define FILAMENT_RUNOUT_SENSOR`

## set bed leveling style to bilinear
`define AUTO_BED_LEVELING_BILINEAR`

## re-enable bel levelling after an auto-home
`define RESTORE_LEVELING_AFTER_G28`

## enble G26
`define G26_MESH_VALIDATION`

## set grid points to 3 for a 3x3 grid
`define GRID_MAX_POINTS_X 5`

## estimate bed beyond
```
define EXTRAPOLATE_BEYOND_GRID
define ABL_BILINEAR_SUBDIVISION
```

## enable leveling menu
`define LCD_BED_LEVELING`

## set level corners
`define LEVEL_BED_CORNERS`

## change level corners
`define LEVEL_CORNERS_INSET_LFRB { 50, 50, 50, 50 } // (mm) Left, Front, Right, Back insets`

## Enable safe z homing
`define Z_SAFE_HOMING`

## set z-home to the center of the bed
```
define Z_SAFE_HOMING_X_POINT ((X_BED_SIZE) / 2 )  // X point for Z homing
define Z_SAFE_HOMING_Y_POINT ((Y_BED_SIZE) / 2 )  // Y point for Z homing
```

## This is not applied at the moment
## calibrating skew with the following
## https://vector3d.co.uk/store/Vector-3D-Printer-Calibration-and-Test-Suite-p429602854

## add nozzle park feature
`define NOZZLE_PARK_FEATURE`

## enable for tft35 e3 v3.0
`define REPRAP_DISCOUNT_FULL_GRAPHIC_SMART_CONTROLLER`

## Enable for RGB LED

`#define BLINKM`

`#define NEOPIXEL_LED`

`#define NEOPIXEL_PIXELS 56`

`#define NEOPIXEL_STARTUP_TEST`