# UServoClass

Arduino/Teensy servomotor class without `delay()`. Created to drive MKS DS95i micro-servomotors throughout the development of Azure Talos, a multi-string mechatronic chordophone.

## Installation

1. Copy the header and source files to your Arduino/Teensyduino project folder.
2. Add the `#include "UServo.h"` directive at the top of your main file.

## Using the class

* Declare a servomotor instance:

`UServo servo(34)`

* Initialize the servomotor pin in `setup()`:

`servo.init()`

* Call the move function with the pulse interval to set the servomotor position (behavior might vary between different servomotor models):

`servo.move(300)`


## Example:

Please refer to the "Clamper.ino" file for an example (for Teensy boards).