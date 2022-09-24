# OvR vs. OvO
## OvR (One vs Rest), OvO(One vs One)

Perceptrons, logistic regression models, support vector machines weren't designed for multi-classification training.

Since they were made for binary classification OvR and OvO were used as a tool that enabled multi-classification.

## One-Vs-Rest
One-Vs-Rest is a method of splitting multiple classes into many binary classifications. 

Ex)
There exists three classes: red, blue, green.
This could then be divided into the following:
- **Binary Classification Problem 1:** red vs [blue, green]
- **Binary Classification Problem 2:** blue vs [red, green]
- **Binary Classification Problem 3:** green vs [red, blue]

However, this implies that for every dataset there needs to be a corresponding alogrithm model. Therefore, the classes were classified into:
- **Binary Classification Problem:** red vs [everything else]

>This approach requires that each model predicts a class membership probability or a probability-like score. The argmax of these scores (class index with the largest score) is then used to predict a class.

!!활용도: Gan의 판별기도 확률을 통해서 어떤 클래스에 대한 classification을 한다. 예를 들어서 1010 패턴을 생성하는 생성자가 만든 아이템은 1에 가까이 판별하지만 랜덤한 난수는 거의 0에 가까운 숫자를 반환한다. 

즉 클래스는 수치화 할 수만 있다면 아무런 문제가 없다.

