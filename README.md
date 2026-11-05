# AI Strategic Narrative Analysis (2020–2026)

This project operationalizes the concept-notes framework for computational analysis of AI narratives in public-company disclosures, with emphasis on **FMCG vs Hardlines** sector dynamics over time.

## Scope

The workflow analyzes PDF-based corporate materials and extracts evidence of AI discourse across three layers:

1. **AI Mention Eligibility**  
   Detects AI-related terminology in documents and quantifies yearly exposure.
2. **Zero-Shot Topic Classification**  
   Classifies AI-related snippets into:
   - Cost Reduction & Operational Efficiency
   - Revenue Generation & Product Innovation
   - Supply Chain & Inventory Logistics
   - Governance, Risk & Ethics
3. **Sentiment Classification**  
   Scores snippet-level sentiment (Negative / Neutral / Positive) and tracks sector-year evolution.

## Main Notebooks

- `ai_eligibility_pdf_analysis.ipynb` — robust PDF extraction, AI-term detection, eligibility rates, AIE-style exposure metrics.
- `ai_zero_shot_topic_classification.ipynb` — transformer zero-shot topic assignment for AI snippets, with sector/year trend charts and heatmaps.
- `ai_snippets_sentiment_classification.ipynb` — transformer sentiment classification for snippets from `data/snippets.csv`, with overall and sector-level evolution.

## Data Assumptions

- Raw and derived datasets are placed under `data/`.
- Metadata file: `data/metadata.json`.
- Snippet-level sentiment notebook expects: `data/snippets.csv`.

## Reproducibility Notes

- Python 3.10+ recommended.
- Install dependencies from `requirements.txt`.
- Run notebooks top-to-bottom to refresh all intermediate outputs and plots.

## Research Intent

The setup supports evidence-building for strategic narrative shifts in AI communication across sectors and years, rather than single-firm case interpretation.
