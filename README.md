# Image_Classification
# CNN을 이용한 이미지 분류 모델 구현

keras에서 제공되는 cifar10 데이터를 사용하여 진행하였다.

결과는 5개 모두 화질이 좋지 않음에도 꽤 높은 정확율을 보였다. 이런 방식으로 상품이미지에 대한 카테고리 라벨을 학습시켜 이미지 특징으로 카테고리를 구분할 수 있는 인공지능을 만들 수 있을 것이다.

또한 전이학습을 이용한 이미지 분류도 진행하였다.

전이학습은 시존에 사전학습된 모델을 가져와, 사용하고자 하는 학습 데이터를 학습시켜 이용하는 방식으로, 데이터가 다소 적더라도 좋은 성능을 보여줄 수 있다.

이것은 ResNet50을 이용하여 분류를 진행하였다.
ResNet50은 Residul Net이라고 하며 각각의 Con -> BatchNormalization -> ReLU 로 묶인 residual 값을 추가적으로 더해줌으로써 gradient vanishing/exploding 문제를 해결할 수 있다.
