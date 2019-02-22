|메인 주제|확률과 통계|
|-|-|
|키워드||
|참고자료|오일석2.1장, |


## 확률과 통계 

![](https://i.imgur.com/6Gn3uE1.png)

- 주머니에서 카드로 뽑아 상자(A,B)를 선택하고, 선택된 상자에서 공(흰색,파란색)을 뽑아 관찰 
- $$ X \in \{A,B\}, Y = \{파랑, 하양\}$$

### 사전 확률 

- 상자 A가 선택될 확률은? 
 - P(X=A)=P(A)=7/10
 

- 상자 A에서 하얀 공이 뽑힐 확률은?  
 - 조건부 확률
 - P(Y=하양|X=A)=P(하양|A)=2/10


- 상자는 A이고 공은 하양이 뽑힐 확률은?
 - 결합 확률
 - P(A, 하양)=P(하양|A)P(A)=(2/10)(7/10)=7/50


- 하얀 공이 나올 확률은?
 - 주변 확률
 - P(하양)=P(하양|A)P(A)+P(하양|B)P(B)=(2/10)(7/10)+(9/15)(3/10)=8/25

> P(X)를 **사전 확률**이라`prior probability` 부름
> - 상자 선택, 공 선택이 연이어 일어 나는데 두번째 사건이 발생 하기 전에 작용하는 확률 이므로 


### 사후 확률 / 우도 

- 시나리오 : 하얀 공이 나왔는데 어느 상자(A or B)에서 나왔는지 모르는 상황 

> Y가 고정되어 있고 X에 따라 확률을 계산 한다. 이 조건부 확률을 **사후 확률**이라 `posterior Probability` 부름 
> - 사전 Y가 일어난 후에 따지는 확률 이므로 

- 활용할 정보 
 - 사전 확률 : P(X=A), P(X=B)   
 - 조건부 확률 : P(하양|A) or P(하양|B) `Y는 하양으로 고정되어 있는 상황에서 X에 따라 확률을 계산 = 우도 or 우도 함수`


- 계산 
 - $$ P(A \mid 하양) =  \frac{P(하양 \mid A)P(A)}{P(하양)} = \frac{(\frac{2}{10})(\frac{7}{10})}{(\frac{8}{25})} = 0.4375   $$
 
 - $$ P(B \mid 하양) =  \frac{P(하양 \mid B)P(B)}{P(하양)} = \frac{(\frac{9}{15})(\frac{3}{10})}{(\frac{8}{25})} = 0.5675   $$
 - B에서 신뢰도 0.5625로 나온다. 












---

# 조건부 확률 

## 1.  정의 

확률 분포 표현법 
- 이산 : 대문자 P(.)
- 연속 : 확률 밀도 함수(pdf), 소문자 p(.)

### 1.1 Sample Sapce
S(set)

### 1.2 Event (A) 
A $$\in$$ S
P(A) = prob(outcome $$\in$$ A)

### 1.3 Conditional Probability (조건부 확률)
어떤 조건에서 목적하는 이벤트가 발생할 확률

P(B|A) : A라는 조건에서 B가 발생할 활률
- 계산 : $$ \frac{P(B \cap A)}{P(A)} $$

예 : P(오늘 날씨|어제 날씨)

### 1.4 Total Probability(전체 확률)
> 베이즈확률을 위한 기본 법칙

$$P(A) = P(A_1)+P(A_2)...+P(A_n)$$, 때 $$A_1, A_2, A_3.....A_n$$ = Partition of S

$$P(A_1) = P(A_1 \cap A)$$  
$$P(A) = \sum^n_{i=1} P(A|A_i)P(A_i)$$
- $$P(A|A_i)$$=Priori 

### 1.5 Bayesian Theorem

$$P(B|A) = \frac{P(B \cap A)}{P(A)}= \frac{P(A|B)P(B)}{P(A)} $$

Partition에 적용 : $$P(A_i|A) = \frac{P(A|A_i)P(A_i)}{P(A)} $$

- $$A$$ = Observation, Data
- $$A_i$$ = Original, (unKonw)Input

Data를 통해서 Input 을 알고자 할때 사용 

### 1.6 Independent Events 

If A and B are mutually independent, $$P(B|A) = P(B) = \frac{P(A \cap B}{P(A)}$$
- Repeated (restored) rials = (복원) 반복 추출
- 영향을 안 미침 

문제를 단순화 시켜줌 

조심 : Indendent $$\neq $$exclusive

### 1.7 Combined experiments
For two experiments with $$S_1, S_2 \Rightarrow  S = S_1 \times S_2 $$
- Ex) 동전 3개 던지는 실험 

---

# 순열과 조합 

# Combinatorial Analysis 

## 1. 순열(Permutations)

### 1.1 Line Permutation

line arrangement(order) of n different object 
- n개의 오브젝트를 순서를 고려 하여 일렬로 나열 
- n!

line arrangement(order) r out of n different object
- n개 오브젝트를 순서를 고려 하여 일렬로 나열 
- nPr
- $$\frac{n!}{(n-r)!}$$

### 1.2 Group Permutation 

중복이 있는 것의 순열 (eg. 흰공 3개, 검은공 4개, 빨간공 2개)

### 1.3 Circular Permutation 
- 순서고려 안함(원형 순열)
- $$\frac{n!}{n}$$


## 2. 조합(Combination) 

### 2.1 기본

Select $$r$$ objects out of $$n$$ ones, 순서 없음

- $$nCr = \frac{nPr}{r!}= \left(\begin{array}{c}n\\ r\end{array}\right)=\frac{n!}{(n-r)!r!}$$

- $$\left(\begin{array}{c}{n+m}\\ r\end{array}\right) = \sum^r_{k=0}\left(\begin{array}{c}{n}\\ k\end{array}\right) \left(\begin{array}{c}{m}\\ r-k\end{array}\right) $$


### 2.2 이항정리(Binomial Theorem)

$$ (a+b)^n = $$



###### [참고] Stirling's Formula 
- !, 팩토리얼 계산시 사용 
- $$n! \approx \sqrt{2\pi n}(\frac{n}{e})^n$$

## 3. Reliability (신뢰도)
- Duration of useful function of system
- R(t) : Probability that a system will be function at time t 

### 3.1 직렬 연결

### 3.2 병렬 연결  
