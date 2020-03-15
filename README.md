# Bee Detection with yolov3
This repository contains the files and appropriate explanation on how to replicate our results for using darknet/yolov3 for detecting bees.

## Repository Contents

The repository is divided in two main folders, the configuration and the results. The configuration contains every file used for configuring the off-the-shelf darknet framework \[4\], including the weights generated after training. The results folder contains the output video of the bees detection.

## How we trained our model
First, we downloaded videos containing bees that were previously used for an analysis with motion detection \[1\]. Then, we used the YAT \[3\] tool for creating and storing labels out of the videos (see configuration/labels). With the labels in hand, we followed the tutorial \[2\] and configured our tiny-yolov3.cfg file (see configuration/cfg) the names file (see configuration/names) and the data file (configuration/data). And finally, cloned the darknet repository:
```
git clone xxx
```

To train the model, we executed the command:
```
yyy
```

The model was saved in a the model.pt file (see configuration/weights).

## How we detected the object

Once we had the trained model, detecting the bees in a video was straight forward. We just needed to execute the command:
```
zzz
```

Which saved a video (results/HT_Vid_detected.mp4) where the object detection is demonstrated.

## References
1. Kulyukin, Vladimir, and Sarbajit Mukherjee. "On Video Analysis of Omnidirectional Bee Traffic: Counting Bee Motions with Motion Detection and Image Classification." Applied Sciences 9.18 (2019): 3743.
2. [How to train YOLOv3 to detect custom objects](https://medium.com/@manivannan_data/how-to-train-yolov3-to-detect-custom-objects-ccbcafeb13d2), Accessed on 15/03 at 20:23.
3. [YAT - An open-source data annotation tool for YOLO](https://medium.com/@vinay.dec26/yat-an-open-source-data-annotation-tool-for-yolo-8bb75bce1767)
4. Insert here the github link for the darknet used.

## Authors
* Johan Karlsson
* Ricardo Caldas
* Teodor Fredriksson
* Yu Ge
