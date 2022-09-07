# Bike Rearview Radar
This embedded machine learning project focuses on visual object detection that can detect and differentiate between a car and a motorcycle. A camera is positioned under a bicycle saddle to see the rearview and can replace the need for a rearview mirror.
The image data is collected by taking pictures from a car using a smartphone camera pointing backwards, this allows to take images of the road/ environment, cars, and motorcycles.

By selecting 320x320 pixels, RGB parameter, Image and Object Detection learning blocks, the model can be expected to differentiate 2 output layers (car, motorcycle). The model should also be capable of obtaining the dimension of the Bounding Boxes, so based on the size and coordinate of the boxes, the distance and position of the car/ motorcycle can be estimated.

MobileNetV2 SSD FPN lite 320x320 is selected in the Edge Impulse Studio and deployed to a Raspberry Pi 4 which is mounted in the bicycle top tube. Additional python program is made to take the Edge Impulse model and show output on a LED matrix 8x8 (Sense HAT) on the Pi 4. The LED matrix will display different colors to differentiate between a car and a motorcycle and its distance and position.

[link to project](https://studio.edgeimpulse.com/studio/96989/)
