# Bit GadgetKit

This Microsoft MakeCode package is used as an **Bit GadgetKit extension** for micro:bit.

## Basic Usage

Here are some related tutorials to help you get started with BitGadget Kit.

### 1. The LED Controller
### 1.1 Implementation
We'll make a LED controller that shows different light displays by rotating the rotary angle sensor.
<p align = "left">
    <img src="https://docproxy.chmakered.com/Public/Uploads/2019-11-05/5dc0eb0ec788d.png" alt="">
</p>

### 1.2 Write a Program
Let's go to MakeCode: https://makecode.microbit.org
Create a new project. Firstly add a "forever" block and connect the block "plot bar graph of up to" into it. Then add a "analog read pin" block. Set the maximum as 1023, which is the greatest value that the rotary angle sensor can produce. Finally, connect a "pause" block and set the time delay as 1,000 millisecond.
<p align = "left">
    <img src="https://docproxy.tinkergen.com/server/../Public/Uploads/2020-03-16/5e6f524c028a9.png" alt="">
</p>

### 1.3 Connect a Device
Modules: micro:bit, BitMaker, rotary angle sensor
Straightly slide the micro:bit into BitMaker and be careful not to reverse it. Connect the rotary angle sensor to the port labeled as P2 on the BitMaker. Then connect the micro:bit to your PC with a USB cable. Check if the LED indicator on the micro:bit lights up. If not, you need to unplug in the USB cable and connect it to the devices again.

### 1.4 Download a Program
You have been introduced how to download a program in the previous tutorials, which can be simply concluded into steps as: rename a program, click the "Download" button and send it to the micro:bit.

### 1.5 Run a Program
Turn on the switch on the BitMaker and see if the micro:bit can work normally.

### 2. Fun with LED Strip
### 2.1 Implementation
Let's take the challenge to another level. In this project, we'll make the RGB LED strip blink red when the micro:bit tilts left, and blink yellow when it tilts right.
<p align = "left">
<img src="https://docproxy.chmakered.com/server/../Public/Uploads/2020-03-05/5e60c05e943b5.png" alt="">
</p>

### 2.2 Write a Program
<p>Note that in MakeCode we don't have blocks that control the Grove modules and BitMaker. Therefore we need to add a MakeCode extension for the BitGadget Kit to make sure that everything goes on well. Let's learn how to do it now!</p>
<p>[How to Add the Extension of BitGadget Kit] Go to MakeCode: https://makecode.microbit.org</p>
<p>Step 1  Click the gear icon (for settings) on the blue bar in MakeCode.
<img src="https://docproxy.tinkergen.com/server/../Public/Uploads/2020-03-16/5e6f53376d166.png" alt=""></p>
<p>Step 2  Select "Extensions" from the drop-down list which takes you to the extensions page.
<img src="https://docproxy.tinkergen.com/server/../Public/Uploads/2020-03-16/5e6f5345efa5c.png" alt=""></p>
<p>Step 3 Input the key word of the BitGadget Kit extension into the search box: Bit GadgetKit or bit-gadgetkit
</p>
<blockquote>
<p>If a prompt says that this extension does not exist, please close the browser and try again.</p>
</blockquote>
<p>Step 4 Click the extension package which takes you back to the homepage. You will see that the BitGadget Kit extension is then successfully added.<br><img src="https://docproxy.tinkergen.com/server/../Public/Uploads/2020-03-16/5e6f539853369.png" alt=""></p>
<p>Firstly, we need to add the Neopixel extension. Let's create a new project to go to the workspace. Click "Extensions" from "Advanced" and select "Neopixel" from the pop-up page.<br>Next, add an "on start" block. Confirm the LEDs quantity and set the color format.<br>Then, find out the block "on shake" from the tab "Input" and select "tilt left". Connect a "repeat 4 times" block from the "Loops" tab into the block "on tilt left". These two blocks together make the micro:bit repeat a designated action 4 times when it tilts left. Similarly, if you select "tilt right", the micro:bit will execute the same action when it tilts right.<br>Select the block "strip show color red" from "neopixel" and connect it into the two blocks above, and still keep the color as red. Connect the blocks "strip show" and "pause (ms) 500" underneath. Then, add the blocks "strip clear", "strip show" and "pause (ms) 500" by turns. The strip will blink when this program starts running. Similarly, when you select "tilt right", you just need to select a yellow color and repeat the steps above. </p>

<p><img src="https://docproxy.tinkergen.com/server/../Public/Uploads/2020-03-16/5e6f551c0e866.png" alt=""></p>

### 2.3 Connect a Device
Straightly slide the micro:bit into BitMaker and be careful not to reverse it. Connect the LED strip to the port labeled as P1 on the BitMaker. Then connect the micro:bit to your PC with a USB cable. Check if the LED indicator on the micro:bit lights up. If not, you need to unplug in the USB cable and connect it to the devices again.

### 2.4 Download a Program
You have been introduced how to download a program in the previous tutorials, which can be simply concluded into steps as: rename a program, click the "Download" button and send it to the micro:bit.

### 2.5 Run a Program
Turn on the switch on the BitMaker and see if the micro:bit can work normally.

## Reference

please visit https://docproxy.chmakered.com/web/#/2?page_id=325

## License
MIT


## Supported targets

* for PXT/microbit

