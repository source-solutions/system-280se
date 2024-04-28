# System 1
System Software for the Chloe 280SE.

The 280SE ROM firmware comprises:
* an API layer: SE/OS 1.0,
* a disk operating system: UnoDOS 3.1, and
* a shell: SE BASIC 4.2.

The 280SE can boot from ROM without requiring any disk files. However, copying the contents of the System disk to the root of your SD card provides additional functionality.

## Applications

System 1 includes ten simple appliactions with source code to demonstrate different technical aspects of the hardware and show you how to:

* **2019**: Scroll a bitmap image file vertically across the screen.
* **AAFALL**: Use color cycling to create animation effects.
* **ANIMSCR**: Animate a set of numbered frames without specifying the number of frames. 
* **BADAPPLE**: Stream video and audio using the DMA.
* **BOING**: Animate a set of frames and play it backwards when the last frame is reached.
* **JUGGLER**: Animate a set of frames and loop when the last frame is reached.
* **KAYAHARA**: Load data into shadow memory.
* **LASTV8**: Play music using the six channel programmable sound generator.
* **SCRSHOW**: Recursively read files from a folder and fade images in and out.
* **VDPTEST**: Read data directly from files.

## Fonts (code pages)

By default, the 280SE uses code page 437. System 1 enables you to override the default system font at boot by specifying a code page:

* **1250**: Latin 2 / Central European
* **1251**: Cyrillic
* **1252**: Latin 1 / Western European
* **1252**: Greek
* **1253**: Turkish

## Headers

System 1 provides a `SYSTEM.INC` file for use when building applications it includes all the SE/OS and UnoDOS system calls.

## Languages

System 1 enables you to change the language for the error messages on boot to:

* **French**
* **German**
* **Portuguese** (Brazilian)
* **Spanish**

## Online Help

System 1 provides an online help system that can be accesed by pressing the <kbd>Help</kbd> key from SE BASIC or by opening the `Help` app. It provides an overview of the 280SE and the SE BASIC language. 

## RUN BASIC application framework

System 1 provides a framework for converting a BASIC program into an application.
