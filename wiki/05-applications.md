# 05. Real-World Application: Naive Bayes Spam Filter
# 05. 현실 응용: 나이브 베이즈 스팸 필터

> **Source Reference:** `[S5]` Paul Graham (2002), *A Plan for Spam*

## 1. How Spam Filters Use Bayes' Theorem (스팸 필터의 작동 원리)
* **KO:** 이메일에 특정 단어(예: `"Free"`, `"당첨"`)가 포함되었을 때, 그 메일이 스팸일 사후확률 $P(\text{Spam} \mid \text{Word})$를 계산합니다.
* **EN:** Computes the posterior probability that an email is spam given the presence of specific trigger words.

$$P(\text{Spam} \mid \text{Word}) = \frac{P(\text{Word} \mid \text{Spam}) \cdot P(\text{Spam})}{P(\text{Word} \mid \text{Spam})P(\text{Spam}) + P(\text{Word} \mid \text{Ham})P(\text{Ham})}$$
*(Ham = 정상 메일 / Legitimate email)*

## 2. Why "Naive"? (왜 '순진한(Naive)' 베이즈인가?)
* **KO:** 문장 속 각 단어가 서로 독립적으로 등장한다고 단순화(조건부 독립 가정)하여 계산 속도를 극대화하기 때문입니다. 현실에서는 단어 간 문맥이 존재하지만, 실무에서 놀라울 정도로 높은 분류 정확도를 보입니다.
* **EN:** Assumes conditional independence between words given the class label. Despite this simplifying assumption, it performs remarkably well in real-time text classification.

## 3. Continuous Learning (지속적 업데이트)
* **KO:** 사용자가 새로운 메일을 '스팸 신고'할 때마다 단어별 우도($P(\text{Word} \mid \text{Spam})$)가 갱신되어 새로운 스팸 유형에도 스스로 적응합니다.
* **EN:** Every time a user marks an email as spam, the likelihood tables update dynamically to adapt to new spam patterns.

---
* **Back to Hub:** [[index|Wiki Index]]
