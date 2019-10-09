# TD-pixelMappingLEDs-3D

LED mapping with arbitrary 3D Geometric arrangements.
Uses SOP Point Color attribute and Group SOP bounds to control colors.

This is a visualizer but also has the ability to send the rgb color data out to your led controller.

![screenshot](/img/viz.png)

The SOP geometry determines the addressing for your leds.

For example with this box arrangement shows the led pixel indices.

![screenshot](/img/addressing.png)

There's a CHOP named LED_Data. The first 3 samples correspond to the RGB of the first sop point/led index. The next 3 samples are for the second. point/led index , and so on.

![screenshot](/img/led_data.png)

This data can then go directly out to your led controller.

See here for a Depth Peel + GLSL method: https://github.com/wuestenarchitekten/collection/tree/master/LEDCubeRender

(actually that seems to be some method based on Depth Peeling, but ratherhave multiple cameras instead of multiple peels. The basis for a true Depth Peel method can be found here: [link](https://www.derivative.ca/forum/viewtopic.php?f=27&t=9938&fbclid=IwAR3o58_C2G5ODOD4FVqCMZW7Rm3OMWR8oPyU6OMMGhSWrNOKXv0jR3GiaL0#p37718))
