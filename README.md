# Real-time Detection of Cavings in Shale Shaker

Some experiments I did when I worked in PRORES AS - not part of company project.

In this project, I implement paper by [Skea, 2018](https://www.sciencedirect.com/science/article/pii/S1674775517304006?via%3Dihub) that classified borehole failure mode based on cavings shape. Cavings are classified into Angular, Tabular, Blocky, and Splintery, and each shape correspond to different failure mode. 

I developed a real-time segmentation using YOLOv11 on a shaker video, calculated the shape of cavings, and produced real-time plot. The 10-second video is publicly accessed from YouTube. 

Here is the result of the detection:

[<img src="https://img.youtube.com/vi/<VIDEO_ID>/hqdefault.jpg" width="600" height="300"
/>](https://github.com/user-attachments/assets/cd2e20c7-5cd1-444d-b68d-111841b4abf5)

And here is the failure plot animation:

[<img src="https://img.youtube.com/vi/<VIDEO_ID>/hqdefault.jpg" width="600" height="300"
/>](https://github.com/user-attachments/assets/c6b9e7cd-dcdc-4b8e-b474-713985478907)

Here is the final plot of all detected cavings. You can see how cavings move from bedding to tensile failure over time. 

<img width="411" alt="image" src="https://github.com/user-attachments/assets/89112a8f-45b0-4993-acb8-f79245d75afc">

## Libraries

* Ultralytics==8.3.47
* OpenCV==4.10.0.84
* FFMPeg==0.2.0
