# Car-license-plate-detection-

# plate detection
**The first step** 
------
Based on the project requirements, we initially trained the model using a dataset of car images obtained from the Kaggle website, applying the YOLO algorithm to accurately detect each car's license plate.

A key step in this process involves converting the file format (from XML, containing coordinates of two points on the bounding rectangle around each license plate and the class of each object) to TXT format. The main point in this conversion is transforming the coordinates to obtain the center coordinates of the rectangle, along with its width, height, and the class types present in the image. In this stage, there is only one class, as we are focused solely on license plate detection.

After downloading the dataset and converting the labeling format of the images, we proceed to train the model using the YOLO algorithm.

Another important point in using the YOLO network is creating a file with a YAML extension, in which the dataset image paths and the classes to be mapped in the network should be specified.

Once the model is trained, the resulting weights from the model are saved, and we evaluate the model using test images from the dataset. It can be observed that the bounding rectangles accurately identify the license plates in the images.

The stored weights will later be used for the final license plate detection and, for convenience, will be transferred to Google Drive.

![Plate detection with YOLO](./car1.png)




# Segmentation
With the arrival of the new license plate image, various filters are first applied to the image and the main location of the license plate is identified using the contour. At this stage, more image processing libraries have been used.
Finally, using conditions such as the height of the numbers or the width of the main location of the license plate numbers, the numbers are separated and entered into the constructed model. Our nerves will be given in the third stage.





# Character recognition (ocr)
At this stage, with the CNN neural network, as well as various filters and activity functions suitable for this network, along with determining the correct values for the hyperparameters, the characters identified in the previous stage will be classified.



