# Gastrointestinal (GI) Tract Video Classifier
## Dataset
[hyperKvasir](https://datasets.simula.no/hyper-kvasir/) <br>
* It contains 314 lower GI videos and 60 upper GI videos. <be>
* Videos have two types of resolutions - 1280 × 1024 and 720 × 576 <be>

## Preprocessing
* Frames are resized to 224 × 224 <be>

## Model Architecture
This model is implemented on top of [TF-3DCNN](https://www.tensorflow.org/tutorials/video/video_classification). <br>
![image](https://github.com/mrinal054/gastrointestinal-video-classifier/assets/44781227/c4598acf-a6f6-4cea-a70d-9dcf90dcbb0f)


## Training
- Data split <br>
    &check; Randomly picked 60 videos from each GI <br>
    &check; Split: training : validation : test -> 70 : 15 : 15 <br>
    &check; Total training data: 84 <br>
- Total validation data: 18 <br>
- Total test data: 18 <br>
- Loss function: Sparse Categorical Cross-Entropy <br>
- Optimizer: Adam <br>
- Batch size: 2 <br>
- Epoch: 50 <br>

## Results
- Result <br>
    &check; Experimented 50 times. <br>
    &check; Each time training, validation, and test data are picked randomly. <br>
 
| No. of incorrect | Without P-scSE3D | With P-scSE3D |
| :---: | :---: |  :---: |
| 0 | 3 |  12 |
| 1 | 17 |  14 |
| 2 | 13 |  16 |
| 3 | 9 |  8 |
| 4 | 5 |  0 |
| 5 | 1 |  0 |
| 6 | 1 |  0 |
| 7 | 1 |  0 |

**This work is the updated version of our previous implementation accepted at the Digestive Disease Week 2024.** <br>

Find the previous version at -<br>
Gopalakrishnan, Keerthy, et al. "Tu2015 A NOVEL 3D CONVOLUTIONAL NEURAL NETWORK BASED DEEP LEARNING MODEL FOR GASTROINTESTINAL ENDOSCOPIC VIDEO CLASSIFICATION: FEASIBILITY STUDY." Gastroenterology 166.5 (2024): S-1493.








