# yolov5-tensorrt 

> port pytorch/onnx yolov5 model to run on a Jetson Nano

`ipynb` is for testing pytorch code and exporting onnx models using Google Colab

`python` code runs numpy/tensorrt implementation on Jetson Nano 

- [x] convert yolov5 onnx model to tensorrt
- [x] pre-process image 
- [x] run inference against input using tensorrt engine
- [x] post process output (forward pass)
- [x] apply nms thresholding on candidate boxes
- [x] visualize results

___

| model  |  fp precision  | input size |  time (ms)   |
| ------------- | ------------- | ---------- | ---- |
| small-simple  |  32  |  640x640x3  | 15.46 |
| small-simple  |  16  |  640x640x3  | 9.47  |