Object Detection using Darknet + yolov4 

Requirements
 * OpenCV - place in C:\ drive 
 * Cuda Version 10.2
 * CuDnn version applicable to Cuda version
	put cudnn.dll file in darknet\build\darknet\x64
 * Visual Studio 2019
 * GPU drivers
 * downlaod yoloV4.weights from 
	put in darknet\build\darknet\x64

How to train Yolo V4 
 * Every required files are already in placed need coco dataset images only 
	place the train and val images in respective folder as mentioned down
	darknet\scripts\coco\images\train
	darknet\scripts\coco\images\val
 * Open command line 
 * change the directory to darknet\build\darknet\x64
 * Run command ./darknet detector train cfg/coco.data cfg/yolov4.cfg csdarknet53-omega.conv.105

Object detection:
 * Open command line 
 * change the directory to darknet\build\darknet\x64
 * Run command ./darknet detector test cfg/coco.data cfg/yolov4.cfg backup/yolov4_final.weights image-path/imageName -ext_output
 