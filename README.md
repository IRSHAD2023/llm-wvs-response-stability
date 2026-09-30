# LLM Response Stability and Neutral Response Options

This repository contains the code and materials for an NLP seminar
experiment investigating whether adding a neutral response option
affects the stability of repeated LLM responses to World Values Survey
(WVS) items.

## Research Question

Does the availability of a neutral response option affect the stability
of LLM responses to value- and attitude-related survey items?

## Experimental Setup

- Dataset: World Values Survey Wave 7
- Survey items: 30
- Model: Qwen/Qwen2.5-1.5B-Instruct
- Repetitions: 10 per item and condition
- Temperature: 0.7
- Top-p: 0.9
- Total responses: 600

## Response Conditions

### No neutral

- Strongly disagree
- Disagree
- Agree
- Strongly agree

### Neutral available

- Strongly disagree
- Disagree
- Neither agree nor disagree
- Agree
- Strongly agree

## Stability Measure

For each item and condition:

Stability = frequency of the most common response /
number of valid responses.

## Results

Mean modal-response stability:

- No neutral: 0.763
- Neutral available: 0.703
- Difference: -0.060

The direction of change varied across individual items.

## Poster

The `poster/` directory contains the LaTeX source and figures used
to generate the seminar poster.

## Reproducibility

The `experiment/` directory contains the experimental implementation
and checkpoint/results file.

## References

Full academic references are provided in the accompanying appendix.
