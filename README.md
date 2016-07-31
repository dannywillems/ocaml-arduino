# ocaml-arduino

Arduino information to run OCaml on Arduino. This repository aims to list details to compile OCaml project to run them on Arduino.

Arduino uses [microcontrollers](https://en.wikipedia.org/wiki/Microcontroller) produced by [Atmel](https://en.wikipedia.org/wiki/Atmel), a company producing semiconductors. Arduino uses [Atmel AVR microcontrollers](https://en.wikipedia.org/wiki/Atmel_AVR). For example, the Arduino Uno use the ATmega328P. **For the moment, we can't compile OCaml for this microcontrollers family.**

To write binaries running on Atmel AVR microcontrollers, you can use [avr-libc](http://www.nongnu.org/avr-libc/) which is a subset of the standard C library and tools to compile in assembler readable for Atmel AVR. See [this page](http://www.nongnu.org/avr-libc/user-manual/overview.html) for an overview of the toolchain. If you are on Debian or you use apt-get, you can install avr-libc and toolchain tools with
```
sudo apt-get install avr-libc
```
It will install avr-libc, binutils-avr (containing all tools) and gcc-arv (to compile C in AVR instructions).
