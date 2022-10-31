# Fall-Detection-Using-Pose-estimation-
An accurate fall detection model that uses pose estimation to detect falls and count people in real time


¬First step would be to download the pre-trained pose estimation model which would be run through Tensorflow(graph_opt.pb). This model basically graphs and points out the body parts which are already defined in the model, for example the nose is the first point, then the eyes etc. This model helps us to draw the basic human pose estimation structure and helps us to go further explore other areas.


Once the pose estimation read the humans body, we can further test it out on several videos and live webcam. Now that all those things are working fine, we can use the human mapping to count the number of people on the screen. To do that we just set up a counter and keep increasing or decreasing it if the number of people on the screen change. The console too will show you the number of people increased or decreased if we need to check at what point how many people were there in the frame.


Now to detect the falling humans, we used the y coordinate of the head to detect a fall. Coordinates of the head in normalised form. Depending on the picture size, we transform normalised points to relative points. y1.append(y) will save the y coordinate for comparison with the preceding point. We utilised try and except because pose estimators frequently fail to anticipate head point.

![image](https://user-images.githubusercontent.com/83086871/199013266-19968a2b-67a4-45d5-b4d7-e2ceff5d2d95.png)


The final result of this project is really fascinating, as itshows the number of people in the frame along with body tracking with great accuracy just by using a basic webcam or just by applying the program to any video locally.

![image](https://user-images.githubusercontent.com/83086871/199013517-2c4d3079-5af4-422d-8746-fd343e34b440.png)
![image](https://user-images.githubusercontent.com/83086871/199013558-163dd3ff-20ae-465a-9d7e-e8f61ebdff17.png)


![image](https://user-images.githubusercontent.com/83086871/199013675-b3fd48d8-de4d-4485-b557-525b374c634e.png)


![image](https://user-images.githubusercontent.com/83086871/199013686-abc12e59-84c4-4930-b51e-ffcc01b4c605.png)
