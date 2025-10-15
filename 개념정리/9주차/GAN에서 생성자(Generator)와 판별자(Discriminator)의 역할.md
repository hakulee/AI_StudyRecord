# GAN에서 생성자(Generator)와 판별자(Discriminator)의 역할

## GAN(Generative Adversarial Network) 모델
GAN은 두 개의 신경망인 생성자(Generator)와 판별자(Discriminator)가 서로 경쟁하면서 데이터를 생성하는 모델이다.  
<img width="400" height="350" alt="image" src="https://github.com/user-attachments/assets/82af7566-f696-43cb-a19e-93c2fe9edab7" />


## 생성자(Generator)
생성자(Generator)는 새로운 데이터를 만들어내는 역할을 한다. 랜덤한 노이즈를 입력으로 받아, 실제 데이터와 구별할 수 없을 정도로 유사한 데이터를 생성한다.

이후 실제 데이터와 가짜 데이터를 적절히 섞어 판별자에게 입력한다. 이때, 판별자는 실제 이미지를 1로, 가짜 이미지를 0으로 구별한다.
이를 통해 생성자는 학습을 거듭하면서 점점 더 현실적인 데이터를 만들어내도록 발전하게 된다.
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/9fc3a228-1927-411a-802d-a3aa8d073a04" />


## 판별자(Discriminator)
반면, 판별자(Discriminator)는 입력된 데이터가 실제 데이터인지, 생성자가 만든 가짜 데이터인지 구별하는 역할을 한다. 
처음에는 가짜 데이터를 쉽게 구별할 수 있지만, 
생성자가 점점 더 정교한 데이터를 만들면서 판별자의 판단이 어려워지게 된다.
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/f5299ec6-7af5-4445-a06b-8913fc224ecb" />


## 생성자와 판별자의 관계
이 두 네트워크는 적대적 학습(adversarial learning)을 통해 서로 경쟁하며 성능을 향상시킨다. 
생성자는 판별자를 속이기 위해 점점 더 현실적인 데이터를 만들어내려 하고, 판별자는 생성자가 만든 데이터를 더 정확하게 구별하려고 학습한다. 
결국, 이 과정이 반복되면서 생성자는 점점 더 실제 데이터와 구별하기 어려운 고품질의 데이터를 생성할 수 있게 된다.

