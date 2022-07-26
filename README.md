# BiNet: Bridge visual inspection dataset and approach for damage detection
Manual damage identification from large visual inspection data sources demands tremendous effort and is prone to discrepancies due to human errors, fatigue, and poor judgments of bridge inspectors. Deep learning techniques have obtained state-of-the-art results in solving computer vision tasks across different domains such as health, retail, among others. To encourage the development of automated visual inspection and damage detection solutions in the realm of infrastructure management, we propose BiNet, a visual inspection dataset for multi-label damage identification that can be used for classification, localisation, and object detection. We have investigated and compared the performance of convolutional neural networks and transfer learning approaches for automated damage classification and localisation. We have established baseline performance results of BiNet for future comparisons. Our contribution is introducing the public well-curated bridge visual inspection dataset and a deep learning approach for automated damage detection. This work is a step toward (semi) automated inspection of bridge structures for cost-effective, consistent and reliable bridge management.


### The overview of BiNet and train/test split 

| Classes | Number of images | Train split  | Test split |
| :---         |     :---:      |          :---: |   ---:|
| Cracks   | 1330     | 931     | 399 |
| Spalling     | 240       | 168      | 72 |
| Corrosion Stain | 961  | 673   | 288  | 
| Exposed bars | 942     | 659 | 283  |
| Total | 3588 | 2431 | 1042 | 



### Apporch - Damage detection using CNNs and transfer learning strategies 
We are proposing the utilisation of deep learning techniques, specifically convolutional neural networks (CNNs), to automatically detect and classify the damages from visual inspection datasets. CNNs are known to perform well with a large amount of data. However, with the manual labelling of domain-specific datasets, the labelled data is most scarce. Therefore, we follow the evaluation approach defined [our previour paper](https://link.springer.com/article/10.1007/s00521-021-06279-x) to compare multiple transfer learning strategies and CNN architectures for developing a robust predictive model. We mainly compare four different approaches as illustrated below:
Standard CNN with random initialisation for damage detection            |  VGG16 with random initialisation for damage detection
:-------------------------:|:-------------------------:
![](https://github.com/Zaharah/BiNet-bridge-visual-inspection-dataset/blob/main/ri.png)  |  ![](https://github.com/Zaharah/BiNet-bridge-visual-inspection-dataset/blob/main/ri_vgg.png) |

Pretrained VGG16 with ImageNet           |  Pretrained VGG16 with CODEBRIM dataset |
:-------------------------:|:-------------------------:
![](https://github.com/Zaharah/BiNet-bridge-visual-inspection-dataset/blob/main/imagenet_vgg.png)   |  ![](https://github.com/Zaharah/BiNet-bridge-visual-inspection-dataset/blob/main/codebrim_vgg.png) 
