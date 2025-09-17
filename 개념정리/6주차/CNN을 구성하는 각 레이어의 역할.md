# :pushpin:CNN을 구성하는 각 레이어의 역할

## :link:Convolutional Neural Network (CNN, 합성곱 신경망)
CNN은 주로 이미지 처리 및 컴퓨터 비전 분야에서 널리 사용되는 딥러닝 모델이다. CNN은 이미지와 같은 2차원 데이터를 처리하는 데 특화된 구조를 가지고 있으며, 합성곱 연산을 통해 입력 데이터를 효과적으로 분석하고 특징을 추출한다.

## :jigsaw:CNN의 주요 구성 요소
- 합성곱 층 (Convolutional Layer)
  - Convolutional layer는 CNN의 핵심 구성 요소로, 커널을 사용하여 입력 이미지에서 작은 지역적인 특징을 추출
  - 커널 이미지의 일부 영역에 대해 합성곱(Convolution) 연산을 수행하고, 그 결과 새로운 특징 맵을 만든다.

- 풀링 층(Pooling Layer)
  - Pooling layer는 합성곱 층에서 나온 특징 맵을 다운샘플링(Downsampling) 하여 크기와 계산량을 줄이고, 중요한 정보만 유지한다.
  - Max Pooling, Average Pooling, Min Pooling이 있으며, 주로 CNN에서는 Max Pooling을 많이 사용한다.

- 완전 연결층(Fully Connected Layer)
  - 합성곱 층과 풀링 층을 거친 특징을 사용하여 최종적인 분류를 수행
  - 이전 층에서 추출된 특징을 이용해 입력을 특정 클래스로 분류하는 역할

- 출력층(Output Layer)
  - 마지막 출력층에서는 Flatten나 Softmax 같은 함수를 사용하여 결과 변환

- 활성화 함수(Activation Function)
  - 합성곱 층의 출력을 비선형적으로 변환하기 위해 활성화 함수 사용  
    활성화함수 종류)  ReLU, Sigmoid, Tanh 등등...



## CNN 응용 분야
- 이미지 분류: CNN은 이미지가 어떤 카테고리에 속하는지를 예측하는 문제에 사용됩니다. 예: 개, 고양이, 자동차 등.  
- 물체 인식(Object Detection): 이미지에서 특정 물체의 위치와 종류를 탐지하는 문제.  
- 이미지 분할(Image Segmentation): 이미지 내 각 픽셀이 어느 객체에 속하는지를 분류하는 문제.
