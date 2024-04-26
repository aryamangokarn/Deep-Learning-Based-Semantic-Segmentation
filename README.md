# Deep-Learning-Based-Semantic-Segmentation

## Paper Link: [https://ieeexplore.ieee.org/document/9973882](https://ieeexplore.ieee.org/document/10220818)

## Abstract

This research study presents a a novel approach for semantic segmentation of land cover using Bhuvan 2D satellite images. The proposed approach utilizes U-Net models for classification. The dataset consists of 2D satellite images covering a region in India. A pre-processing pipeline is applied to extract relevant features and generate ground-truth labels. The model is trained on the dataset, and the results demonstrate its effectiveness in accurately classifying different types of land cover, such as forest, water bodies, agriculture, roads and urban areas, using performance metrics such as Dice coefficient (F1-Score), and Intersection over Union (IoU). The model is made more accurate and robust through the implementation of data augmentation techniques. The proposed approach can have significant applications in environmental monitoring, disaster management, and urban planning, providing accurate and detailed information on land cover patterns and changes over time.

## Dataset

  **Study Area**- Varanasi, a city located in the north India in the state of  Uttar Pradesh, with coordinates ranging from 25.3-25.5° N, 83-83.2°E.

  **Programme** – Bhuvan Indian Geo Platform by Indian Space Research Organisation (ISRO)

  **Image** – Satellite/Sensor Image type. 

    - Created a satellite image dataset of the region of Varanasi.
    - A set of manually generated masks were created for each image in dataset. 
    - Performed data augmentation to increase the size of the dataset.

<p align="center">  
<img width="771" alt="Dataset Sample" src="https://github.com/aryamangokarn/Counterfeit-Currency-Detection/assets/88145926/989785a4-4233-40cb-85cd-4cd74be951fe">
</p>

## Result Analysis

Performance metrics of VGG16 and Resnet50 with U-Net Model for different epochs are listed in below table. The highest performance in terms of Dice coefficient is achieved by the Resnet50 model at epoch 5, while the VGG16 model achieves its highest performance at epoch 10, both with a score of 0.70. It can be observed that the Resnet50 model outperforms the VGG16 model with higher accuracy achieved at the 5th epoch, indicating more efficient training time. It is important to highlight that even though epoch 15 has a high pixel accuracy, it does not necessarily imply superior segmentation ability.

<p align="center">
<img width="520" alt="Results_1" src="https://github.com/aryamangokarn/Counterfeit-Currency-Detection/assets/88145926/713b8442-3774-4c0b-866b-632126e9fa2b">

The below table presents the performance metrics of VGG16 and Resnet50 with U-Net model for different land cover classes. Scores for the "Road" and "Urban" classes are comparatively lower than the scores for "Water," "Forest," and "Agriculture". This difference in scores can be attributed to the frequency of occurrence of each class in the dataset.

</p>

<p align="center">
 <img width="451" alt="Results_2" src="https://github.com/aryamangokarn/Counterfeit-Currency-Detection/assets/88145926/371b70b6-4e32-4cdf-8bb4-e2f074292e6e"> 
</p>

## Conclusion

In this paper, we have proposed an approach for land cover classification utilizing VGG16 and Resnet50 with U-Net architectures, leveraging Bhuvan 2D satellite images and manually created masks for accurate classification. Our modelsachieve a training accuracy of 96.63%, test accuracy of 90% with dice coefficient of 0.70. The findings of this study show-case the efficacy of the VGG16 and Resnet50 U-Net models in semantically segmenting satellite images, emphasizing the significance of developing precise and efficient algorithms for land cover classification. The models can produce high-resolution land cover maps that can be used for a wide range of applications, including environmental monitoring, urban planning, and natural resource management.
