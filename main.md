# Final Project

## Poor Man's Augmented Reality

I used a cardboard box and shot a quick 9 second video of it moving towards a different angle.

I labelled 24 points based on the grid I drew on the box. Using the CSRT Tracker from opencv, I initialized trackers for each point and then updated them over each frame in the video. In the end, the tracker was relatively successful and was able to able most of the points correctly.

Using the bottom-left point as the origin, I generated 3D coordinates for each marked point, then used these to generate the camera calibration matrix for each frame using least squares. 

Using the `draw` function from the OpenCV tutorial [here](https://docs.opencv.org/3.4/d7/d53/tutorial_py_pose.html), I then successfully rendered the cube to move with the changing angle in the video.

Unfortunately did not do any of the Bells & Whistles but I really enjoyed this project and class!