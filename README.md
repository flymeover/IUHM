Code and data used in Sensors "Research on learning data and data format for reducing quan-tization error in stereo vision system":
Using the code at https://github.com/ardiya/gc_net, we created codes for learning and evaluation using Disparity data and Normalized z-distance data as output values.
The codes were written based on Python3 and TensorFlow2 in a Jupyter Notebook environment.
Users can download the test data, modify the code according to the saved path, and run it.

![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/a7873e54-c3c2-4105-825a-29971b0cff7a)

Fig1. Comparison of Disparity Map based on original data and model pre-diction results used for training and evaluation:

(Top) LiDAR data; (Middle) GC-Net with disparity data; (Bottom) GC-Net with normalized Z-distance data.
 
![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/5b992b18-19de-4ddc-a8de-ea9e06a96d90)

Fig2. Comparison of Depth Map based on original data and model pre-diction results used for training and evaluation:

(Top) LiDAR data; (Middle) GC-Net with disparity data; (Bottom) GC-Net with normalized Z-distance data.

Table. Comparison of predicted values using Z-distance data and Disparity data

Data	MAE of Disparity	MAE of Normalized Z-distance
		
		
		
GC-Net (with Disparity)	6.4~6.6	0.017~0.075
GC-Net (with Normalized Z-distance)	3.0~3.2	0.007~0.008
![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/37f41e9b-93a9-4557-a01e-07243858460a)

