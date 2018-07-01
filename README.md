# TD-pixelMappingLEDs-3D

LED mapping with arbitrary 3D Geometric arrangements.
Uses SOP Point Color attribute and Group SOP bounds to control colors.

This is a visualizer but also has the ability to send the rgb color data out to your led controller.

![screenshot](/img.png)

The SOP geometry determines the addressing for your leds.

For example with this box arrangement shows the led pixel indices.

![screenshot](/addressing.png)

There's a DAT named LEDRGBData. This has all the rgb data in three columns: Cd(0),Cd(1),Cd(2), which correspond to R,G,B. So the first row corresponds to the RGB data of the led address of 0. The second row is the RGB data for the address 1, and so on.

![screenshot](/ledRGBData.png)

This DAT data can then go directly out to your led controller.
