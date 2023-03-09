---
layout: archive
title: ""
permalink: /research/
author_profile: true
---
Vision Based Exploration in Fully Unknown Environment
=======
I worked in Professor [Yiannis Kantaros'](https://engineering.wustl.edu/faculty/Yiannis-Kantaros.html) lab at WashU since August 2022. I applied autonomous exploration algorithm on our Turtlebot3 Waffle Pi robot by combining RRT naviation algorithm and Karto SLAM method. Besides this, I applied YOLOv7 on our robot for object detection and depth estimation to obtain distance of specific object. My current work is combing laserscan and YOLO info to obtain position of pedestrian. The next step is predicting pedestrians trajectory based on their behavior.

Please check these demo videos. 

Object detection and autonomous navigation on pad (kinda bumpy)
<iframe width="560" height="315" src="https://www.youtube.com/embed/ixDVWG9pUJ4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

not on pad
<iframe width="560" height="315" src="https://www.youtube.com/embed/ICd1tCqf2rU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

depth estimation
<iframe width="560" height="315" src="https://www.youtube.com/embed/qh8bAIE5-mA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

test environment of depth estimation
<iframe width="560" height="315" src="https://www.youtube.com/embed/OoZ20Jg31_E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

The reason that I use Karto instead of Gmapping SLAM method is, Gmapping works pretty well in Gazebo but works bad on our Turtlebot. It somestimes messes the map up when twisting. When Turtlebot is stuck by something, Karto is able to know that robot is stuck, while gmapping method makes robot think it is still moving. When using gmapping SLAM, Turtlebot moves much faster than Karto SLAM.

Please check these 2 videos for comparison.<br />
[gmapping doesn't know where it is.webm](https://user-images.githubusercontent.com/71891452/223967531-422d316b-fa48-4b53-9962-19c2dc2c1ff9.webm)<br />
[Karto knows it is stuck by rod.webm](https://user-images.githubusercontent.com/71891452/223967493-efaf9b33-272e-4548-944c-458d2825d1d1.webm)

Computer Vision and Machine Learning with Self-driving Car project
======
I worked on this project from Aug 2019 to Nov 2020. I wrote my code of semantic segmantation for pixel-wise classification. The classification accuracy is increased from 34% to 87% on a small dataset by tuning upsample method and kernel size of CNN. The small dataset only contains 101 test 367 train images with their annotation images. The research is published in this [paper](https://tianyouhu.github.io/files/publication1.pdf).

The figure below shows comparison of input image, ground truth and segmentation outcome from different models. 
![fcns](https://user-images.githubusercontent.com/71891452/223976395-2404956a-4e4e-4d95-be64-5ff47cd8382b.png)

FCN-8s has the highest accuracy and mean Intersection over Union metric.
![fcns sheet](https://user-images.githubusercontent.com/71891452/223977059-32441257-9ecc-4ea7-858d-20876facb5e7.png)
<img src="https://user-images.githubusercontent.com/71891452/223977059-32441257-9ecc-4ea7-858d-20876facb5e7.png" alt="Image" height="202" width="509">

Code here. <iframe src="https://ghbtns.com/github-btn.html?user=TianyouHu&repo=models-in-paper&type=star&count=true&size=large" frameborder="0" scrolling="0" width="170" height="30" title="GitHub"></iframe>




