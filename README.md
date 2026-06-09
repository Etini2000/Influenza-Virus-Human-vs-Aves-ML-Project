# Influenza-Virus-Human-vs-Aves-ML-Project
## Project Overview
This project features a production-grade machine learning pipeline that automatically identifies whether a mutating strain of the Influenza A virus is adapted to infect Humans or restricted to Avian (Bird) hosts. Using real genetic sequences pulled live from the NCBI Nucleotide Database, the model trains on localized structural protein changes using text-tokenization ($K$-mers) and achieves an outstanding 98.67% predictive accuracy.

## Key Skills Showcased
### Live Database Mining: Used Biopython (Entrez) to stream, structure, and filter live genomic records directly from public health repositories.
### Bioinformatics Quality Control: Built a custom QC pipeline to safely translate raw RNA nucleotides to functional proteins, drop incomplete gene fragments, eliminate machine sequencer errors (X flags), and prevent ML data leakage by pruning duplicates.
### Feature Engineering (K-mers): Transformed character-string biological sequences into a high-performance mathematical feature matrix containing 5,086 unique active biomarkers.
### Ensemble Machine Learning: Trained and optimized a 100-tree Random Forest Classifier using a strict train-test validation framework to guarantee real-world scalability.
### Model Interpretability (XAI): Extracted global feature importances to successfully reverse-engineer the "black box" model, revealing the exact 3-mer motifs driving host adaptation (MKA, VRD).

## Performance Metrics
Overall Accuracy: 98.67%
F1-Score: 0.99
Top Biomarker Discovered: MKA (Importance Score: 3.16%)
