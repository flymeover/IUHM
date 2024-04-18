Code and data used in Sensors "Research on learning data and data format for reducing quan-tization error in stereo vision system":

Using the code at https://github.com/ardiya/gc_net, we created codes for learning and evaluation using Disparity data and Normalized z-distance data as output values.
The dataset used in existing stereo matching research consists of stereo image pairs and disparity data, where the disparity data is expressed as an integer with a limited number of digits. The distance must be a continuous value, but if the stereo matching algorithm is learned and calculated using the disparity value expressed as a quantized value, quantization error will inevitably occur.
To verify that the distance prediction performance of the stereo matching algorithm is improved by collecting and learning real-type distance data rather than disparity values expressed as quantized values, the test data set used in the study, model data that has already completed learning, and The performance of the model can be evaluated using the evaluation code.
The codes were written based on Python3 and TensorFlow2 in a Jupyter Notebook environment.
Users can download the test data, modify the code according to the saved path, and run it.
The results of learning GC-Net using disparity and normalized z-distance are shown in the following figures and table.
It can be seen that the disparity or distance error (Mean Absolute Error) is reduced in the model learned using real normalized z-distance.

![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/a7873e54-c3c2-4105-825a-29971b0cff7a)

Fig1. Comparison of Disparity Map based on original data and model pre-diction results used for training and evaluation:
(Top) LiDAR data; (Middle) GC-Net with disparity data; (Bottom) GC-Net with normalized Z-distance data.
 
![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/5b992b18-19de-4ddc-a8de-ea9e06a96d90)

Fig2. Comparison of Depth Map based on original data and model pre-diction results used for training and evaluation:
(Top) LiDAR data; (Middle) GC-Net with disparity data; (Bottom) GC-Net with normalized Z-distance data.


Table. Comparison of predicted values using Z-distance data and Disparity data

![image](https://github.com/flymeover/ReduceQuantizedErrorOfDisparity/assets/167387983/37f41e9b-93a9-4557-a01e-07243858460a)

