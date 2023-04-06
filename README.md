# Rock Pi 5 image
![output image]( https://qengineering.eu/github/SDcard32GB_RockPi5_Large.webp)<br/>
## A Rock Pi 5 image with OpenCV, ncnn, TNN and NPU
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>

------------

## Installation.

- Get a 32 GB (minimal) SD-card which will hold the image. 
- Download the `RockPi5.img.xz` image (2.8 GByte) from our [Sync](https://ln5.sync.com/dl/b9c189080/csvcycve-qn6f2zt8-49z54nm6-m9gvzbf3) site. 
- Flash the image on the SD card with the [Imager](https://www.raspberrypi.org/software/) or [balenaEtcher](https://www.balena.io/etcher/).
- Insert the SD card in your Rock Pi 5 and enjoy.
- Username: ***rock***
- no password 

------------

## Tips.

* If you are in need of extra space, you can delete the opencv and the opencv_contrib folder from the SD card. There are no longer needed since all libraries are placed in the /usr/ directory.
* Use a tool like [GParted](https://gparted.org/) `sudo apt-get install gparted` to expand the image to larger SD cards. We recommend a minimum of 64 GB. Deep learning simply requires a lot of space.<br/><br/>
* An example of YoloV5 running on the NPU (25 FPS) is included.

------------

## Pre-installed frameworks.

- [OpenCV](https://qengineering.eu/deep-learning-with-opencv-on-raspberry-pi-4.html) 4.6.0
- [ncnn](https://qengineering.eu/install-ncnn-on-raspberry-pi-4.html) 20210720
- [TNN](https://qengineering.eu/install-tnn-on-raspberry-pi-4.html) 0.3.0
- NPU software [rknpu2](https://github.com/rockchip-linux/rknpu2) 1.4.0
- [TeamViewer aarch64](https://www.teamviewer.com/en/download/linux/) 15.24.5

![output image]( https://qengineering.eu/github/RockPi5.webp )<br/><br/>

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 


