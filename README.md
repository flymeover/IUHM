Code and data used in Sensors "Research on learning data and data format for reducing quan-tization error in stereo vision system":
Using the code at https://github.com/ardiya/gc_net, we created a code for learning and evaluation using Disparity data and Normalized z-distance data as output values.
The codes were written based on Python3 and TensorFlow2 in a Jupyter Notebook environment.
Users can download the test data, modify the code according to the saved path, and run it.
 	![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/a7873e54-c3c2-4105-825a-29971b0cff7a)
     Figure. Comparison of Disparity Map based on original data and model pre-diction results used for training and evaluation:
        (Top) LiDAR data; (Middle) GC-Net with disparity data; (Bottom) GC-Net with normalized Z-distance data.
  ![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/5b992b18-19de-4ddc-a8de-ea9e06a96d90)
	   Figure. Comparison of Depth Map based on original data and model pre-diction results used for training and evaluation:
        (Top) LiDAR data; (Middle) GC-Net with disparity data; (Bottom) GC-Net with normalized Z-distance data.
