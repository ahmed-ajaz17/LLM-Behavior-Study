# LLM Behavior Study

> **Status:** Work in progress. This is a temporary README and will be updated as the study develops.

## Research Question
Does changing the tone of a prompt (polite, neutral, rude, urgent) change how accurately a large language model answers, or how it words its answers?

## Overview
This is a small pilot study. The same set of questions is sent to several LLMs, each wrapped in a different tone. Every prompt is run multiple times, because model outputs vary from run to run. Accuracy is then compared across tones.

## Repository Structure
```
├── data/        # Test questions and correct answers (CSV)
├── prompts/     # Exact wording of each tone condition
├── results/     # Raw model responses
├── analysis/    # Scoring script, summary tables and charts
└── paper/       # Draft notes and the arXiv paper
```

## Planned Design
| Item | Plan |
|------|------|
| Questions | ~100 questions with objective answers |
| Tone conditions | Polite, neutral, rude, urgent |
| Repeats | 3–5 runs per prompt |
| Models | [Model A], [Model B], [Model C] (exact versions and test dates recorded) |
| Analysis | Accuracy per tone, with confidence intervals / significance test |

## Reproducing the Results
1. Open `data/prompts.csv` for the questions.
2. Use the wording in `prompts/conditions.md` for each tone.
3. Save the raw responses in `results/`.
4. Run `analysis/analysis.py` to produce the accuracy tables and charts.

## Limitations
- Small pilot study, so results are preliminary.
- Model behavior changes over time, so results apply only to the versions and dates tested.

## Citation
The arXiv link will be added here once the paper is published.

## License
MIT License. See `LICENSE`.

## Author
[Your name] — [your GitHub handle]
