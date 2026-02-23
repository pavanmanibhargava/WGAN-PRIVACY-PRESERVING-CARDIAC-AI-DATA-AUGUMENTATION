# WGAN-PRIVACY-PRESERVING-CARDIAC-AI-DATA-AUGUMENTATION

**Module 1 — Data Pipeline & Preprocessing**

Builds a robust ECG data pipeline from raw public/hospital datasets to clean, fixed-length segments for WGAN training. Includes lead selection, resampling, segmentation, filtering (0.5–40 Hz), noise removal, and normalization.

Supports labeled rhythms (e.g., NSR, AF, PVC) and structured train/validation/test splits.

Outputs: Clean ECG tensors and preprocessing scripts (ecg_data_loader.py, preprocess_ecg.py, data_config.yaml).

**Module 2 — WGAN Architecture for ECG**

Implements a 1D Wasserstein GAN for realistic ECG signal generation. Includes a generator for synthetic ECG segments and a critic for distribution learning. Designed for stable training and extensibility to conditional ECG generation.

**Module 3 — Training Engine (WGAN / WGAN-GP)**

Handles adversarial training with Wasserstein loss and optional Gradient Penalty (WGAN-GP) for improved stability. Supports configurable hyperparameters, checkpointing, and training monitoring.

**Module 4 — Evaluation & Quality Assessment**

Evaluates synthetic ECG quality using statistical similarity, signal morphology comparison, and downstream classifier performance. Ensures realism, diversity, and clinical relevance.

**Module 5 — Deployment Layer (API + UI)**

Provides an API for synthetic ECG generation and a lightweight UI for visualization. Enables controlled data generation for research and privacy-preserving AI applications.

**Module 6 — Monitoring, Versioning & Continuous Improvement**

Implements model versioning, experiment tracking, and performance monitoring. Supports iterative improvement through retraining, evaluation, and controlled deployment updates.
