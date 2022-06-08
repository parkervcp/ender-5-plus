## set fan for hotend to fan1_pin
`define E0_AUTO_FAN_PIN FAN1_PIN`

## set z-steppers to 2
`define NUM_Z_STEPPER_DRIVERS 2   // (1-4) Z options change based on how many`

## disable bltouch delay
`#define BLTOUCH_DELAY 500`

## set auto-align for z-steppers
`define Z_STEPPER_AUTO_ALIGN`

## define z-stepper orientation
`define Z_STEPPERS_ORIENTATION 0`

## enable z-probe offset wizard
`define PROBE_OFFSET_WIZARD`

## disable marlin boot logo
`#define BOOT_MARLIN_LOGO_ANIMATED // Animated Marlin logo. Costs 3260 (or ~940) bytes of PROGMEM.`

## enable baby steppeing for setting z-offset
`define BABYSTEPPING`

## enable print pausing
`define ADVANCED_PAUSE_FEATURE`

## Set current limits for x,y,z and e steppers.
### Stock creality steppers are rated at 1600 mA 
```
define X_CURRENT       1000        // (mA) RMS current. Multiply by 1.414 for peak current.
define Y_CURRENT       1000
define Z_CURRENT       1000
define Z2_CURRENT      1000
define E0_CURRENT      1000
```  

## needed for print pausing
`define AUTO_REPORT_POSITION`

## enable for tft35 E3 V3.0
`define M115_GEOMETRY_REPORT`

## enable for tft35 E3 V3.0
`define M114_DETAIL         // Use 'M114` for details to check planner calculations`

## enable for tft35 E3 V3.0
`define REPORT_FAN_CHANGE   // Report the new fan speed when changed by M106 (and others)`

## enable for tft35 E3 V3.0
`define HOST_ACTION_COMMANDS`

## undefine  PROBING Margins
```
//#define PROBING_MARGIN_LEFT PROBING_MARGIN
//#define PROBING_MARGIN_RIGHT PROBING_MARGIN
//#define PROBING_MARGIN_FRONT PROBING_MARGIN
//#define PROBING_MARGIN_BACK PROBING_MARGIN
```