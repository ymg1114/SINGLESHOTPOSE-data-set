# SINGLESHOTPOSE dataset for food dataset
Food data for 6D pose estimation algorithm (especailly for SingleShotPose)
SingleShotPose: https://github.com/microsoft/singleshotpose

The dataset is composed of `ace`, `diget`, `diget_sand`, `gotica`, `small_spam`, `spam`, and `tomato_soup`.

data link: https://koreaoffice-my.sharepoint.com/:f:/g/personal/jhj0630_korea_edu/Emnjiedw6XNKsJlXlu_xZjABi-gfIaUCw7sq4sn5cdFSzw?e=5zvFsP

# Collection method

The dataset is collected using markers. First, we collected the pose of object in a image with respect to 16 kinds of markers like below image.

![data collection](https://user-images.githubusercontent.com/24308201/142810967-dc5ed41c-be7c-4bc2-823a-92a12f964407.gif)

Then, we can know the pose of object if a marker exists in the image. For this method, the CAD file of the object is necessary to match the origin of the object.
The 'inspection_test' files show whether the pose of object is correctly estimated, so you can confirm the correctness of the labels.

* * *
# Description of the dataset
## Structure
```
singleshotpose
--mask
--labels
--inspection
--depth
--ply
```

## Labels
This dataset has same style of label with SingleShotPose. Therefore, you can refer it. [https://github.com/microsoft/singleshotpose]

This labeling style have the center of object and the width & height of object, you can utilize it for object detection such as YOLO.
This dataset also have masks of objects, it can be used for instance segmentation such as Mask RCNN.


## Files
```
JPEGImages : Input RGB image
mask : Mask image
labels : Target label
inspection : Input 3D bounding box
depth : Depth image
food_type.ply : CAD model
```
* * *

## Items
### `ace`
<img src="https://user-images.githubusercontent.com/54105796/67358408-39cd4280-f59b-11e9-9ad6-520f90ce369b.jpg" width="30%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>

### `diget`
<img src="https://user-images.githubusercontent.com/54105796/67358632-06d77e80-f59c-11e9-9ee9-5625c3a7572c.jpg" width="30%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>

### `diget_sand`
<img src="https://user-images.githubusercontent.com/54105796/67358729-3f775800-f59c-11e9-8612-61364abbabc5.jpg" width="30%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>

### `gotica`
<img src="https://user-images.githubusercontent.com/54105796/67358791-6df53300-f59c-11e9-9cd3-1846f44bdc6b.jpg" width="30%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>

### `small_spam`
<img src="https://user-images.githubusercontent.com/54105796/67358844-911fe280-f59c-11e9-9b46-268ceb9463ec.jpg" width="30%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>

### `spam`
<img src="https://user-images.githubusercontent.com/54105796/67358865-a7c63980-f59c-11e9-94e7-187c0669e3d0.jpg" width="30%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>

### `tomato_soup`
<img src="https://user-images.githubusercontent.com/54105796/67358917-ccbaac80-f59c-11e9-8790-a1325bb4669f.jpg" width="30%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
