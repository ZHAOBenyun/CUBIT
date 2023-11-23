<h1 style="text-align: center; font-size: 36px; font-family: 'Roboto';"> CUBIT: A High-resolution Infrastructure Defect Dataset <br> Fully Evaluated with Autonomous Detection Framework
    <div style="text-align: center; font-size: 20px; font-family: 'Georgia';">   
Submitted to International Conference on Acoustics, Speech, & Signal Processing 2024 (ICASSP 2024)
</div>
</h1>

<div style=" text-align: center; font-size: 17px;">
Benyun Zhao<sup>1</sup>, Xunkuai Zhou<sup>2</sup>, Guidong Yang<sup>1</sup>, Junjie Wen<sup>1</sup>, Jihan Zhang<sup>1</sup>,  Xi Chen<sup>1</sup>, and <a href="http://www.mae.cuhk.edu.hk/~bmchen/">Ben M. Chen</a><sup>1</sup>, IEEE Fellow
</div>

<div  style="text-align: center; font-size: 17px;" >
1.Department of Mechanical and Automation Engineering, The Chinese University of Hong Kong  <br />       2.School of Electronics and Information Engineering,Tongji University

</div>
<div style="display: flex; flex-direction: row; margin: 10px auto; justify-content: center"> 

<button style="background-color: #c3bebe; color: white;margin-right: 15px; padding: 10px 15px;border: none; border-radius: 5px;">
<a href="" style="color: white; text-decoration: none;">Paper</a>
</button>

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px; border: none; border-radius: 5px;">
<a href="https://github.com/ZHAOBenyun/CUBIT" style="color: white; text-decoration: none;">Dataset</a>
</button>

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px; border: none; border-radius: 5px;">
<a href="./ICASSP_2024_Appendix.pdf" style="color: white; text-decoration: none;">Supplementary </a>
</button>

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px; border: none; border-radius: 5px;">
<a href="./ICASSP2024_Rebuttal.pdf" style="color: white; text-decoration: none;">Rebuttal </a>
</button>
</div>


<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Abstract</h2>
</div>

<div style="text-align: justify; text-justify:inter-ideograph;">
Learning-based visual inspection, integrated with unmanned robotic system, offers a more effective, efficient, and safer alternative for infrastructure inspection tasks that are traditionally heavily reliant on human labor. However, the potential of learning-based inspection methods remains limited due to the lack of publicly available, high-quality datasets. This paper presents CUBIT, a high-resolution defect detection dataset comprising more than <strong><em>5500</em></strong> images with resolutions up to <strong><em>8000 x 6000</em></strong> which covers a broader spectrum of practical situations, backgrounds, and defect categories than existing publicly available datasets. We conduct extensive experiments to benchmark the performance of state-of-the-art real-time detection methods on our proposed dataset, validating the effectiveness of it. Moreover, based on the benchmark results, we develop a module named GIPFPP to integrate multi-scale feature, enhancing the AP by 3% while reducing the number of parameters by 10% on baseline model. Additionally, a real-site UAV-based inspection has been conducted to verify the reliability of the dataset.
</div>

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h3>Sample images in CUBIT</h3>
</div>

<div style="text-align: justify; text-justify:inter-ideograph;">

 The sample images in CUBIT has been shown below. All the data are collected by autonomous unmanned systems such as UAV and UGV. Our dataset includes various scnarios and defect categories compared with the existing open-source bounding-box level defect detection dataset. 

</div>

<p align="center">
  <img src="./sample.png" style="width: 80%;"> 
</p>

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h4> The Comparison between Existing Bounding-box-level Defect Dataset with CUBIT
</h4>
</div>

| Dataset       | Num. of Images | Resolution          | Data Collection Platform           | Category               | Scenario                 | Material             | Experiments                                  |
|---------------|----------------|----------------------|------------------------------------|------------------------|--------------------------|----------------------|-----------------------------------------------|
| RDD-2018      | 9053           | 600x600              | Smartphones                        | Crack, Corrosion       | Pavement                 | Asphalt              | SSD                                           |
| RDD-2019      | 13135          | 600x600              | Smartphones                        | Crack, Corrosion       | Pavement                 | Asphalt              | SSD                                           |
| RDD-2020      | 26336          | 600x600, 720x720     | Smartphones                        | Crack, Pothole         | Pavement                 | Asphalt              | SSD                                           |
| RDD-2022      | 47420          | 512x512, 600x600, 720x720, 3650x2044 | Smartphones, Hand-held cameras, UAV cameras, Google street view | Crack, Pothole     | Pavement             | Asphalt              | -                                             |
| PID           | 7237           | 640x640              | Crawled from Internet               | Crack                  | Pavement                 | Asphalt              | YOLOv2, Fast R-CNN                            |
| Murad         | 2620           | up to 838x809        | Smartphones                        | Crack                  | Pavement                 | Asphalt              | Faster R-CNN                                  |
| CODEBRIM      | 1590           | up to 6000x4000      | Hand-held cameras, UAV Cameras     | Crack, Corrosion       | Bridge                   | Concrete             | MetaQNN, ENAS                                 |
| **CUBIT**     | **5527**       | **4624x3472 and 8000x6000** | **Cameras in Unmanned Systems**  | **Crack, Spallinig, Moisture** | **Building (65%), Pavement (29%), Bridge (6%)** | **Concrete, Asphalt, Stone** | **Faster R-CNN, PP-YOLO, PP-YOLOv2, YOLOX, YOLOv5, YOLOv7, YOLOv6, YOLOv6+GIPFPP(ours), Real-site experiment** |





<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h3>Defect Detection Framework based on CUBIT</h3>
</div>
<div style="text-align: justify; text-justify:inter-ideograph;">

The visualization of defect detection framework based on CUBIT dataset is illustrated below, which encompasses the entire process: data collection by autonomous unmanned system; the baseline network integrated with our GIPFPP module; the output of defect detection results. 

</div>

<p align="center">
  <img src="./frame.png" style="width: 80%;"> 
</p>



<div style="text-align: center; font-weight: 400; font-family: 'American Typewriter' "> 
<h3>Prediction results on the test set of the proposed CUBIT defect dataset are shown below
</h3>
</div>

<div style="text-align: justify; text-justify:inter-ideograph;">
We enlarge the prediction results in the bottom right corner of framework images above. CUBIT dataset covers three infrastructure types: <strong> Building, Pavement</strong>, and <strong>Bridge</strong>, and aims for three types of defect: <strong>Crack, Spalling</strong>, and <strong>Moisture</strong>. Rectangles indicate the output prediction box <font color="red">Red</font> for Crack, <font color="pink">Pink</font> for Spalling, and <font color="orange">Orange</font> for Moisture with inferred defect type and confidence score from YOLOv6-n+GIPFPP trained on the training set of our proposed dataset.

</div>

<p align="center">
  <img src="./index_show.png" style="width: 70%;">
</p>

<div style="text-align: center; font-weight: 400; font-family: 'American Typewriter' "> 
<h3>
Multi-UAV-Based Real-world Infrastructure Defects Inspection
</h3>
</div>
<div style="text-align: justify; text-justify:inter-ideograph;">
Qualitative visualization of UAV-based real-world experiment is shown below. On the left, our multi-UAVs inspection schematics is illustrated. On the right, the detection results of four direction façades of the building are displayed.

</div>

<p align="center">
  <img src="./goodman_zigzag.png" style="width: 80%;">
</p>
<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Acknowledgement</h2>
</div>
This work was supported by the InnoHK of the Government of the Hong Kong Special Administrative Region via the Hong Kong Centre for Logistics Robotics. Credits also to <a href="http://www.yjhuang.net"> Yijun Huang </a> for constructing the project page.


