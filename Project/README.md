# Car-license-plate-detection-

<b>Ability to manually adjust the artificial neural network </b>








# plate detection
The first step in resolving plaque detection problems is to identify the plaque. In the first phase of LPR, a limiting box is produced that fits exactly where the license plate is located. This is the main condition for successful LPR. Therefore, LP diagnosis should be relatively accurate. In this article, we have used the opencv library as well as contour and edge finder to detect this bug.






# Segmentation
With the arrival of the new license plate image, various filters are first applied to the image and the main location of the license plate is identified using the contour. At this stage, more image processing libraries have been used.
Finally, using conditions such as the height of the numbers or the width of the main location of the license plate numbers, the numbers are separated and entered into the constructed model. Our nerves will be given in the third stage.





# Character recognition (ocr)
At this stage, with the CNN neural network, as well as various filters and activity functions suitable for this network, along with determining the correct values for the hyperparameters, the characters identified in the previous stage will be classified.



