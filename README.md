# Biwi-Kinect-Head-Pose_Point-Detection

### Overview
 Dataset [Biwi Kinect Head Pose Database](https://icu.ee.ethz.ch/research/datsets.html) contains images of 20 people (6 females and 14 males - 4 people were recorded twice). For each frame, a depth image, the corresponding rgb image (both 640x480 pixels), and the annotation is provided. The head pose range covers about +-75 degrees yaw and +-60 degrees pitch. Ground truth is provided in the form of the 3D location of the head and its rotation.




### Implementation details
| Feature | Brief Explanation |
| ------ | ------ |
| Base Model Architecture | Resnet18 from [ResNet](https://arxiv.org/abs/1512.03385) family, implemetation from [PyTorch](https://pytorch.org/)|
| Learning Rate Finder | [Learning rate finder](https://arxiv.org/abs/1506.01186) implemetation from [FastAI](https://www.fast.ai/) |
| Learning rate and  Momentum scheduler| [One cycle policy](https://arxiv.org/abs/1803.09820) implemetation from [FastAI](https://www.fast.ai/)  to achieve superconvergence |
| Dataset |  Dataset [Biwi Kinect Head Pose Database](https://icu.ee.ethz.ch/research/datsets.html) from [ETH Zurich](https://icu.ee.ethz.ch/the-group.html) |


### Results
| Model | Metrics(Validation Loss) | Epochs |
| ------ | ------ | ------ |
| Resnet18 | 0.000186 	 | 8 |


#### Inference
![Alt text](https://github.com/gurucharanmk/Biwi-Kinect-Head-Pose_Point-Detection/blob/main/images/results.png  )

## License
This project is licensed under the [MIT License](https://github.com/gurucharanmk/Biwi-Kinect-Head-Pose_Point-Detection/blob/main/LICENSE)
