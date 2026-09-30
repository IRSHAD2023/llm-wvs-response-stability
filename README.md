# LLM Response Stability under Survey Response-Option Conditions

## Research Questions

- Does the availability of a neutral response option affect the stability of LLM responses?
- Is the effect consistent across different survey items?

## Experiment

Model:
Qwen/Qwen2.5-1.5B-Instruct

Dataset:
World Values Survey Wave 7

Items:
30 selected survey items

Conditions:
1. Four-point response scale without a neutral option
2. Five-point response scale with a neutral option

Repetitions:
10 per item and condition

Temperature:
0.7

Top-p:
0.9

## Stability Metric

Modal response share:

stability = frequency of the most common response / number of valid responses

## Results

Mean stability:

- No neutral: 0.763
- Neutral available: 0.703
- Difference: -0.060

Item-level changes:

- Decreased: 14
- Increased: 8
- Unchanged: 8

Neutral responses:

- 6 of 300 responses
- 2%

## Poster

The poster is available in the `poster/` directory.

## Reproducibility

The experiment code and checkpoint data are provided in `experiment/`.

## References

Full academic references and dataset documentation are provided in the appendix.
