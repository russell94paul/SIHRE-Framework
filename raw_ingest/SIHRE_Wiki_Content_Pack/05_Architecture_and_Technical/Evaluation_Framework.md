# SIHRE Evaluation Framework

## Evaluation axes

| Axis | Question |
|---|---|
| Drift robustness | Does SIHRE degrade gracefully after distribution shift? |
| Calibration | Does uncertainty remain meaningful under shift? |
| Escalation quality | Does it call verification or simulation at the right times? |
| Abstention quality | Does it defer when evidence is insufficient? |
| Expert contribution | Which modalities improve outcomes? |
| Recovery speed | How quickly does trust update after regime change? |
| Memory usefulness | Does prior evidence improve future reasoning? |
| Verification value | Do critics reduce errors? |
| Simulation value | Do stress scenarios reveal fragility? |
| Cost-benefit | Does added complexity justify compute cost? |

## Recommended evaluation methods

- temporal validation
- ablation tests
- drift simulation
- calibration analysis
- routing analysis
- disagreement analysis
- failure replay
- public-safe synthetic environments
