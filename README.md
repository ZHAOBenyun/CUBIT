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
<a href="https://doi.org/10.1016/j.autcon.2024.105405" style="color: white; text-decoration: none;">Paper from Automation in Construction</a>
</button>
</div>

<!-- <br>
<button style="background-color: #000000; color: white; margin: 0 auto; padding: 10px 15px;border: none; border-radius: 5px;">
Dataset can be available at: <br><a href="https://mycuhk-my.sharepoint.com/:f:/g/personal/1155145791_link_cuhk_edu_hk/EvIGO4s7idhAuIj_WrfJ3wgB5HS6bSfPbce8WJxqLEwEWA?e=ftelDM" style="color: white; text-decoration: none;">https://mycuhk-my.sharepoint.com/:f:/g/personal/1155145791_link_cuhk_edu_hk/EvIGO4s7idhAuIj_WrfJ3wgB5HS6bSfPbce8WJxqLEwEWA?e=ftelDM</a>
</button> -->


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
This work was supported by the InnoHK of the Government of the Hong Kong Special Administrative Region via the Hong Kong Centre for Logistics Robotics. 
Credits also to <a href="http://www.yjhuang.net/" style="color: white; text-decoration: none;">Yijun Huang</a> for constructing the project page.


## Citation
If you find this project helpful for your research, please consider citing our paper and giving a ⭐.

Any questions or academic discussion, please contact me at: byzhao@mae.cuhk.edu.hk

```BibTex
@article{ZHAO2024105405,
title = {High-resolution infrastructure defect detection dataset sourced by unmanned systems and validated with deep learning},
journal = {Automation in Construction},
volume = {163},
pages = {105405},
year = {2024},
issn = {0926-5805},
doi = {https://doi.org/10.1016/j.autcon.2024.105405},
author = {Benyun Zhao and Xunkuai Zhou and Guidong Yang and Junjie Wen and Jihan Zhang and Jia Dou and Guang Li and Xi Chen and Ben M. Chen},
}
```

