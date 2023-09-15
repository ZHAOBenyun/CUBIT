<h1 style="text-align: center; font-size: 36px; font-family: 'Sama Devanagari';"> CUBIT: A High-resolution Infrastructure Defect Dataset Fully Evaluated with Autonomous Detection Framework
    <div style="text-align: center; font-size: 20px; font-family: 'Sama Devanagari';">    Submitted to International Conference on Acoustics, Speech, & Signal Processing 2024
</div>
</h1>

<div style=" text-align: center; font-size: 17px;">
Benyun Zhao<sup>1</sup>, Xunkuai Zhou<sup>2</sup>, Guidong Yang<sup>1</sup>, Junjie Wen<sup>1</sup>, Jihan Zhang<sup>1</sup>,  Xi Chen<sup>1</sup>, and <a href="http://www.mae.cuhk.edu.hk/~bmchen/">Ben M. Chen</a><sup>1</sup>, Fellow, IEEE
</div>
<br>
<div  style="text-align: center; font-size: 17px;" >
1.Department of Mechanical and Automation Engineering, The Chinese University of Hong Kong <\br>
    2.School of Electronics and Information Engineering,Tongji University

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

## The Comparison between Existing Bounding-box-level Defect Dataset with CUBIT

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
<h3>Prediction results on the test set of the proposed CUBIT-RGB-v1 defect dataset are shown below
</h3>
</div>

## Experimental Results
The evaluation results of SOTA real-time detection methods and YOLOv6-n with our GIPFPP module are benchmarked in the table below. After switching from the original module to GIPFPP module, the AP of YOLOv6-n is improved by 3%, while its number of parameters is reduced by 10%. The enhancements made to the model will facilitate the real-time defect detection using unmanned systems.

## The Evaluation Results of SOTA models on CUBIT

| Model                       | #Params.(M) | FLOPs(G) | Size | mAP$_{50}^{test}$ / mAP$_{50:95}^{test}$ | Latency(ms) |
|-----------------------------|-------------|----------|------|-----------------------------------------|--------------|
| Faster R-CNN(Res50)         | 42.62       | 477.24   | 1024 | 71.5% / 43.3%                           | 76.9         |
| PP-YOLO                     | 48.99       | 136.43   | 1024 | 76.4% / 45.1%                           | 14.5         |
| PP-YOLOv2                   | 56.91       | 146.50   | 1024 | 77.3% / 47.1%                           | 13.8         |
| YOLOv5-n                    | 1.76        | 4.10     | 1024 | 73.4% / 39.9%                           | 1.8          |
| YOLOv5-s                    | 7.18        | 15.80    | 1024 | 78.5% / 47.2%                           | 3.3          |
| YOLOv7-t                    | 6.01        | 13.01    | 1024 | 71.1% / 39.7%                           | 1.9          |
| YOLOX-n                     | 2.24        | 17.75    | 1024 | 73.0% / 39.5%                           | 4.4          |
| YOLOX-t                     | 5.03        | 39.00    | 1024 | 75.3% / 49.2%                           | 5.8          |
| YOLOX-s                     | 8.94        | 68.51    | 1024 | 77.9% / 49.4%                           | 7.6          |
| YOLOv6-n(baseline)          | 4.63        | 29.03    | 1024 | 76.3% / 47.9%                           | 2.2          |
| YOLOv6-s                    | 18.50       | 115.64   | 1024 | 79.0% / 48.2%                           | 5.3          |
| **YOLOv6-n+GIFPFF(ours)**   | **4.14 (-0.49)** | **28.02 (-1.01)** | 1024 | **77.5% (+1.2) / 50.3% (+3.1)**       | **2.2**      |



We enlarge the prediction results in the bottom right corner of framework images above. CUBIT dataset covers three infrastructure types: **Building facade, Pavement**, and **Bridge**, and aims for three types of defect: **Crack, Spalling, and Moisture**. Rectangles indicate the output prediction box (\textcolor{red}{Red} for \textbf{Crack}, \textcolor{pink}{Pink} for \textbf{Spalling}, and \textcolor{orange}{Orange} for \textbf{Moisture}) with inferred defect type and confidence score from YOLOv6-l trained on the training set of our proposed dataset.
<p align="center">
  <img src="./index_show.png">
</p>

*Qualitative visualization of UAV-based real-world experiment is shown below* On the left, our multi-UAVs inspection schematics is illustrated. On the right, the detection results of four direction façades of the building are displayed.
<p align="center">
  <img src="./goodman_zigzag.png">
</p>


