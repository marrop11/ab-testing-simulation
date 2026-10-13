# A/B Testing Simulation

## Výskumná otázka
Koľko pozorovaní potrebujeme, aby sme spoľahlivo odhalili zvolený
rozdiel v konverznom pomere (MDE) pri α = 0.05 a power = 0.80?
Ako sa správajú klasické testy pri priebežnom sledovaní výsledkov?

## Motivácia
Projekt nadväzuje na diplomovú prácu — správny návrh experimentu
šetrí pozorovania a znižuje riziko falošných záverov.

## Plán projektu
| Deň | Úloha |
|-----|-------|
| 13.10 | Power analysis – štúdium, základ teórie |
| 14.10 | Implementácia `sample_size.py` |
| 15.10 | Simulácia A/A testov (overenie α = 5 %) |
| 16.10 | Peeking problem – ako rastú falošné pozitíva |
| 17.10 | Sekvenčné testovanie (alpha spending) |
| 26.10 | Grafy a vizualizácie (matplotlib) |
| 27.10 | Prepojenie s diplomovkou |

## Metódy
- `statsmodels.stats.power.TTestIndPower` (frekventistický prístup)
- Simulácia Monte Carlo
- Alpha spending (Lan–DeMets)
- Bayesovský A/B test (beta-binomický model)


## Zdroje
- [Evan Miller – Sample Size Calculator](https://evanmiller.org/ab-testing/sample-size.html)
- [statsmodels – TTestIndPower](https://statsmodels.org/stable/generated/statsmodels.stats.power.TTestIndPower.html)
- [TDS: Minimum sample size in statsmodels](https://towardsdatascience.com/computing-minimum-sample-size-for-a-b-tests-in-statsmodels-how-and-why-398e357945d9/)