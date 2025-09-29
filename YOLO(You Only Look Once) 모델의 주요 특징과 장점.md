# YOLO(You Only Look Once) 모델의 주요 특징과 장점

## YOLO(You Only Look Once) 모델
<img width="901" height="460" alt="17591504107209215213449165914390" src="https://github.com/user-attachments/assets/1c1ce915-6b57-4c1c-9486-242fd8a36b3f" />

YOLO(You Only Look Once)는 실시간 객체 탐지(Object Detection) 분야에서 혁신을 일으킨 딥러닝 모델이다.
YOLO는 이미지를 한 번만 처리하여 객체를 탐지하는 방식으로, 매우 빠른 속도와 높은 정확도를 자랑한다.

기존의 객체 탐지 모델들은 이미지에서 객체를 탐지하기 위해 이미지의 여러 부분을 반복적으로 처리하는 방식을 사용했지만, 
YOLO는 이미지 전체를 한 번에 처리하여 객체를 탐지한다.
이로 인해 YOLO는 실시간으로 객체를 탐지하는 데 매우 효율적이다.

## YOLO 모델의 특징
- 이미지 전체를 한번만 본다.
- one-stage로 통합하여 빠르다
- 주변 정보까지 학습하여 이미지 전체를 처리하기 때문에 background error가 적다
- 훈련 단계에서 보지못한 새로운 이지미에 대해서도 검출 정확도가 높다

<img width="1280" height="851" alt="17591509055238627416505903304534" src="https://github.com/user-attachments/assets/69fd7644-2d24-4d51-9e54-23e3f356dfe5" />

사진을 입력하면 그리도로 나눠

## YOLO 모델의 장점




> 단점:
> 실시간으로  object detection이 가능하고 기존의  Faster R-CNN 보다 6배 빠른 성능을 보였기 때문이다.
하지만 R-CNN계열 모델들에 비해 낮은 정확도를 가지고 있으며 특히 작은 객체에 대해 정확도가 아쉬울 정도로 낮은 편이다.

 
