<h1 style="text-align: center; font-size: 36px; font-family: 'Sama Devanagari';"> CUBIT: A High-resolution Infrastructure Defect Dataset Fully Evaluated with Autonomous Detection Framework
    <div style="text-align: center; font-size: 20px; font-family: 'Sama Devanagari';">    Submitted to International Conference on Acoustics, Speech, & Signal Processing
</div>
</h1>

<div style=" text-align: center; font-size: 17px;">
Benyun Zhao<sup>1</sup>, Xunkuai Zhou<sup>1, 2</sup>, Guidong Yang<sup>1</sup>, Junjie Wen<sup>1</sup>, Jihan Zhang<sup>1</sup>,  Xi Chen<sup>1</sup>, and <a href="http://www.mae.cuhk.edu.hk/~bmchen/">Ben M. Chen</a><sup>1</sup>, Fellow, IEEE
</div>
<br>
<div  style="text-align: center; font-size: 17px;" >
1.Department of Mechanical and Automation Engineering, The Chinese University of Hong Kong &nbsp; &nbsp; &nbsp; 2.School of Electronics and Information Engineering,Tongji University

</div>
<div style="display: flex; flex-direction: row; margin: 10px auto; justify-content: center"> 

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px;border: none; border-radius: 5px;">
<a href="https://www.overleaf.com/" style="color: white; text-decoration: none;">Paper</a>
</button>

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px; border: none; border-radius: 5px;">
<a href="https://github.com/ZHAOBenyun/CUBIT" style="color: white; text-decoration: none;">Dataset</a>
</button>

<button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px; border: none; border-radius: 5px;">
<a href="#" style="color: white; text-decoration: none;">Supplementary</a>
</button>
</div>


<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Abstract</h2>
</div>


Learning-based visual inspection, integrated with unmanned robotic system, offers a more effective, efficient, and safer alternative for infrastructure inspection tasks that are traditionally heavily reliant on human labor. However, the potential of learning-based inspection methods remains limited due to the lack of publicly available, high-quality datasets. This paper presents CUBIT, a high-resolution defect detection dataset comprising more than $5500$ images with resolutions up to $8000\times6000$ which covers a broader spectrum of practical situations, backgrounds, and defect categories than existing publicly available datasets. We conduct extensive experiments to benchmark the performance of state-of-the-art real-time detection methods on our proposed dataset, validating the effectiveness of it. Moreover, based on the benchmark results, we develop a module named GIPFPP to integrate multi-scale feature, enhancing the AP by 3\% while reducing the number of parameters by 10\% on baseline model. Additionally, a real-site UAV-based inspection has been conducted to verify the reliability of the dataset.

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h3>Sample images in CUBIT</h3>
</div>
* The sample images in CUBIT has been shown below.* All the data are collected by autonomous unmanned systems such as UAV and UGV. Our dataset includes various scnarios and defect categories compared with the existing open-source bounding-box level defect detection dataset. 
<p align="center">
  <img src="./sample.png"> 
</p>

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h3>Defect Detection Framework based on CUBIT</h3>
</div>

* The visualization of defect detection framework based on CUBIT dataset is illustrated below *, which encompasses the entire process: data collection by autonomous unmanned system; the baseline network integrated with our GIPFPP module; the output of defect detection results. 
<p align="center">
  <img src="./frame.png"> 
</p>

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h3>Prediction results on the test set of the proposed CUBIT-RGB-v1 defect dataset are shown below
</h3>
</div>

We enlarge the prediction results in the bottom right corner of framework images above. CUBIT dataset covers three infrastructure types: **Building facade, Pavement**, and **Bridge**, and aims for three types of defect: **Crack, Spalling, and Moisture**. Rectangles indicate the output prediction box (\textcolor{red}{Red} for \textbf{Crack}, \textcolor{pink}{Pink} for \textbf{Spalling}, and \textcolor{orange}{Orange} for \textbf{Moisture}) with inferred defect type and confidence score from YOLOv6-l trained on the training set of our proposed dataset.
<p align="center">
  <img src="./index_show.png">
</p>

*Qualitative visualization of UAV-based real-world experiment is shown below* On the left, our multi-UAVs inspection schematics is illustrated. On the right, the detection results of four direction façades of the building are displayed.
<p align="center">
  <img src="./goodman_zigzag.png">
</p>


