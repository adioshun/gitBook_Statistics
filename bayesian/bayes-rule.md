# Bayes Rule 

정의 
- 이전의 경험과 현재의 증거를 토대로 어떤 사건의 확률을 추론하는 과정
- 한 사건이 발생했을 때 이 사건을 근거로 알고자 하는 사실의 가능성을 추측하는 것이다.
- 사전확률 P(A)과 우도(B|A)를 안다면 사후확률 P(A|B)를 알 수 있다
    - 사후확률 문제 -> 사전확률 문제로 변환
    - 우도 (likelihood probability) : A(원인)가 발생하였다.는 조건하에서 B(결과)가 발생할 확률 P(B|A)를 나타낸다.

확률의 개선과정
- 처음 확률은 사전확률 (prior probability) 
- 개선된 확률을 사후확률 (posterior probability) 
- 확률의 개선을 이룩하는 것이 베이즈의 정리 (Bayes' theorem) 이다

![](https://i.imgur.com/1nYH4MY.png)



특징 
- '결과를 관측한 뒤 원인을 추론할 수 있다'는 것입니다.
- 즉, 조건부 확률 P(A | B)를 이용하여 다른 조건부 확률 P(B | A)를 구하는 것이죠.


## 1. 공식 

![](https://i.imgur.com/KlPcfJn.png)


## 2. 유도 

-  분자 :확률의 곱셈정리 (Conditional Probability, product rule)

    ![](https://i.imgur.com/GM4l35r.png)



- 분모 : 전체 확률의 법칙 (Law of total probability, sum rule)

![](https://i.imgur.com/u1MKevW.png)





## 3. 해석 

### 3.1 설명 A

베이지안 룰 `Bayes’ rule is a consequence of conditional probability,`

![](https://i.imgur.com/6nxS25l.png)

### 3.2 설명 B

![](https://i.imgur.com/KkgB9to.png)


- ωi는 우리가 확률을 알고자 하는 명제(proposition)이고, 
- x는 실험(experiment)에서 얻게 되는 정보인 증거(evidence)이다. 
- P(x)는 증거 x가 발생할 확률이고, 
- '사전 확률'(prior probability) P(ωi)는 실험 전의 ωi의 확률이며, 
- '사후 확률'(posterior probability) P(ωi|x)는 실험하여 x를 얻은 후의 ωi의 확률이다. 
- 한편, P(x|ωi)는 명제 ωi가 참인 경우에 증거 x가 발생할 확률이다.




---

|베이즈정리(사후확률 문제 -> 사전확률 문제로 변환)|
|-|
|$$P(\omega_i \mid X ) = \frac{p(X\mid \omega_i)P(\omega_i}{p(X)} = \frac{우도 \times 사전확률}{p(X)}$$|
|- $$P(\omega_i \mid X )$$ : 사후확률, 매개변수 = $$\omega$$= 이산 값 = 대문자 P() <br> - $$P(\omega_i)$$ : 사전확률, 매개변수 = $$\omega$$= 이산 값 = 대문자 P() <br> - $$p(X\mid \omega_i)$$ : 우도, 매개변수 = $$X$$= 연속값 = 소문자 p()|

각 값 구하기
- 사전확률 = 주어진 데이터로 확인 가능 $$\frac{\omega_1분류 데이터수}{총데이터수}$$
- 우도(부류 조건부 확률) = 주어진 데이터 분포 확인 가능, 최대 우도법, MAP등 (3장에서 자세히 다룸)
- p(X) = 삭제 가능(양쪽이 모두 가지고, 크기 비교가 목적이므로)

