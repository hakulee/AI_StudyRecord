# mAP(mean Average Precision)?
mAP는 한국말로 번역하면 평균 정확도의 평균이다. 좀 더 자세히 풀어보면, 
mAP는 AP(Average Precision)의 평균이고 AP는 Precision의 평균이다. 

- Precision
  - 정밀도로 모델이 True로 예측한 것들 중에서 실제 True인 비율  
    <img width="365" height="168" alt="image" src="https://github.com/user-attachments/assets/0e59a20d-78df-4223-9d7c-f147bb618079" />


- IoU
  - 모델이 검출한 bounding box가 ground truth box와 얼마만큼 겹치는지를 나타내는 지표
    특정 threshold 값을 넘긴 predict bounding box에 대해서 TP로 판단    
    <img width="500" height="280" alt="image" src="https://github.com/user-attachments/assets/995dc024-7872-4da4-a85f-cc1d7f6f8d0f" />

- PR Curve
  - confidence score에 대한 threshold 값이 변화함에 따른 Precision과 Recall의 변화량을 나타낸 그래프이다. object detection에서 confidence score는 IoU가 된다  
    <img width="400" height="350" alt="image" src="https://github.com/user-attachments/assets/b2b07d9e-48cb-49a6-b353-e938cdeea2e7" />

- AP
  - AP는 PR Curve의 아래 영역이 된다. AUC가 ROC curve의 아래 영역을 의미하는 것과 동일하다.
    Curve의 아래영역을 계산하기 쉽게 하기 위해서 PR Curve가 단조적으로 감소하도록 수정한 후 AP를 계산한다.  
    <img width="400" height="350" alt="image" src="https://github.com/user-attachments/assets/12a73be7-f621-44b8-83d6-a0c5e59ec0f3" />

- mAP
  - object detection task에서는 강아지, 고양이, 자동차, 비행기 등 탐지하고자 하는 물체(class)가 다양하다.
    mAP란 각 class 별 AP의 평균을 나타낸 값으로 모델의 정확도를 측정하는 평가 지표가 된다.

## 객체 인식에서의 활용
- mAP는 YOLO, Faster R-CNN, SSD 등 객체 인식 모델의 대표적인 성능 지표로 사용
- 즉, mAP는 모델이 얼마나 정확하게 객체를 탐지하고, 각 클래스별 예측 성능이 얼마나 균일한지를 종합적으로 보여준다.
