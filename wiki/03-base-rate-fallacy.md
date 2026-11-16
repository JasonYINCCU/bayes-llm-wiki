# 03. Base Rate Fallacy & Natural Frequencies
# 03. 기저율 오류와 자연빈도(Natural Frequency)

> **Source Reference:** `[S2]` Kahneman & Tversky (1973), `[S3]` Gigerenzer & Hoffrage (1995)

## 1. Base Rate Fallacy (기저율 오류) `[S2]`
* **KO:** 인간이 어떤 사건의 전체적인 발생 빈도인 **기저율(사전확률 $P(H)$)**을 무시하고, 눈앞의 구체적인 증거($P(E \mid H)$)에만 과도하게 집중해 확률을 잘못 판단하는 인지 편향입니다.
* **EN:** A cognitive bias where people ignore general base rate information (prior probability $P(H)$) and focus solely on specific case information ($P(E \mid H)$).

## 2. Prosecutor's Fallacy / Inverse Confusion (역확률 혼동)
* **KO:** 조건의 방향을 뒤바꾸어 착각하는 치명적 오류입니다.
* **EN:** Confusing the probability of evidence given a hypothesis with the probability of the hypothesis given evidence.

$$P(H \mid E) \neq P(E \mid H)$$
*(예: "병에 걸렸을 때 양성일 확률 90%" $\neq$ "양성일 때 병에 걸렸을 확률 90%")*

## 3. Pedagogical Solution: Natural Frequencies (교육적 해결책: 자연빈도법) `[S3]`
* **KO:** 기거렌처(Gigerenzer)의 연구에 따르면, 추상적인 백분율($\%$) 대신 **1,000명 단위의 자연수(자연빈도)**로 표본을 쪼개어 시각화하면 비전공자의 추론 정답률이 15%에서 50% 이상으로 급증합니다.
* **EN:** Replacing normalized percentages with natural frequencies (e.g., "10 out of 1,000 people") makes Bayesian updating transparent and intuitive for non-mathematicians.

---
* **Previous:** [[02-bayes-theorem|02. Bayes' Theorem]] | **Next:** [[04-classic-cases|04. Classic Paradoxes]]
