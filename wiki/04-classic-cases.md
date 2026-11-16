# 04. Classic Paradoxes: Medical Test & Monty Hall
# 04. 대표 사례: 희귀병 진단 역설 & 몬티홀 문제

> **Source Reference:** `[S3]` Gigerenzer & Hoffrage (1995), `[S4]` Selvin (1975) & vos Savant (1990)

## Case 1: The Rare Disease Paradox (희귀병 진단 역설) `[S3]`
### Setup (문제 설정)
* **Prevalence (유병률 / Prior):** $P(D) = 1\%$ (1,000명 중 10명 감염)
* **Sensitivity (민감도 / Likelihood):** $P(+ \mid D) = 90\%$ (환자 중 90%가 양성 판정)
* **False Positive Rate (위양성률):** $P(+ \mid D^c) = 10\%$ (건강한 사람 중 10%가 오진으로 양성 판정)
* **Question:** 양성 판정($+$)을 받았을 때, 실제로 병에 걸렸을 확률 $P(D \mid +)$는?

### Natural Frequency Breakdown (1,000명 기준 자연빈도 분석)
| Group (집단) | Total (인원) | Test Positive ($+$) | Test Negative ($-$) |
| :--- | :---: | :---: | :---: |
| **Infected ($D$, 환자)** | 10 | **9** (True Positive) | 1 (False Negative) |
| **Healthy ($D^c$, 정상)** | 990 | **99** (False Positive) | 891 (True Negative) |
| **Sum (합계)** | **1,000** | **108** | **892** |

$$P(D \mid +) = \frac{9}{9 + 99} = \frac{9}{108} = \frac{1}{12} \approx \mathbf{8.33\%}$$
* **Takeaway:** 검사 정확도가 90%여도 병 자체가 희귀하기 때문에, 양성 판정자 108명 중 99명은 가짜 양성(오진)입니다.

---

## Case 2: The Monty Hall Problem (몬티홀 문제) `[S4]`
### Setup (문제 설정)
* 3개의 문($1, 2, 3$) 중 하나 뒤에 자동차가 있고, 나머지 둘 뒤에는 염소가 있습니다.
* 참가자가 **1번 문**을 선택하자, 정답을 아는 사회자가 염소가 있는 **3번 문**을 열어 보여주었습니다($E = H_3$).
* **Question:** 선택을 **2번 문**으로 바꾸는 것이 유리할까?

### Bayesian Calculation (베이즈 업데이트)
* **Prior (사전확률):** $P(C_1) = P(C_2) = P(C_3) = \frac{1}{3}$ ($C_i$: $i$번 문에 차가 있는 사건)
* **Likelihood (사회자가 3번 문을 열 확률):**
  * $P(H_3 \mid C_1) = \frac{1}{2}$ (사회자가 2번, 3번 중 무작위 선택)
  * $P(H_3 \mid C_2) = 1$ (사회자는 차가 있는 2번을 열 수 없으므로 반드시 3번 선택)
  * $P(H_3 \mid C_3) = 0$ (차가 있는 3번 문을 열 수 없음)

$$P(C_2 \mid H_3) = \frac{P(H_3 \mid C_2)P(C_2)}{P(H_3 \mid C_1)P(C_1) + P(H_3 \mid C_2)P(C_2) + P(H_3 \mid C_3)P(C_3)} = \frac{1 \cdot \frac{1}{3}}{\frac{1}{2}\cdot\frac{1}{3} + 1\cdot\frac{1}{3} + 0} = \mathbf{\frac{2}{3}}$$

* **Takeaway:** 사회자의 의도적인 정보 공개($H_3$)로 인해 2번 문에 차가 있을 사후확률이 $\frac{1}{3}$에서 **$\frac{2}{3}$**로 2배 상승합니다.

---
* **Previous:** [[03-base-rate-fallacy|03. Base Rate Fallacy]] | **Next:** [[05-applications|05. Real-World Applications]]
