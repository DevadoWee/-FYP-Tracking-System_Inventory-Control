# FYP-Tracking-System_Inventory-Control
Tools used - 1.Yolov7  2.Flutter  3.Firebase

# If for some reason you came to my page looking to do your FYP...
1. IMO, Please don't even try Yolov3 if accuracy is necessary for your project.
2. Sure Yolov7 will be hard to run live on your computer but starting it off as a video is not bad at all.

# Main point
The system uses the results provided by Yolov7 such as...
1. Coordinates of the detected objects.
2. Class name of the detected objects.
3. Track id of the detect objects.

By using these three attributes, the system detects the movement of an object, links it to the person taking the object and updates all of these including the personnel's credentials when he/her taps their name tag onto a sensor.

# Points to note
1. The mobile application serves nothing but to show the end result made by the system (firebase update).
2. The coordinates(xyxy) of the detected objects vary by a small margin even if the both the footage and the object is stationary.
3. Yolov7 is not flawless. You should take note of minor errors whenever it detects something wrongly and come up with a measure for it.
4. Despite how simplified the summary of the result manipulation is, it is important to take note that video footages are but frames bound together. With that, reassurance steps must be made to ensure only correct information is retained.
5. Creating a custom yolo weight is advised. Had a scissors be identified as a person because I was using a pre-trained weight.
