# IS550_Final_Project


IS550 Big Data Management

Anthony Chung


## **Foot Traffic Tracker**

**Summary:**

This project aims to capture Foot traffic entering a certain space. There are three major steps:
1) Detecting if a object is passing through a certain area of the room and if it is, capture that instances and upload to dropbox 
2) Retrieve image and classify each image and output the number of faces detected for a head count 

3) Upload the result to Google sheets for logging

I was able to follow a tutorial that utilize a Raspberry Pi Camera and uploads occupy images to dropbox. Then I utilize opencv’s face detection classifier FrontalFace_default to classify the image and count how many people are captured in the image. Lastly I connected to my google sheet and upload the results.

This is a barely working model, but I was able to get all my pieces together. Right now my troubles are connecting to my dropbox to pull the images out on to my local drive. Images are retrieved locally. The predicting power of the classifier is weak. I plan to actually train a model that I can substitute with CascadeClassifier. I believe with a better train model on classifying the capture image, I will be able to get a good working Foot Traffic Tracker for my company.

**Methodology:**

Part 1: Capturing Motion on the Street

link: [Follow guide on pyimagesearch code](https://github.com/chungyta/IS550_Final_Project/tree/master/pi-home-surveillance)


Part 2: Classifying Images to get Head count

Part 3: Uploading to Google sheet to keep log

Part 4: Do it over certain time period
This step is plan to be implmented when model gets deploy. The idea is that every hour or so, the script should run to pull the lastest set of images and classify them 


There are a few steps I was not able to complete. 
