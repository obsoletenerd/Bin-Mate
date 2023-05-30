# Bin Mate

Bin Mate is a multi-MCU (ESP32, RPi Pico, more soon) bin reminder tool. Initially for Ballarat in Victoria AU but hopefully rolling out to more cities soon. It is an open source software/hardware project connecting to local council APIs to remind you which bins to put out on which days.

The project can be as simple as buying an RPi Pico + a click-on e-Paper hat (see "/RPi Pico" folder), up to a fully-custom PCB you can self-solder (see "/ESP32 PCB" folder) or buy as a kit (Soon™) that runs for months on a coin cell battery and sticks to your fridge with a magnet.

## Raspberry Pi Pico W + Waveshare Pico e-Paper 2.13in Hat

This is the easiest way to get started with this project, using just an [RPi Pico W](https://www.raspberrypi.com/documentation/microcontrollers/raspberry-pi-pico.html) (WiFi model) and a [Waveshare Pico e-Paper 2.13in Hat](https://www.waveshare.com/pico-epaper-2.13.htm). Install MicroPython onto the RPi Pico using Thonny (or your tool of choice), then edit your address and wifi details into the code, then copy the code onto the Pico. Plug it into any USB plug for power (or if you're RPi-savvy, wire up some batteries) and you're running.

We have also designed a few different 3D printable cases or a laser-cut wooden case to pretty the project up, both of which take a magnet on the back to stick to your fridge or use double-sided tape to put it up wherever you want.


## ESP32 + 2.9" e-Paper Module

For a version of the project that can run off a coin-cell battery for many months, we're developing a custom PCB with an ESP32 onboard utilising all the deep sleep trickery, along with a cheap 2.9" e-Paper module, to create a device that can stick to your fridge/etc and requires no wiring, soldering, or coding. It will throw up its own Wifi AP with a dashboard for configuration and customisation. PCB designs and code will all be open-sourced and added here soon.

## Notes

## #Creating New Graphics

- Images should be 250px wide by 128px high
- Use [this website](https://javl.github.io/image2cpp/) to convert the images, and the below settings:
    - Section 1. Select your image(s)
    - Section 2. All settings in this section stay as default other than "Rotate Image 90 degrees"
    - Section 4. Code output format to "Raw Bytes", Draw Mode to "Horizontal - 1 bit per pixel"
    - Click "Generate Code"
    - Paste into the appropriate area in the project code