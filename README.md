# CUBIT-RGB-v1
Visual Detection of Infrastructure Defects: A Comprehensive Experiment Evaluation of Deep Learning

**Abstract:**\
Diagnosing infrastructure defects is a crucial yet highly complex task that can be more safely and efficiently performed through machine vision instead of human visual inspection. Deep learning-based autonomous visual methods have demonstrated superior performance in numerous object detection tasks, but they have not been thoroughly explored for infrastructure inspection due to the lack of high-quality datasets. To address this gap, we present CUBIT-RGB-v1, a high-resolution infrastructure defects dataset comprising over 5500 images with resolutions ranging from $4624\times3472$ to $8000\times6000$ obtained using professional acquisition equipment on various robotic platforms in multiple scenarios. In contrast to other datasets, CUBIT-RGB-v1 covers a broader spectrum of practical situations, backgrounds, and defect types, making it more extensive and comprehensive. Extensive benchmarking experiments have been conducted by using more than 25 state-of-the-art deep neural networks to validate the feasibility of our dataset. To the best of our knowledge, this is the first work to comprehensively benchmark autonomous infrastructure inspection performances on high-resolution images, providing references for future researchers to develop new specific defect detection solutions. The reliability and feasibility of our dataset have been further demonstrated by utilizing an object detection network trained on our dataset for real-world building inspection. 

<img src="https://github.com/CUHK-USR-Group/Defect-Dataset/blob/main/Taxonomy.PNG">

*Figure 1:* \
Prediction results on the test set of the proposed CUBIT-RGB-v1 defect dataset. The CUBIT-RGB-v1 dataset covers three infrastructure types: Building facade, Pavement,
and Bridge, and aims for three types of defect: Crack, Spalling, and Moisture. Red Rectangle indicates the output prediction box with inferred defect type and confidence score from YOLOv6-l trained on the training set of our proposed dataset


