# Incident Severity BERT

BERT-based NLP classifier for predicting workplace incident severity, 
developed as part of MSc Computer Science research at Northumbria University.

## Research

**Paper:** Predicting Workplace Incident Severity Using BERT-Based NLP —
Probabilistic Classification and SHAP Analysis for UK OHS Decision Support  
arXiv: *submission in progress*

**Model:** HuggingFace — *link coming*

## Key Findings

- DistilBERT achieved 0.58 weighted F1 and 0.60 recall on high-severity incidents
- SHAP attribution revealed a critical **needlestick blind spot**: 99.25% of 
  needlestick injuries misclassified as None severity
- Organisational size feature introduced spurious correlation — 50.8% bias 
  toward None class for small organisations
- Models function as decision-support tools in human-in-the-loop workflows 
  rather than standalone classifiers

## Scope and Limitations

- Trained on US OSHA data, health and social care sector only
- Not validated for UK RIDDOR severity determination outside demonstration contexts
- Time-loss days used as severity proxy — compatible with both OSHA and RIDDOR frameworks
- Cross-jurisdictional performance on UK incident reports not characterised

## Repository Contents

*Code and model weights uploading shortly. Full reproducibility pipeline 
for the dissertation research.*

- `data/` — preprocessing and feature engineering scripts
- `models/` — fine-tuning scripts for DistilBERT and ModernBERT
- `evaluation/` — metrics, confusion matrices, ROC curves
- `shap/` — SHAP attribution analysis and visualisation

## Citation

*arXiv citation will be added upon publication*

## Licence

MIT
