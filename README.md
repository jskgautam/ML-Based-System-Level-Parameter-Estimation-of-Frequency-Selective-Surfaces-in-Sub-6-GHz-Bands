ML-Based System-Level Parameter Estimation of Frequency Selective Surfaces in Sub-6 GHz Bands
Random Forest Regression with Physics-Aware Synthetic Data

Overview:
  This repository presents a system-level machine learning approach for parameter estimation of Frequency Selective Surfaces (FSS) operating in the sub-6 GHz band.
  A Random Forest regression model is trained on physics-aware synthetic data to learn the relationship between FSS geometry, material properties, and key frequency-domain response metrics.

The primary goal of this work is not solver-level accuracy, but to study ML behavior, interpretability, and physics consistency in RF system-level modeling.

Problem Statement:
  Full-wave electromagnetic simulation of Frequency Selective Surfaces (FSS) is computationally intensive for large parametric studies. 
  This work formulates FSS response prediction as a supervised regression problem and applies a system-level, physics-aware machine learning approach for efficient parameter estimation.

Key Features:
  Physics-aware synthetic dataset generation
  Supervised regression using Random Forest
  Prediction of multiple FSS response parameters
  Interpretability via feature importance

Dataset: The dataset is synthetically generated using heuristic, physics-inspired formulations consistent with general antenna and FSS design principles.

  Input Features:
    d_mm — FSS element size (mm)
    p_mm — periodicity (mm)
    w_mm — metallic strip width (mm)
    eps_r — substrate relative permittivity
    f_center_ghz — system center frequency (GHz)

  Target Variables:
    f_res_ghz — resonance frequency (GHz)
    BW_10dB_ghz — −10 dB bandwidth (GHz)
    S21_min_dB — minimum transmission magnitude (dB)
