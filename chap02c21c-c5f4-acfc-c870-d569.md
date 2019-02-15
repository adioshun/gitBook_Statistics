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
