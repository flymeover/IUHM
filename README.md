[Under construction]

# "Resource-Constrained Stereo Matching for Greenhouse Tomatoes and Napa Cabbages: An Efficient and Accurate Approach with Optimized Memory Usage"

## [Proposed Model]

Integrated U-Net model with histogram-equalized mono channel stereo data (IUHM)

### **Figure. IUHM model structure and features.**
![image](https://github.com/user-attachments/assets/51ac092a-1b3b-4d46-9820-8368a4632980)
![image](https://github.com/user-attachments/assets/48e6205c-30a3-4157-810f-1fdb47aec45d)


To evaluate the performance of the IUHM model, GC-Net and PSMNet were trained and evaluated together.

**IUHM, GC-Net, PSMNet Model's test code in github : GCNet_predict_tomato.ipynb, PSMNet_predict_tomato.ipynb, IUHM_predict_tomato.ipynb**

**IUHM, GC-Net, PSMNet Model's save data available for download from the link below : saved_model.zip**

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing

## [Stereo Matching Algorithm Code]

The codes were written based on Python3 and TensorFlow2 in a Jupyter Notebook environment.

(The code or data path that loads learning/evaluation data must be modified and executed according to the path where the user saved the data.)

※ Refer to the Jupyter Notebook environment file (kcy.yaml file) to install the libraries required to run the code
   
## [Scene Flow Data]

Pretraining by refining only data with disparity range of 0-160

**Dataset for pretraining :**

Users can download data, modify the test code according to the saved path, and run it.

https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html

## [Tomato Greenhouse Data]

This study utilized stereo images and LiDAR data collected from tomato plants cultivated in a greenhouse managed by the Korea Institute of Science and Technology (KIST) in Gangwon-do, South Korea. The data collection was conducted over a two-month period, from July to August 2024.

Owing to the interference of strong sunlight during daylight hours, LiDAR measurements were exclusively taken at night, facilitated by light-emitting diode (LED) illumination.


### **Figure. Data collection location and equipment:(a) landscape of KIST greenhouse and (b) multifunction camera setup (LED bar, dual Intel Realsense L515s, control box).**
![image](https://github.com/user-attachments/assets/a31c504a-04d5-4802-bd65-4308dbfd0f7f)

### **Figure. Range of distance from tomatoes to MFC in KIST’s greenhouse.**
![image](https://github.com/user-attachments/assets/d67b6212-3a7a-4fb1-af1a-97fe7428627f)

### **Figure. Example of original data collected by the MFC in KIST’s greenhouse: (a) left camera’s Image, (b) right camera’s Image, and (c) left disparity data converted by LiDAR depth data.**
![image](https://github.com/user-attachments/assets/a5ca5580-56c7-49c7-9003-122c6ac4402f)


**Dataset for retraining and evaluation :**

tomato_data.zip-tomato_data.z23 (Compressed file divided into 24 parts)

Users can download it from the following path:

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing



## [Result]

The proposed model, IUHM surpasses existing models such as geometry and context network (GC-Net) and pyramid stereo matching network (PSMNet)
in terms of disparity prediction accuracy and computational speed,
consuming less than one-third of the memory in tomato greenhouse dataset.

### **Figure. Prediction results of models by retraining iterations with tomato dataset.**
![image](https://github.com/user-attachments/assets/42829cbc-ad43-45d8-81a6-cf1901588931)

### **Table. Calculation resource usage by models predicted with tomato dataset (image size: 960 × 544).**
![image](https://github.com/user-attachments/assets/e990a3ea-594a-4a8b-b8f9-07be78c07c07)

Evaluation Data(Disparity Error and Disparity map) :

IUHM_H4WW6_iter177.zip, PSMNet_iter196.zip, GCNet_iter52.zip

Users can download it from the following path:

https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=sharing


> [!NOTE]
> **Download trained parameter data and the tomato greenhouse dataset.**
> 
> The trained parameter data for the IUHM, GC-Net, and PSMNet models, along with the Scene Flow dataset and the tomato greenhouse dataset, are available for download. To access them, please follow these steps:
>
> Request access: Visit the Google Drive link (https://drive.google.com/drive/folders/1C9imrSk1bZTLQYUEmxgvCfZMEFtMwPLn?usp=drive_link) and briefly state your purpose for downloading the data. Your access will be reviewed and granted upon confirmation.
> 
> Download timeframe: Once approved, you will have 3 days to download the data due to sharing speed and daily transfer limits.
> 
> **Important Note:**
> 
> Downloading or using this data for commercial purposes by any individual, group, institution, company, or data collection system not involved in this study is strictly prohibited.
