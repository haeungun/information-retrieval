# Support Vector Machine
- 기존의 classification 방법들은 분류 '오류율'을 최소화 하는 목적으로 설계
- SVM 은 두 범주 사이에 존재하는 margin 을 최대화 하여 일반화 능력을 극대화
- 주로 classification 과 회귀분석을 위해 사용

## Terminology
- Hyperplane: p - 차원의 데이터 그룹을 분류하는 데이터를 기준으로 한 (p - 1) - c차원의 subspace
- Support vector: Hyperplane 으로부터 가장 가까운 벡터들
- Margin: 결정선 혹은 결정면으로부터 가장 가까이에 있는 벡터까지의 거리
> 결정선 혹은 결정면에 가까이 있는 점들이 틀릴 가능성이 높기 때문에 결정 한계를 최대로 하는 것이 오류를 가장 줄일 수 있는 방법

## 선형 SVM


## 비선형 SVM
두 범주를 완전하게 나눌 수 있는 hyperplane 이 존재하면 그 두 범주는 선형적으로 분리 가능하다. 그러나 Real world 에서 실제적으로 선형으로 분류가능한 경우는 드물다. 
### Kernel function
주어진 데이터를 고차원 특징 공간으로 맵핑해주는 작업


비선형 SVM 에서 feature 수가 너무 많은 경우(dimension 의 수가 너무 높으면), 각 feature 를 모두 kernel function 을 통과 시켜 맵핑해야 하기 때문에 소요 시간이 증가한다. 따라서 모든 feature 가 hyperplane 을 결정하는데에 영향을 끼치는 것은 아니므로, 불필요한 차원을 축소시킬 필요가 있다.
> 차원을 축소할 수 있는 방법으로는 PCA(주성분 분석), LDA 등이 있다.


## Pros and Cons
- SVM 은 복잡한 비선형 의사결정 영역을 모델화 할 수 있기 때문에 매우 정확
- 학습 데이터를 상당히 줄일 수 있다
- 다른 모델들보다 Overfitting 되는 경향이 적다

- Binary Classification 만 가능

