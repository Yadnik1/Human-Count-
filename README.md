# Human-Count++(People's Counter) 

Deploy a People Counter App at the Edge

What it Does
The people counter application is a smart video IoT solution using Intel® hardware and software tools. The app will detect people in a designated area, providing the number of people in the frame, average duration of people in frame, and total count. The app will also save a copy of the streamed output to the local storage device. The people counter app includes a built-in alarm that sends an alert the user on the GUI of the app when there are more than 5 people in the video.The people counter application is a smart video IoT solution using Intel® hardware and software tools. The app will detect people in a designated area, providing the number of people in the frame, average duration of people in frame, and total count. The app will also save a copy of the streamed output to the local storage device. The people counter app includes a built-in alarm that sends an alert the user on the GUI of the app when there are more than 5 people in the video.

How it Works

The counter will use the Inference Engine included in the Intel® Distribution of OpenVINO™ Toolkit. The model will identify people in a video frame. The app will count the number of people in the current frame, the duration that a person is in the frame (time elapsed between entering and exiting a frame) and the total count of people since the start of the video playback till the video ends or is interupted. It then sends the data to a local web server using the Paho MQTT Python package. The app also saves a copy of the streamed output to the local storage device. Thus a minimum of 150MB is recommended for smooth running of the app.
The app can take in a video of the following file formats: .mp4, .webm, .mpg, .mp2, .mpeg, .mpe, .mpv, .ogg, .m4p, .m4v, .avi, .wmv, .mov, .qt, .flv, .swf, and .avchd
It also works with images of these formats as input: .jpg, .bmp, .dpx, .png, .gif, .webp, .tiff, .psd, .raw, .heif, and .indd

What model was used
Model Used is the tensorflow model SSD Mobilenet v2 coco 2018. You can download the model direcly from the tensorflow model zoo by using this link.

The Intermediate Representation (IR) of the model can be downloaded by using this link.

Hardware
6th to 10th generation Intel® Core™ processor with Iris® Pro graphics or Intel® HD Graphics.
OR use of Intel® Neural Compute Stick 2 (NCS2)

Software
Intel® Distribution of OpenVINO™ toolkit 2019 R3 release
Node v6.17.1
Npm v3.10.10
CMake
MQTT Mosca server



