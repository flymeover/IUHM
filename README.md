"Resource-Constrained Stereo Matching for Agricultural Applications: An Efficient and Accurate Approach with Optimized Memory Usage in Field and Greenhouse Environments"

[Proposed Model]

Integrated U-Net model with histogram-equalized mono channel stereo data (IUHM)

![image](https://github.com/user-attachments/assets/48e6205c-30a3-4157-810f-1fdb47aec45d)

![image](https://github.com/user-attachments/assets/04ba8194-92a8-40b3-923f-f2d928e0c160)


IUHM, GC-Net, PSMNet Model's save data : saved_model.zip

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing


[Stereo Matching Algorithm Code]

![image](https://github.com/user-attachments/assets/2add8710-5c49-431f-b1f8-5fd96270e973)

The codes were written based on Python3 and TensorFlow2 in a Jupyter Notebook environment.

[Scene Flow Data]

Dataset for pretrain :

Users can download data, modify the test code according to the saved path, and run it.

https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html


[Tomato Greenhouse Data]

Dataset for retrain and evaluation :

tomato_data.zip-tomato_data.z23 (Compressed file divided into 24 parts)

Users can download it from the following path:

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing

[Result]

The proposed model, IUHM surpasses existing models such as geometry and context network (GC-Net) and pyramid stereo matching network (PSMNet)
in terms of disparity prediction accuracy and computational speed,
consuming less than one-third of the memory in tomato greenhouse dataset.


![image](https://github.com/user-attachments/assets/42829cbc-ad43-45d8-81a6-cf1901588931)

Figure. Prediction results of models by retraining iterations with tomato dataset.



Table. Calculation resource usage by models predicted with tomato dataset (image size: 960 × 544).
![image](https://github.com/user-attachments/assets/e990a3ea-594a-4a8b-b8f9-07be78c07c07)

Evaluation Data(Disparity Error and Disparity map) :

IUHM_H4WW6_iter177.zip, PSMNet_iter196.zip, GCNet_iter52.zip

Users can download it from the following path:

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing


※ Caution.

To download the pre-learned parameter data of the IUHM, GC-Net, and PSMNet models and the tomato greenhouse dataset, access the Google Drive link (https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=drive_link) and write the purpose of downloading to apply. Access will be permitted after confirmation. Due to sharing speed and daily transfer limits, downloads are allowed for up to 3 days after sharing permission is approved.
(Downloading or using the data in the link for commercial purposes by person, people, institutions, companies, and data collection system other than those who participated in this study is prohibited.)
