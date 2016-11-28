# mbed-js-repl-example

JavaScript REPL (Read-Eval-Print-Loop) for mbed OS 5.

<img src="img/repl.png" alt="Awesome stuff" width="440">

## Dependencies

Install:

* A recent version of [node.js](http://nodejs.org/).
* [Gulp](http://gulpjs.com/).
* [mbed CLI](https://github.com/ARMmbed/mbed-cli) and its dependencies.

### Patching mbed-js-gulp

In `mbed-js-gulp\tmpl\main.cpp.tmpl` change `Serial` into `RawSerial` and move it into global scope and to the top of the file.

## Build

1. Run `npm install`.
2. Run `gulp --target=YOUR_TARGET_NAME`.
    * To find your target name, look at the [platforms](http://developer.mbed.org/platforms/) page for your development board.
3. Copy the `mbedos5.hex` or `mbedos5.bin` file from `build/out/YOUR_TARGET_NAME` onto your development board.
4. Connect a serial monitor to your device (baud rate 115200).
5. Hack along!
