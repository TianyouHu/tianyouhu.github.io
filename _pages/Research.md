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

Please check these 2 videos for comparison.
[gmapping doesn't know where it is.webm](https://user-images.githubusercontent.com/71891452/223967531-422d316b-fa48-4b53-9962-19c2dc2c1ff9.webm)<br />
[Karto knows it is stuck by rod.webm](https://user-images.githubusercontent.com/71891452/223967493-efaf9b33-272e-4548-944c-458d2825d1d1.webm)

Computer Vision and Machine Learning with Self-driving Car project
======




