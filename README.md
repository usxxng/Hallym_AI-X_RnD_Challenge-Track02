# Hallym_AI-X_RnD_Challenge
## Track02. 피부암 영상 인식 및 판별 (2020 한림대학교 AI+X R&amp;D 챌린지)


[\[Competition Page\]](https://www.kaggle.com/c/hallym-2020-2-aicomp02)<br>
![img1](./img1.PNG)
<br>

![img2](./img2.PNG)
## Private Leaderboard : 1st (NAME : useung)

[\[Solution 참고\]](./solution_track02_report.pdf)<br>

### sub_log
83.667 - efficientNet b3  lr - 0.0001 ep 10

*************************************************************************************************************************
84.527 - efficientNet b3 / lr - 0.0001 / ep 10 <br> 
transforms(resize(320,320), CenterCrop(280,280), RandomHorizontalFlip, RandomVerticalFlip, RandomRotation(10) <br>
param.require_grad = True(이전 레이어 전체 학습) <br>
data loader : train - batchsize 32 , val - batchsize 8 <br>

Dataset - image preprocessing
<br>(이미지 라운드를 통해 특징점에 더 집중할 수 있도록 데이터 증강)
<br>Data Augmentation - OpenCV 활용
![img3](./img3.PNG)<br>

Albumentation
![img4](./img4.PNG)<br>



Best acc : 0.8574<br>
Evaluation<br>
Avg loss(test) : 0.0479<br>
Avg acc(test) : 0.8702<br>

*************************************************************************************************************************
<br>

Public Leaderboard Score : 0.84527<br>
Private Leaderboard Score : 0.82000