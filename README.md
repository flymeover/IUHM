# "Resource-Constrained Stereo Matching for Agricultural Applications: An Efficient and Accurate Approach with Optimized Memory Usage in Field and Greenhouse Environments"

## [Proposed Model]

Integrated U-Net model with histogram-equalized mono channel stereo data (IUHM)

![image](https://github.com/user-attachments/assets/48e6205c-30a3-4157-810f-1fdb47aec45d)

![image](https://github.com/user-attachments/assets/04ba8194-92a8-40b3-923f-f2d928e0c160)

**Figure. IUHM model structure and features.**

To evaluate the performance of the IUHM model, GC-Net and PSMNet were trained and evaluated together.


IUHM, GC-Net, PSMNet Model's save data : saved_model.zip

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing

   
   
## [Stereo Matching Algorithm Code]

![image](https://github.com/user-attachments/assets/2add8710-5c49-431f-b1f8-5fd96270e973)

The codes were written based on Python3 and TensorFlow2 in a Jupyter Notebook environment.

(The code or data path that loads learning/evaluation data must be modified and executed according to the path where the user saved the data.)

※ Refer to the Jupyter Notebook environment file (kcy.yaml file) to install the libraries required to run the code


   
   
## [Scene Flow Data]

Pretraining by refining only data with disparity range of 0-160

Dataset for pretrain :

Users can download data, modify the test code according to the saved path, and run it.

https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html




## [Tomato Greenhouse Data]

This study utilized stereo images and LiDAR data collected from tomato plants cultivated in a greenhouse managed by the Korea Institute of Science and Technology (KIST) in Gangwon-do, South Korea. The data collection was conducted over a two-month period, from July to August 2024.

![image](https://github.com/user-attachments/assets/a31c504a-04d5-4802-bd65-4308dbfd0f7f)

Figure. Data collection location and equipment:

(a) landscape of KIST greenhouse and (b) multifunction camera setup (LED bar, dual Intel Realsense L515s, control box).


![image](https://github.com/user-attachments/assets/d67b6212-3a7a-4fb1-af1a-97fe7428627f)

Figure. Range of distance from tomatoes to MFC in KIST’s greenhouse.

![image](https://github.com/user-attachments/assets/a5ca5580-56c7-49c7-9003-122c6ac4402f)

Figure. Example of original data collected by the MFC in KIST’s greenhouse: (a) left camera’s Image, (b) right camera’s Image, and (c) left disparity data converted by LiDAR depth data.

Dataset for retrain and evaluation :

tomato_data.zip-tomato_data.z23 (Compressed file divided into 24 parts)

Users can download it from the following path:

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing



## [Result]

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


### ※ Caution.

To download the pre-learned parameter data of the IUHM, GC-Net, and PSMNet models and the tomato greenhouse dataset, access the Google Drive link (https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=drive_link) and write the purpose of downloading to apply. Access will be permitted after confirmation. Due to sharing speed and daily transfer limits, downloads are allowed for up to 3 days after sharing permission is approved.
(Downloading or using the data in the link for commercial purposes by person, people, institutions, companies, and data collection system other than those who participated in this study is prohibited.)
