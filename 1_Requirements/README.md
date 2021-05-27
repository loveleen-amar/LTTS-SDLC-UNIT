# Requirements :clipboard:

## :pushpin: Introduction
Requirement analysis is the most important and fundamental stage in SDLC. The following are the set of requirements for the Object detection API:-
### :heavy_check_mark: *Functional Requirements*
1) **System Interface Requirement**

   **i) User Interfaces**
        API can be used for many applications. One of the applications of this API is an android app which
        sends an image from phone gallery to the server via API call and receives an image with all the
        objects detected.

     **1. Install the android app and select image from gallery.** 
      
     <img src="https://github.com/loveleen-amar/LTTS-SDLC-UNIT/blob/main/1_Requirements/1.JPG" width="400">  



     **2. Select a photo from the gallery.**
     
     <img src="https://github.com/loveleen-amar/LTTS-SDLC-UNIT/blob/main/1_Requirements/2.JPG" width="400">  
     
     
     
     
     **3. Send and wait for the response image.**
     
     <img src="https://github.com/loveleen-amar/LTTS-SDLC-UNIT/blob/main/1_Requirements/3.JPG" width="400">
     

  **ii) Hardware Interfaces**
  * Any machine with Network Interface Card and Ethernet drivers to connect to the internet.
  
  * Programmable devices to send the image to API dynamically.
  
  * Devices able to process graphical matrix(image) eg. Raspberry Pi, Arduino etc.
        
  **iii) Software Interfaces**
        This API requires internet drivers at client-side and any programming language which supports
        network programming. However, the application of this API can have vivid requirements. For
        example, the android app requires Android OS, access to camera and gallery & access to use the
        internet.
        
  **iv) Communications Interfaces**
        Internet connection is required for frequent upload and download of image stream bytes to/from the
        server. Every request requires the client to be connected to the internet to make an API call.


2) **Legal or Regulatory Requirements**

    * **Sending data:**
        A valid image file should be sent to the server at a sufficient interval depending on the
        image size. Invalid images or any other file types will be discarded.
        
    * **Invalid Image File :**
        In case of invalid image file, the server will respond with an error message stating
        “Invalid Image Type”.
### :heavy_check_mark: *Non-Functional Requirements*
1) **Security Requirements**
There is no privacy issue as the images sent to the server are not stored anywhere in the database. Also, the API requires data to be sent over https connection thus it is secured from man-in-the-middle attack. However, other applications of this API could pose security threats which the API is not responsible for.



## :pushpin: Research
* Early works on object detection were based on template matching techniques and simple part-based models [e.g., Fischler and Elschlager (1973)] 

* Later, methods based on statistical classifiers (e.g., Neural Networks, SVM, Adaboost, Bayes, etc.) were introduced [e.g., Osuna et al. (1997), Rowley et al. (1998), Sung and Poggio (1998), Schneiderman and Kanade (2000), Yang et al. (2000a,b)]

* This initial successful family of object detectors, all of them based on statistical classifiers, set the ground for most of the following research in terms of training and evaluation procedures and classification techniques.

* Since applying all these algorithms for the task of object detection is not possible for everyone, as all users cannot have that high-end systems.
 
* Hence, this API is made to leverage the power of ML/DL for Object detection task for common people too, who can directly use the API and have results out of it without having any high-end system.

## :pushpin: Cost and Features
### :heavy_check_mark: *Cost*
Since the system uses only open source software, it is free of cost :+1:

*TBD*

### :heavy_check_mark: *Features*
The folowing are the features of this API:

  **1 Description and Priority**

  The main task of the API is to detect the objects present in the image and plot the boundary
  box around them. When a client sends any image to the server via the API, the server calls
  YOLO algorithm on the image to detect objects. It plots the boundary boxes and then revert
  back the new image with detected objects to the client.
  
  >> **Priority: High**

  **2 Stimulus/Response Sequences**
  
     1. Client send an image to the API.

     2. API, after authenticating the validity of image, sends it to server.

     3. Returns the new image to the client.


## :pushpin: Defining the System 
### :heavy_check_mark: *Product Perspective*

Currently, most of the Object detection softwares do all the computations on the devices they’re
installed on which can be slow due to low hardware specifications. The product proposed in this
document overcomes this problem by doing all the computation at the server side and in return
provides the image with objects detected in only a few cycles of CPU.

<img src="https://github.com/loveleen-amar/LTTS-SDLC-UNIT/blob/main/1_Requirements/4.JPG" width="800"> 

### :heavy_check_mark: *Product Functions*
  * API accepts image of any extension and detects objects present in it.
  * After detecting API, it returns the image with object detected in PNG format.
  * All the computations are done at the server end.
  * YOLO v3.0 algorithm is used for the Object Detection Task.

## :pushpin: SWOT ANALYSIS
![SWOT-Analysis](https://github.com/Sanchana-2k/LTTS_C_MiniProject/blob/6f6972167470b4b186e9995b7a6647f3f8c7cbd5/1_Requirements/swot%20analysis.jpg)




# :pushpin: 4W&#39;s and 1&#39;H 	

## :heavy_check_mark: Who:

The API has the following levels of users described below:-

* **LEVEL 1 user:**
A first type of user of the API is a software developer who are building up big projects in which a
part is of object detection , so the can integrate and object detection part using this. They should
have the following technical skills:-
  1. Generally has the skills and experience to design, construct, test, and maintain the software
  systems;
  2. Understands processes and procedures to compile, link and load software for embedded
  systems;
  3. Is proficient at writing software in the python language

* **LEVEL 2 user:**
The second type of users for this API is a students who required not to do heavy backend work and
can simply use this API by accessing it through URL.


* **LEVEL 3 user:**
The third type of users for this API are typical internet users who only need to upload an image and
wait for the results.



## :heavy_check_mark: What:

This object detection API take in image as input and return an image with all the objects detected in it by just hitting a url.

## :heavy_check_mark: When:

When a particular student/developer wants to do object detection task in his/her big projects so he can easily use this api and integrate it in his project. 


## :heavy_check_mark: Where:

It can be used at places where research work projects are going on, or just if a typical internet user wants to get all the objects out of an image wihout having any high-end system.

## :heavy_check_mark: How:

Simple the user send an image to the API. Then the API, after authenticating the validity of image, sends it to server where the object detection task happens using DL model. Then the API returns the object detected image to the user.

# :pushpin: Detail requirements
## :heavy_check_mark: High Level Requirements:

|      ID          |Description                          |Status                         |
|----------------|-------------------------------|-----------------------------|
|HR_01|Length |Implemented|
|HR_02|Area |Implemented|
|HR_03|Volume|Implemented|
|HR_04|Mass |Implemented|
|HR_05|Speed |Implemented|
|HR_06|Time|Future|
|HR_07|Temperature|Future|



## :heavy_check_mark: Low level Requirements:
|      ID          |Description                          |  HLR_ID  |Status               |
|----------------|-------------------------------|----------|-----------------------------|
|LR_01|Meter|HR_01|Implemented|
|LR_02|Centimeter|HR_01|Implemented|
|LR_03|Foot|HR_01|Implemented|
|LR_04|Inch|HR_01|Implemented|
|LR_05|Millimeter|HR_01|Implemented|
|LR_06|Square Meter|HR_02|Implemented|
|LR_07|Square Centimeter|HR_02|Implemented|
|LR_08|Square Foot|HR_02|Implemented|
|LR_09|MSquare Inch|HR_02|Implemented|
|LR_10|Square Yard|HR_02|Implemented|
|LR_11|Cubic Meter|HR_03|Implemented|
|LR_12|Cubic Centimeter|HR_03|Implemented|
|LR_13|Litre|HR_03|Implemented|
|LR_14|Millilitre|HR_03|Implemented|
|LR_15|Gallon (imperial)|HR_03|Implemented|
|LR_16|Kilogram|HR_04|Implemented|
|LR_17|Gram|HR_04|Implemented|
|LR_18|Ounce|HR_04|Implemented|
|LR_19|Tonne (metric)|HR_04|Implemented|
|LR_20|Pound|HR_04|Implemented|
|LR_21|Meter per Second|HR_05|Implemented|
|LR_22|Kilometer per Hour|HR_05|Implemented|
|LR_23|Miles per Hour|HR_05|Implemented|
|LR_24|Foot per Second|HR_05|Implemented|
|LR_25|Knot|HR_05|Implemented|
|LR_26|Hour|HR_06|Future|
|LR_27|Minute|HR_06|Future|
|LR_28|Second|HR_06|Future|
|LR_29|Celcius|HR_07|Future|
|LR_30|Farenheit|HR_07|Future|
|LR_31|Kelvin|HR_07|Future|
