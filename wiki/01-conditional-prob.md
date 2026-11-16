# 01. Conditional Probability & Law of Total Probability
# 01. 조건부 확률과 전확률의 법칙

## 1. Conditional Probability (조건부 확률)
* **KO:** 어떤 사건 $B$가 이미 일어났다는 전제하에, 다른 사건 $A$가 일어날 확률입니다. 직관적으로는 **전체 표본공간(Sample Space)을 사건 $B$로 축소**하는 과정입니다.
* **EN:** The probability of event $A$ occurring given that event $B$ has already occurred. Intuitively, it shrinks the sample space from $\Omega$ down to $B$.

$$P(A \mid B) = \frac{P(A \cap B)}{P(B)}, \quad \text{where } P(B) > 0$$

* **Multiplication Rule (곱셈정리):**
  $$P(A \cap B) = P(B \mid A)P(A) = P(A \mid B)P(B)$$

## 2. Law of Total Probability (전확률의 법칙)
* **KO:** 사건 $B$가 일어날 전체 확률을 구하기 위해, 표본공간을 서로 배반인 사건들($A_1, A_2, \dots, A_n$)로 나누어 각각의 경로를 모두 더하는 법칙입니다.
* **EN:** Calculates the total probability of an outcome $B$ by summing its probabilities across all mutually exclusive and exhaustive scenarios ($A_1, A_2, \dots, A_n$).

$$P(B) = \sum_{i=1}^{n} P(B \mid A_i)P(A_i)$$

* **Binary Case (이진 사건의 경우, $A$와 $A^c$):**
  $$P(B) = P(B \mid A)P(A) + P(B \mid A^c)P(A^c)$$

---
* **Next:** [[02-bayes-theorem|02. Bayes' Theorem (베이즈 정리)]]
