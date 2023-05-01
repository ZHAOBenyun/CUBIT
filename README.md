# CUBIT-RGB-v1
Visual Detection of Infrastructure Defects: A Comprehensive Experiment Evaluation of Deep Learning

**Abstract:**\
Diagnosing infrastructure defects is a crucial yet highly complex task that can be more safely and efficiently performed through machine vision instead of human visual inspection. Deep learning-based autonomous visual methods have demonstrated superior performance in numerous object detection tasks, but they have not been thoroughly explored for infrastructure inspection due to the lack of high-quality datasets. To address this gap, we present CUBIT-RGB-v1, a high-resolution infrastructure defects dataset comprising over 5500 images with resolutions ranging from $4624\times3472$ to $8000\times6000$ obtained using professional acquisition equipment on various robotic platforms in multiple scenarios. In contrast to other datasets, CUBIT-RGB-v1 covers a broader spectrum of practical situations, backgrounds, and defect types, making it more extensive and comprehensive. Extensive benchmarking experiments have been conducted by using more than 25 state-of-the-art deep neural networks to validate the feasibility of our dataset. To the best of our knowledge, this is the first work to comprehensively benchmark autonomous infrastructure inspection performances on high-resolution images, providing references for future researchers to develop new specific defect detection solutions. The reliability and feasibility of our dataset have been further demonstrated by utilizing an object detection network trained on our dataset for real-world building inspection. 

*Sample images from InnoAIR-HK-v1 dataset are shown below.* The first row of images is crack defects on building facades. The second row is about spalling, and the third is about moisture. These images are collected by UAVs and DSLR in the old districts of Hong Kong. \
<img src="https://github.com/ZHAOBenyun/CUBIT-RGB-v1/blob/master/sample-min.png"> 


*Prediction results on the test set of the proposed CUBIT-RGB-v1 defect dataset are shown below.* The CUBIT-RGB-v1 dataset covers three infrastructure types: **Building facade, Pavement**, and **Bridge**, and aims for three types of defect: \textbf{Crack, Spalling, and Moisture}. **Red Rectangle** indicates the output prediction box with inferred defect type and confidence score from YOLOv6-l trained on the training set of our CUBIT-RGB-v1 dataset.\
<img src="https://github.com/ZHAOBenyun/CUBIT-RGB-v1/blob/master/index_show-min.png" width=60% height=60%>

*Qualitative visualization of real-world experiment is shown below.* On the left, three of our UAVs are cooperating to detect the building. On the right, each of the four columns shows the results of the facade in one direction of this building. The inspection results of this logistics building demonstrate that the deep learning models trained on CUBIT-RGB-v1 can be easily transferred to real-world inspection application. \
<img src="https://github.com/ZHAOBenyun/CUBIT-RGB-v1/blob/master/goodman-min.png">


