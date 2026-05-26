# STOLEN-MODEL-DETECTION-VIA-MULTI-SIGNAL-SIMILARITY-SCORING
Open and run `tmla2.ipynb` end-to-end. It will:
- Load the target model and 360 suspect models
- Compute three similarity signals per suspect model:
  - Weight-space cosine similarity (weight 0.4)
  - Prediction-space cosine similarity (weight 0.4)
  - CKA representation similarity (weight 0.2)
- Min-max normalize scores to [0, 1]
- Save results to `submission.csv`

- ### 5. Output
A `submission.csv` file with columns `id` (0–359) and `score` (stealing
confidence). Higher score = more likely stolen.
