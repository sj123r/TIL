# Perceptron Training Rule
## 규칙
### 1. 가중치를 초기화 시킨다(0 또는 작은 값)
### 2. 본격
![perceptron_weightupdate](https://github.com/sj123r/Assets/blob/main/Perceptron_weight.jpeg)
>실제 레이블과 예측한 레이블의 차이(y - yi), 학습률(learning rate, n), feature(xi)를 곱한 값을 기존 가중치에 더해서 새로운 가중치에 업데이트 한다.

x 값이 계산에 들어가 있는 만큼 실제 데이터와 예측값의 차이가 클 수록 가중치를 높여 더 크게 조정하겠다는 의미를 내포.(vise versa)

![Activationfunction](https://github.com/sj123r/Assets/blob/main/Activation_function.png)

위 사진에서는 sigmoid function을 임계함수로 활용함. 이전에는 step function을 통해서 임계점 θ를 기준으로 출력을 했다면 이제는 데이터셋에 따라 더 다양한 Activation function을 활용함.