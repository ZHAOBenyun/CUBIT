# CUBIT
## CUBIT: A High-resolution Infrastructure Defect Dataset Fully Evaluated with Autonomous Detection Framework

**Abstract:**\
Learning-based visual inspection, integrated with unmanned robotic system, offers a more effective, efficient, and safer alternative for infrastructure inspection tasks that are traditionally heavily reliant on human labor. However, the potential of learning-based inspection methods remains limited due to the lack of publicly available, high-quality datasets. This paper presents CUBIT, a high-resolution defect detection dataset comprising more than $5500$ images with resolutions up to $8000\times6000$ which covers a broader spectrum of practical situations, backgrounds, and defect categories than existing publicly available datasets. We conduct extensive experiments to benchmark the performance of state-of-the-art real-time detection methods on our proposed dataset, validating the effectiveness of it. Moreover, based on the benchmark results, we develop a module named GIPFPP to integrate multi-scale feature, enhancing the AP by 3\% while reducing the number of parameters by 10\% on baseline model. Additionally, a real-site UAV-based inspection has been conducted to verify the reliability of the dataset.


*Sample images in CUBIT*
* The sample images in CUBIT has been shown below.* All the data are collected by autonomous unmanned systems such as UAV and UGV. Our dataset includes various scnarios and defect categories compared with the existing open-source bounding-box level defect detection dataset. 
<p align="center">
  <img src="https://github.com/ZHAOBenyun/CUBIT/blob/master/sample.png"> 
</p>

*Defect Detection Framework based on CUBIT*
* The visualization of defect detection framework based on CUBIT dataset is illustrated below *, which encompasses the entire process: data collection by autonomous unmanned system; the baseline network integrated with our GIPFPP module; the output of defect detection results. 
<p align="center">
  <img src="https://github.com/ZHAOBenyun/CUBIT/blob/master/frame.png"> 
</p>


*Prediction results on the test set of the proposed CUBIT-RGB-v1 defect dataset are shown below* 
We enlarge the prediction results in the bottom right corner of framework images above. CUBIT dataset covers three infrastructure types: **Building facade, Pavement**, and **Bridge**, and aims for three types of defect: **Crack, Spalling, and Moisture**. Rectangles indicate the output prediction box (\textcolor{red}{Red} for \textbf{Crack}, \textcolor{pink}{Pink} for \textbf{Spalling}, and \textcolor{orange}{Orange} for \textbf{Moisture}) with inferred defect type and confidence score from YOLOv6-l trained on the training set of our proposed dataset.
<p align="center">
  <img src="https://github.com/ZHAOBenyun/CUBIT/blob/master/index_show.png" width=60% height=60%>
</p>

*Qualitative visualization of UAV-based real-world experiment is shown below* On the left, our multi-UAVs inspection schematics is illustrated. On the right, the detection results of four direction façades of the building are displayed.
<p align="center">
  <img src="https://github.com/ZHAOBenyun/CUBIT/blob/master/goodman_zigzag.png">
</p>


