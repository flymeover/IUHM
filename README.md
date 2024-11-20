"Resource-Constrained Stereo Matching for Agricultural Applications: An Efficient and Accurate Approach with Optimized Memory Usage in Field and Greenhouse Environments"

[Proposed Model]

Integrated U-Net model with histogram-equalized mono channel stereo data (IUHM)

![image](https://github.com/user-attachments/assets/48e6205c-30a3-4157-810f-1fdb47aec45d)


[Stereo Matching Algorithm Code]

The codes were written based on Python3 and TensorFlow2 in a Jupyter Notebook environment.

[Scene Flow Data]

Users can download data, modify the test code according to the saved path, and run it.
https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html


[Tomato Greenhouse Data]

Users can download it from the following path:
https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing

[Result]

The proposed model, IUHM surpasses existing models such as geometry and context network (GC-Net) and pyramid stereo matching network (PSMNet) in terms of disparity prediction accuracy and computational speed, consuming less than one-third of the memory.


![image](https://github.com/user-attachments/assets/42829cbc-ad43-45d8-81a6-cf1901588931)

   Figure Prediction results of models by retraining iterations with tomato dataset.



Table Calculation resource usage by models predicted with tomato dataset (image size: 960 × 544).
![image](https://github.com/user-attachments/assets/109c25c5-fa5b-42dd-af1c-e91d11a4e224)
