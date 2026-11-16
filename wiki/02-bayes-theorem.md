# 02. Bayes' Theorem & Its 4 Components
# 02. 베이즈 정리 공식과 4대 구성 요소

> **Source Reference:** `[S1]` Bayes & Price (1763)

## 1. Core Formula (핵심 공식)
* **KO:** 결과(데이터 $E$)를 관측한 후, 원인(가설 $H$)이 참일 확률을 역으로 추론(Inverse Probability)하는 공식입니다.
* **EN:** Updates the probability of a hypothesis ($H$) as more evidence or data ($E$) becomes available.

$$P(H \mid E) = \frac{P(E \mid H) \cdot P(H)}{P(E)}$$

## 2. The 4 Building Blocks (4대 구성 요소)

| Term (용어) | Notation | Meaning (KO) | Meaning (EN) |
| :--- | :---: | :--- | :--- |
| **Prior (사전확률)** | $P(H)$ | 증거를 보기 전, 가설 $H$에 대한 초기 믿음 | Initial belief about hypothesis $H$ before seeing evidence |
| **Likelihood (가능도)** | $P(E \mid H)$ | 가설 $H$가 참일 때, 증거 $E$가 관측될 확률 | Probability of observing evidence $E$ assuming $H$ is true |
| **Marginal Likelihood (주변확률)** | $P(E)$ | 모든 가능한 시나리오에서 증거 $E$가 관측될 전체 확률 | Total probability of observing evidence $E$ under all hypotheses |
| **Posterior (사후확률)** | $P(H \mid E)$ | 증거 $E$를 확인한 후 업데이트된 가설 $H$의 확률 | Updated probability of $H$ after observing evidence $E$ |

## 3. Intuition: Updating Beliefs (직관적 이해: 믿음의 업데이트)
$$\text{Posterior (사후 믿음)} \propto \text{Likelihood (데이터의 지지)} \times \text{Prior (기존 믿음)}$$

---
* **Previous:** [[01-conditional-prob|01. Conditional Probability]] | **Next:** [[03-base-rate-fallacy|03. Base Rate Fallacy]]
