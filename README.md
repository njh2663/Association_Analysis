## Association_Rule_Analysis

| 지표 | 계산방법 | 의미 |
|------|----------|------|
| 지지도(support) | P(A $\cap$ B) | 이 조합이 등장한 비율, 얼마나 흔한 경우인가 |   
| 신뢰도(confidence) | $\frac{P(A\cap B)}{P(A)}$ | A를 산 경우 중 B가 포함된 비율, A를 산 사람 중 B를 산 경우가 몇 가지인가 |   
| 향상도(lift) | $\frac{P(A\cap B)}{P(A)P(B)}$ | A와 B가 독립인지, A가 B를 예측하는데 얼마나 영향을 주는지, 1 이상이면 양의 상관관계, 1 이하이면 음의 상관관계 |  
| 레버리지(leverage) | Support(A->B) - Support(A) X Support(B) | A와 B가 독립인지, A가 B를 예측하는데 얼마나 영향을 주는지, 0 이상이면 양의 상관관계, 0 이하이면 음의 상관관계 |  
| 확신도(conviction) | $\frac{(1-Support(B))}{1-Confidence(A->B)}$ | 신뢰도에 대한 확신, 우연히 발생한 것이 아님을 나타내는 수치, 1일 경우 독립 | 
