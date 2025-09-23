## 데이터 증강(Data Augmentation)이란?
데이터 증강은 기존 학습 데이터를 변형해 새로운 데이터를 만들어내는 방법이다. 딥러닝 모델은 많은 양의 데이터가 필요하지만, 실제로는 데이터를 충분히 모으기가 쉽지 않다.

이럴 때 데이터 증강을 활용하면 기존 데이터를 여러 방식으로 변형해 쓸 수 있어, 모델의 일반화 능력이 좋아진다. 덕분에 과적합을 막고, 모델이 한 가지 패턴에만 치우치지 않도록 도와준다.    

## 이미지 데이터에서 주로 사용하는 증강 기법

1. 기하학적 변환
- 회전 (Rotation)
- 좌우/상하 반전 (Flip)
- 이동 (Translation)
- 크기 조정(Scaling)
- 잘라내기 (Cropping)

---

2. 픽셀/색상 변형
- 밝기 조정 (Brightness Adjustment)
- 대비 조정 (Contrast Adjustment)
- 색상 변화 (Color Jitter: Hue, Saturation 등)
- 노이즈 추가 (Gaussian Noise, Salt & Pepper Noise)
- 블러 (Blur)

---

3. 노이즈 추가
- Cutout / Random Erasing
- Mixup (두 이미지 섞기)
- CutMix (한 이미지 일부를 다른 이미지에 붙이기)
---
