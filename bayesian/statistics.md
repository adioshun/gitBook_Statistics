# 베이지안 통계

통계 분류 
- 고전 통계학
    - 관측된 현상(phenomena)은 '우리가 알지 못하는 고정된 프로세스'로부터 발생한 것이라는 가정을 가지고, 그 현상을 분석하는 통계학이다. 
    - 따라서 p값을 가정한 뒤, 그 값이 타당한 값인지를 검정하고, 타당하다고 판단되면 그 p값으로 예측하는 것이다.

- 베이즈 통계학
    - 실증적(empirical) 통계학이라 이야기할 수 있다. 즉, 과거의 결과를 기반으로 분석 및 예측하는 통계학을 말한다.
    - '조건부 확률(conditional probability)'과 '베이즈 정리(bayes rule)'을 이용한다

> 고전 통계학은 통계적 모델(model)을 가정하여, 과거의 결과(data)에 대한 분석을 바탕으로 모델의 타당성을 검정하고, 베이즈 통계학은 과거의 결과에 대하여 모델의 가능성을 계산하여 예측한다고 말할 수 있다

정의 
- A statistical inference framework
- Can be used for estimation, classification, detection, model selection, etc.

특징 
- unknown quantities are described as **random**.


단점 
- 계산하기 어렵다는 문제가 있다. (eg.미적분학)
- 가정이 타당하지 않으면 그 계산 결과는 신뢰하기가 어렵다.
- 마지막으로 베이즈 통계학에서는 모델을 확률 변수처럼 사용하였다.

활용 예 #1 : 병원 

- Quantity of interest: the disease
- Observations: blood samples, temperature, comments by patient, etc
- 결과 : based on our observations, patient has disease X with 97% probability

활용 예 #2 : 자율 주행 차 

- Quantity of interest: relative position and velocity of other vehicles at the current time.
- Observations: wheel speeds, INS measurements, radar detections (distance and angle), Lidar point clouds, camera images, etc.
- 결과 : vehicle motions are modelled statistically


기존 통계학과의 차이점 `COMPARISON: BAYES VS FREQUENTIST`

- We wish to estimate the height of the Eiffel tower. 
    - Frequentist perspective: the tower has a certain height and is therefore not random.
    - Bayesian perspective: we describe our uncertainties in the height stochastically -> height is described as random!
    
OVERVIEW OF THE BAYESIAN STRATEG
- Modeling.
- Measurement update (본 강의에서 주로 다룸) 
- Decision making