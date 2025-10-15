#  Semantic Segmentation이란 무엇이며, 이미지 분류(Classification)와 어떤 차이가 있는가?

## 이미지 분류 (Classification)  
이미지 분류는 주어진 이미지가 무엇인지 판별하는 것이다. 즉, 이미지 전체에 대해 단 하나의 클래스를 예측하는 과정이다.  
따라서 출력은 보통 하나의 클래스 레이블이다. 이미지에서 객체의 위치나 세부적인 정보는 고려하지 않으며, 전체 이미지에 대한 판단만 이루어진다.

> 이미지 분할은 크게 두 가지 종류로 나뉜다.  
> Instance Segmentation: 같은 클래스의 다른 객체들을 개별적으로 구분하여 분할한다.  
> ex) 사람 무리에서 각기 다른 사람들을 인식  
> Semantic Segmentation: 같은 클래스라면 동일하게 취급하여 분할한다.  
> ex) 모든 사람은 같은 클래스  
<img width="919" height="269" alt="image" src="https://github.com/user-attachments/assets/f9e0c784-a078-4cca-8462-67730980ae35" />


## 이미지 분류와 Segmentation의 차이
이미지 분류는 개별 객체를 인식하는 데 유용하고, 이미지 분할은 자율주행(차선 및 보행자 감지),
의료 영상 분석(암 조직 탐지) 등과 같이 정확한 영역 구분이 필요한 작업에서 유용하다.
