# Clinical NLP — Uncertainty-Aware Specialty Routing

## Overview
A clinical NLP system that classifies unstructured medical notes 
into medical specialties — and signals when it shouldn't be trusted.

Built for MSBX 5425 — NLP for Healthcare Analytics, University of 
Colorado Leeds School of Business.

## Research Question
Can we build a model that not only routes clinical notes to the 
right medical specialty, but also reliably signals when it 
shouldn't be trusted?

## Approach
- Fine-tune ClinicalBERT on MTSamples medical transcriptions
- Apply conformal prediction to output uncertainty-aware 
  prediction sets instead of single confident answers
- Use embedding space density to flag outlier patients
- Stress test with noise injection and synthetic hard cases

## Dataset
MTSamples — 3,743 clinical transcriptions across 18 specialties  
Source: https://www.kaggle.com/datasets/tboyle10/medicaltranscriptions

## Tech Stack
- Python, PyTorch, HuggingFace Transformers
- ClinicalBERT (emilyalsentzer/Bio_ClinicalBERT)
- scikit-learn, UMAP, scispaCy
- Conformal prediction (MAPIE)

## Project Structure
coming soon

## Authors
[Your name] and [Partner name]  
University of Colorado Boulder, 2026
