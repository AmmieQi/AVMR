## Adversarial Video Moment Retrieval by Jointly Modeling Ranking and Localization (AVMR)
This is our implementation for the paper:

Da Cao, Yawen Zeng, Xiaochi Wei, Liqiang Nie, Richang Hong, Zheng Qin. 2020. Adversarial Video Moment Retrieval by Jointly Modeling Ranking and Localization. In The ACM International Conference on Multimedia (ACM MM '20). ACM, Seattle, United States.

## Environment Settings
We use the framework pytorch.

* pytorch version: '1.2.0'
* python version: '3.5'

## AVMR
The released code consists of the following files.
```
--workplaceTest
--workplaceTrain
--feature_all
--main.py
--MADDPG.py
--model.py
--memory.py
--utils.py
--randomProcess.py
--readme
```

## Example to run the codes
Run AVMR：
```
python main.py
```

## Example demo
AVMR_demo_YVKIV.mp4

The visualization of five generated video moments on five iterations is revealed above. The green line and green box indicate the ground truth, the black line and black box represent the generated video moment candidates.

## Dataset
We provide two processed datasets: Charades-STA && TACoS
The strategy of multi-scale sliding windows is utilized to segment each video with the size of [64, 128, 256, 512] frames with 80% overlap and we randomly selected 80% and 20% of them for training and testing, respectively.

All features are saved in ./feature_all_train, ./feature_all_test. 
* These two processed features are available for downloading here: https://drive.google.com/open?id=1-AMToMuTlPRY1C2n0ZoyKrwBsVPehbFK
* The original videos and their corresponding caption annotations/querys: https://github.com/jiyanggao/TALL and http://www.coli.uni-saarland.de/projects/smile/tacos

## Workspace
/workplaceTest and /workplaceTrain that processes videos in advance as a runtime workspace.

#


Last Update Date: Jul 28, 2020
