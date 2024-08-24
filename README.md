# ASL Sign Language Translation
This git repository contains all the files for hand gesture classification model, hand landmark calculation, ASL dataset parser and the app.py file.

###  Hand Gesture Classification Model
- A simple CNN which takes hand landmarks as a 1-Dimensional input and predicts classes based on the localized hand landmarks. 

### Hand Landmark Calculation
- Leveraged Google Media Pipe to extract frames from a camera feed and perform Google's hand recognition and hand landmark extraction. 
- Implemented a logger function which lets the user feed more gestures into the keypoints.csv file and retrain the model.
- The final outcome is a keypoints.csv file which includes labels and hand landmark (x,y) coordinates in a 1D array. 

### ASL Dataset Parser
- The ASL Dataset consists of hand images in ASL language. The parser file converts the image by running Google's Hand Detection and Hand Landmark Extraction and stores in a keypoints_ASL_data.csv. 
- This csv can be combined with keypoints.csv to generate a dataset of 35 labels. 0-9 being custom hand gestures and 10-35 being the ASL alphabets. 

## Further work
- Further work includes extending the custom hand gestures and adding more labels. 
- Implementation of point history to take sequential data for dynamic gestures with single finger.



