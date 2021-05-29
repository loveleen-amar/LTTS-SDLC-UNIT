# Object-Detection-API

This project introduces an API for object detection. The server will do all the heavy work for the client even if client has low-end system. This API can be used by anyone for the object detection task freely. 
An image by the client will be sent to the API end-point in specific format and then API would do the object detection task and send back the object detected image. The received image will be obtained by the client with objects classified within that image. YOLO v3.0 is used as the object detection model.

## Folder Structure
Folder             | Description
-------------------| -----------------------------------------
`1_Requirements`   | Documents detailing requirements and research
`2_Design`         | Documents specifying design details
`3_Implementation` | All code and documentation
`4_Test_plan`      | Documents with test plans and procedures
`5_Report`                | Report attached
`6_Imagesand Videos`      | Images out the results
`7_Others`                | other addons


## Setup Instructions

* Clone this repository `git clone https://github.com/loveleen-amar/Object-Detection-API.git`
* `cd Object-Detection-API`  will get you into root folder of the project.
* `cd API-Backend_Django` will get you into the Django Project Folder.
* Install all the python3 dependencies by `pip3 install -r requirements.txt`
* Download [yolov3.weights](https://pjreddie.com/media/files/yolov3.weights)
* Place *yolov3.weights* in `/API-Backend_Django/YOLOv3` directory. 
* Now start the Django Server: `python3 manage.py runserver 0.0.0.0:80` . It will start the server at port 80 so that it can be accessed just by the IP address.
* There is very basic Interface too for confirming the working of the API. After starting the server, goto `http://localhost:PORT` which in this case is 80. Thus, access the server simply by `http://locahost`.

## Example

After uploading photos, we get images with boundary boxes detected around it. For examples
<img src="https://github.com/loveleen-amar/LTTS-SDLC-UNIT/blob/main/output.JPG" width="500">



## Built With
* [Django](https://www.djangoproject.com/) - Python Based Web Framework
* [PyTorch](https://pytorch.org/) - A Deep Learning Framework
* [YOLO v3.0](https://pjreddie.com/yolo/) - Object Detection Algorithm
* [Android Studio](https://developer.android.com/studio) - Android Development IDE
* [Retrofit](https://github.com/square/retrofit) - Android Java Library for easy HTTP requests management


## To-Do
* [X] Add Android Application
* [X] Update README for the Android App.
* [ ] Host the API on Heroku.

## Authors
* **Loveleen Amar** [LinkedIn](https://www.linkedin.com/in/loveleen-amar/) | [GitHub](https://github.com/loveleen-amar)



## Learning Resources
1. [markdownCheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
2. [markdownBasics](https://guides.github.com/features/mastering-markdown/)
3. [git inspector](https://github.com/ejwa/gitinspector.git)
4. [github workflow](https://docs.github.com/en/actions/learn-github-action)

## Credits

1. Reference requirements and architecture and test plan - [Manjari_AP](https://github.com/256152/Mini_Project_1_April_2021.git)
2. Reference for High Level Requirements and Low Level Requirements Table - [arc-arnob](https://github.com/arc-arnob/LnT_Mini_Project.git)
3. Reference for the work- the main repo is [here](https://github.com/loveleen-amar/Object-Detection-API)

