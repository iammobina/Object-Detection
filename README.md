# Object Detection - Yolo Algorithm

"You Only Look Once" (YOLO) performs object detection, and then applies it to car detection. 
##### YOLO is computationally expensive to train, so pre-trained weights should be loaded.

#### Inputs and outputs
* The input is a batch of images, and each image has the shape (m, 608, 608, 3)
* The output is a list of bounding boxes along with the recognized classes.
Each bounding box is represented by 6 numbers  (pc,
b<sub>x</sub> ,b<sub>y</sub>,b<sub>h</sub>,b<sub>w</sub>,c).

#### Anchor Boxes
* Anchor boxes are chosen by exploring the training data to choose reasonable height/width ratios that represent the different classes.
* The dimension for anchor boxes is the second to last dimension in the encoding:  (m,n<sub>H</sub>,n<sub>W</sub>,anchors,classes) .

## Language
The code is written in python(keras).

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
