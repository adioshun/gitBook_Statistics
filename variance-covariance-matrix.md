# 분산공분산 행렬 [ variance-covariance matrix ]

>  다변량 자료를 분석할때 분산이 하나의 값으로 표현이 되지 않으므로 variance-covariance matrix를 사용

여러 개의 변수를 동시에 고려할 때, 각 변수의 분산과 변수 사이의 공분산을 요소로 구성된 행렬을 말한다. X1, X2, ..., Xk와 같이 k개 변수를 고려하면, k×k분산-공분산 행렬을 생성할 수 있다. 

대각선 행렬 값은 각 변수의 분산이고, 
대각선 이외의 행렬 값들은 변수 사이의 공분산이다.



---

## [Variance-Covariance Matrix](https://stattrek.com/matrix-algebra/covariance-matrix.aspx)

## 1. Variance 

정의 : a measure of the variability or spread in a set of data. 

계산법 : it is the average squared deviation from the mean score. 

Var(X) = Σ ( Xi - X )^2 / N = Σ x_i^2 / N



## 2. Covariance

정의 : 같이 변화 하는 요소 찾기, 관련도 높은것, 
    - `a measure of the extent to which corresponding elements from two sets of ordered data move in the same direction. `
    - `covariance is a measure of how much two random variables change to gether`


## 3. Variance-Covariance Matrix (=covariance matrix)

정의 
- 정방 행렬의 값을 각 변수의 분산과 공분산으로 채운 것이 바로 공분산 행렬입니
- Variance and covariance are often displayed together in a variance-covariance matrix

The variances appear along the diagonal and covariances appear in the off-diagonal elements, as shown below.
- 대각선 행렬 값은 각 변수의 분산이고, 
- 대각선 이외의 행렬 값들은 변수 사이의 공분산이다.



---

# correlation matrix




correlation coefficient도 여러개가 되며 이것을 행렬로 정리한 것이 correlation matrix


