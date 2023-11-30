This is done to determine the intensity of the number of vehicles on that particular highway lane. My code uses general 'coco' weights, but we can custom train and use those weights.

The code exploits the feature of deep-sort multi-object tracking. Further application must be to check how many vehicles are entering that particular side and leaving, we can even classify amongst the vehicles and put up the counter. It will look something like this:
![image](https://github.com/katikkale15/vehicle_intensity_heatmap/assets/98995391/09c249e6-506b-4f31-a7fd-1ae9ba4edf17)

To implement this, there has to be a code block added to the heatmaps file that we have used in out notebook. The updated code is in this [drive link](https://drive.google.com/uc?id=1eA1UzQby0yLb6fc3Dy9cX7aqH0JdCcO-&confirm=t). Then the codeblock would be:
```
!gdown "https://drive.google.com/uc?id=1eA1UzQby0yLb6fc3Dy9cX7aqH0JdCcO-&confirm=t"
```
Since the name of the file is the same, to run it with a demo video:
```
!python heatmaps.py --weights yolov7.pt  --img 640  --source test1.mp4  
```
This will replicate the image exactly.
