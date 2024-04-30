# Rock 5 image
![output image]( https://qengineering.eu/github/SDcard32GB_RockPi5_Large.webp)<br/>
## A Rock 5 image with OpenCV, ncnn, TNN and NPU
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>

------------

## Installation.

- Get a 32 GB (minimal) SD card holding the image. 
- Download the `RockPi5.img.xz` image (2.8 GByte) from our [Sync](https://ln5.sync.com/dl/b9c189080/csvcycve-qn6f2zt8-49z54nm6-m9gvzbf3) site. 
- Flash the image on the SD card with the [Imager](https://www.raspberrypi.org/software/) or [balenaEtcher](https://www.balena.io/etcher/).
- Insert the SD card in your Rock 5 and enjoy.
- Username: ***rock***
- no password 

------------

## Model performance benchmark(FPS)

All models, with C++ examples, can be found on the SD image.<br>

| demo             | model_name                   | inputs_shape            | dtype | Rock 5        |
| ---------------- | ---------------------------- | ----------------------- | ----- | ------------- |
| yolov5           | yolov5s_relu                 | [1, 3, 640, 640]        | INT8  | 50.0          |
|                  | yolov5n                      | [1, 3, 640, 640]        | INT8  | 58.8          |
|                  | yolov5s                      | [1, 3, 640, 640]        | INT8  | 37.7          |
|                  | yolov5m                      | [1, 3, 640, 640]        | INT8  | 16.2          |
| yolov6           | yolov6n                      | [1, 3, 640, 640]        | INT8  | 63.0          |
|                  | yolov6s                      | [1, 3, 640, 640]        | INT8  | 29.5          |
|                  | yolov6m                      | [1, 3, 640, 640]        | INT8  | 15.4          |
| yolov7           | yolov7-tiny                  | [1, 3, 640, 640]        | INT8  | 53.4          |
|                  | yolov7                       | [1, 3, 640, 640]        | INT8  | 9.4           |
| yolov8           | yolov8n                      | [1, 3, 640, 640]        | INT8  | 53.1          |
|                  | yolov8s                      | [1, 3, 640, 640]        | INT8  | 28.5          |
|                  | yolov8m                      | [1, 3, 640, 640]        | INT8  | 12.1          |
| yolox            | yolox_s                      | [1, 3, 640, 640]        | INT8  | 30.0          |
|                  | yolox_m                      | [1, 3, 640, 640]        | INT8  | 12.9          |
| ppyoloe          | ppyoloe_s                    | [1, 3, 640, 640]        | INT8  | 28.8          |
|                  | ppyoloe_m                    | [1, 3, 640, 640]        | INT8  | 13.1          |
| yolov5_seg       | yolov5n-seg                  | [1, 3, 640, 640]        | INT8  | 9.4           |
|                  | yolov5s-seg                  | [1, 3, 640, 640]        | INT8  | 7.8           |
|                  | yolov5m-seg                  | [1, 3, 640, 640]        | INT8  | 6.1           |
| yolov8_seg       | yolov8n-seg                  | [1, 3, 640, 640]        | INT8  | 8.9           |
|                  | yolov8s-seg                  | [1, 3, 640, 640]        | INT8  | 7.3           |
|                  | yolov8m-seg                  | [1, 3, 640, 640]        | INT8  | 4.5           |
| ppseg	           | ppseg_lite_1024x512          |	[1, 3, 512, 512]	      | INT8	| 27.5          |
| RetinaFace       | RetinaFace_mobile320         | [1, 3, 320, 320]        | INT8  | 243.6         |
|                  | RetinaFace_resnet50_320      | [1, 3, 320, 320]        | INT8  | 43.4          |
| PPOCR-Det        | ppocrv4_det                  | [1, 3, 480, 480]        | INT8  | 31.5          |
| PPOCR-Rec        | ppocrv4_rec                  | [1, 3, 48, 320]         | FP16  | 35.7          |

* Due to the pixel-wise filling and drawing, segmentation models are relatively slow

------------

## Tips.

* If you need extra space delete the opencv and the opencv_contrib folder from the SD card. They are no longer needed since all libraries are stored in the /usr/ directory.
* Use a tool like [GParted](https://gparted.org/) `sudo apt-get install gparted` to expand the image to larger SD cards. We recommend a minimum of 64 GB. Deep learning requires a lot of space.<br/>
* An example of YoloV5 running on the NPU (25 FPS) is included.

------------

## Pre-installed frameworks.

- [OpenCV](https://qengineering.eu/deep-learning-with-opencv-on-raspberry-pi-4.html) 4.9.0
- [ncnn](https://qengineering.eu/install-ncnn-on-raspberry-pi-4.html) 20240410
- NPU [rknpu2](https://github.com/airockchip/rknn-toolkit2/tree/master/rknpu2) 1.5.2
- NPU [model zoo](https://github.com/airockchip/rknn_model_zoo) 2.0.0
- NPU [model zoo models](https://github.com/Qengineering/rknn_model_zoo) 2.0.0
- [TeamViewer aarch64](https://www.teamviewer.com/en/download/linux/) 15.24.5

------------

### Thanks.
A more than special thanks to [***Stuart Naylor***](https://forum.radxa.com/u/stuartiannaylor/summary), who, ever so kindly, provided us the Rock Pi 5 for free.

------------

![output image]( https://qengineering.eu/github/RockPi5.webp )<br/><br/>

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 


