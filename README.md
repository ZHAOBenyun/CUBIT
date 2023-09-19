<h1 style="text-align: center; font-size: 36px; font-family: 'Sama Devanagari';"> CUBIT: A High-Resolution Infrastructure Defect Dataset <br /> Fully Evaluated with Autonomous Detection Framework
</h1>

<h3 style="text-align: center; font-size: 25px; font-family: 'Sama Devanagari';"> Submitted to International Conference on Acoustics, Speech, & Signal Processing 2024 (ICASSP 2024)
</h3>


<div style=" text-align: center; font-size: 17px;">
Benyun Zhao<sup>1</sup>, Xunkuai Zhou<sup>2</sup>, Guidong Yang<sup>1</sup>, Junjie Wen<sup>1</sup>, Jihan Zhang<sup>1</sup>,  Xi Chen<sup>1</sup>, and <a href="http://www.mae.cuhk.edu.hk/~bmchen/">Ben M. Chen</a><sup>1</sup>, IEEE Fellow
</div>
<br>
<div  style="text-align: center; font-size: 17px;" >
1.Department of Mechanical and Automation Engineering, The Chinese University of Hong Kong  <br />       2.School of Electronics and Information Engineering,Tongji University

</div>
<div style="display: flex; flex-direction: row; margin: 10px auto; justify-content: center" > 

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px;border: none; border-radius: 5px;">
<a href="#" style="color: white; text-decoration: none;">Paper (coming soon)</a>
</button>

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px; border: none; border-radius: 5px;">
<a href="#" style="color: white; text-decoration: none;">Supplementary</a>
</button>
</div>

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px;border: none; border-radius: 5px;">
<a href="https://zhaobenyun.github.io/CUBIT/" style="color: white; text-decoration: none;">Project Page</a>
</button>


<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Abstract</h2>
</div>

Learning-based visual inspection, integrated with unmanned robotic system, offers a more effective, efficient, and safer alternative for infrastructure inspection tasks that are traditionally heavily reliant on human labor. However, the potential of learning-based inspection methods remains limited due to the lack of publicly available, high-quality datasets. This paper presents CUBIT, a high-resolution defect detection dataset comprising more than $5500$ images with resolutions up to $8000\times6000$ which covers a broader spectrum of practical situations, backgrounds, and defect categories than existing publicly available datasets. We conduct extensive experiments to benchmark the performance of state-of-the-art real-time detection methods on our proposed dataset, validating the effectiveness of it. Moreover, based on the benchmark results, we develop a module named GIPFPP to integrate multi-scale feature, enhancing the AP by 3\% while reducing the number of parameters by 10\% on baseline model. Additionally, a real-site UAV-based inspection has been conducted to verify the reliability of the dataset.

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Sample images in CUBIT</h2>
</div>
The sample images in CUBIT has been shown below. All the data are collected by autonomous unmanned systems such as UAV and UGV. Our dataset includes various scenarios and defect categories compared with the existing open-source bounding-box level defect detection dataset. 

Image Resolution | Year | Structure Type | Number of Images | Defect Type | Annotation Level
--- | --- | --- | --- | --- | --- |
4624x3472, 8000x6000 | 2023 | Building, Pavement, Bridge | 5527 | Crack, Spalling, Moisture | Bounding-box Level

<p align="center">
  <img src="./sample.png" width=80% height=80%> 
</p>

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Defect Detection Framework based on CUBIT</h2>
</div>
The visualization of defect detection framework based on CUBIT dataset is illustrated below, which encompasses the entire process: data collection by autonomous unmanned system; the baseline network integrated with our GIPFPP module; the output of defect detection results. 
<p align="center">
  <img src="./frame.png" width=80% height=80%> 
</p>


<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Prediction results on the test set of the proposed CUBIT-RGB-v1 defect dataset are shown below</h2>
</div>
We enlarge the prediction results in the bottom right corner of framework images above. CUBIT dataset covers three infrastructure types: Building facade, Pavement, and Bridge, and aims for three types of defect: Crack, Spalling, and Moisture. Rectangles indicate the output prediction box Red for Crack, Pink for Spalling, and Orange for Moisture with inferred defect type and confidence score from YOLOv6-n+GIPFPP modle trained on the training set of our proposed dataset.
<p align="center">
  <img src="./index_show.png" width=70% height=70%>
</p>


<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Multi-UAV-based Real-world Infrastructure Defects Inspection</h2>
</div>
Qualitative visualization of multi-UAV-based real-world experiment is shown below. On the left, our multi-UAVs inspection schematics is illustrated. On the right, the detection results of four direction façades of the building are displayed.
<p align="center">
  <img src="./goodman_zigzag.png" width=80% height=80%>
</p>


<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Acknowledgement</h2>
</div>
This work was supported by the InnoHK of the Government of the Hong Kong Special Administrative Region via the Hong Kong Centre for Logistics Robotics.


