<h1 style="text-align: center; font-size: 35px; font-family: 'Sama Devanagari';"> CUBIT Dataset
</h1>

<h3 style="text-align: center; font-size: 28px; font-family: 'Sama Devanagari';"> 
High-Resolution Infrastructure Defect Detection Dataset Sourced by Unmanned Systems and Validated with Deep Learning
</h3>

<h3 style="text-align: center; font-size: 21px; font-family: 'Sama Devanagari';"> 
Automation in Construction 2024
</h3>


<div style=" text-align: center; font-size: 21px;">
Benyun Zhao<sup>1</sup>, Xunkuai Zhou<sup>2,1</sup>, Guidong Yang<sup>1</sup>, Junjie Wen<sup>1</sup>, Jihan Zhang<sup>1</sup>, Jia Dou<sup>1</sup>, Li Guang<sup>1</sup>, Xi Chen<sup>1</sup>, and <br> <a href="http://www.mae.cuhk.edu.hk/~bmchen/">Ben M. Chen</a><sup>1</sup> IEEE Fellow
</div>
<div  style="text-align: center; font-size: 18px;" >
1.Department of Mechanical and Automation Engineering, The Chinese University of Hong Kong <br>   
2.School of Electronics and Information Engineering,Tongji University
</div>


<br>
<div style="display: flex; flex-direction: row; margin: 10px auto; justify-content: center" > 
<button style="background-color: #000000; color: white;margin-centre: 15px; padding: 10px 15px;border: none; border-radius: 5px;">
<a href="https://authors.elsevier.com/a/1ixzx3IhXM-IYB" style="color: white; text-decoration: none;">Paper from Automation in Construction</a>
</button>
</div>

<!-- <button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px; border: none; border-radius: 5px;">
<a href="https://zhaobenyun.github.io/CUBIT/ICASSP_2024_Appendix.pdf" style="color: white; text-decoration: none;">Supplementary;</a>
</button> -->

<!-- <button style="background-color: #000000; color: white;margin-right: 15px; padding: 10px 15px;border: none; border-radius: 5px;">
<a href="https://zhaobenyun.github.io/CUBIT/" style="color: white; text-decoration: none;">Project Page;</a>
</button> -->

<br>
<button style="background-color: #000000; color: white; margin: 0 auto; padding: 10px 15px;border: none; border-radius: 5px;">
Dataset can be available at: <br><a href="https://drive.google.com/drive/folders/1LWwEKQ8rSB97fCRD4sG7b6UcK40rSdA2?usp=drive_link" style="color: white; text-decoration: none;">https://drive.google.com/drive/folders/1LWwEKQ8rSB97fCRD4sG7b6UcK40rSdA2?usp=drive_link</a>
</button>

<!-- <div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Abstract</h2>
</div>

Learning-based visual inspection, integrated with unmanned robotic system, offers a more effective, efficient, and safer alternative for infrastructure inspection tasks that are traditionally heavily reliant on human labor. However, the potential of learning-based inspection methods remains limited due to the lack of publicly available, high-quality datasets. This paper presents CUBIT, a high-resolution defect detection dataset comprising more than $5500$ images with resolutions up to $8000\times6000$ which covers a broader spectrum of practical situations, backgrounds, and defect categories than existing publicly available datasets. We conduct extensive experiments to benchmark the performance of state-of-the-art real-time detection methods on our proposed dataset, validating the effectiveness of it. Moreover, based on the benchmark results, we develop a module named GIPFPP to integrate multi-scale feature, enhancing the AP by 3\% while reducing the number of parameters by 10\% on baseline model. Additionally, a real-site UAV-based inspection has been conducted to verify the reliability of the dataset. -->

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Sample images in CUBIT</h2>
</div>
The sample images in CUBIT has been shown below. All the data are collected by autonomous unmanned systems such as UAV and UGV. Our dataset includes various infrastructure scenarios and defect categories, which is more plantiful than the existing open-source bounding-box-level defect detection dataset. 

Image Resolution | Year | Structure Type | Number of Images | Defect Type | Annotation Level
--- | --- | --- | --- | --- | --- |
4624x3472, 8000x6000 | 2023 | Building, Pavement, Bridge | 5527 | Crack, Spalling, Moisture | Bounding-box Level

<p align="center">
  <img src="./sample.png" width=80% height=80%> 
</p>

<!-- <div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Defect Detection Framework based on CUBIT</h2>
</div>
The visualization of defect detection framework based on CUBIT dataset is illustrated below, which encompasses the entire process: data collection by autonomous unmanned system; the baseline network integrated with our GIPFPP module; the output of defect detection results. 
<p align="center">
  <img src="./frame.png" width=80% height=80%> 
</p> -->

<div style="text-align: center; font-family: 'American Typewriter'; font-weight: 400; "> 
<h2>Acknowledgement</h2>
</div>
This work was supported by the InnoHK of the Government of the Hong Kong Special Administrative Region via the Hong Kong Centre for Logistics Robotics. Credits also to <a href="http://www.yjhuang.net/" style="color: white; text-decoration: none;">Yijun Huang</a> for constructing the project page.


