# canny_edge_my_face
Canny Edge Detector For ROS

This is a simple program that subscribes to camera images, apply a canny detector to it and publishes it to a particular 
topic of your choice. The result can be viewed in stand alone image windows using the opencv imshow function or can be viewed
in rqt by subscribing to the topic. The result with and without rqt are attached as png files.

Steps to run the program:
1. roslaunch usb_cam usb_cam-test.launch
2. rosun canny_edge_my_face canny_edge_node

This would open two windows one with the camera view and one with the canny edge detector as can be seen in the image 
result_without_rqt.png. You can also view the result in rqt and for that go to the terminal and type rqt and when the window
subscribe to the topic /edge_detector/raw_image. Open the image viewer in the rqt and it will show the edge detector result.
