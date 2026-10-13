# Notebook 14 — Visualization and Ablation-Style Findings

## Recognition results

- Original-only test accuracy: 0.0068807339449541
- Original + traditional augmentation test accuracy: 0.0229357798165137
- Original + GAN exploratory test accuracy: 0.0045871559633027

These experiments are not a controlled ablation: training budgets and prior configurations differ, and Notebook 10 used two epochs per experiment.

## Membership inference

The evaluated confidence/loss attack AUC values were near 0.5 on the sampled data. This does not establish absence of privacy leakage.

## Interpretation limitations

- Low-level image statistics do not prove perceptual quality or identity preservation.
- GAN conditioning labels are not verified biometric identity labels.
- The generated-image sample sizes differ.
- No formal multi-seed or matched-compute ablation was performed.

## Generated outputs

- IITD_recognition_comparison.png
- IITD_image_statistics_comparison.png
- IITD_membership_attack_auc_comparison.png
- IITD_final_recognition_summary.csv
- IITD_final_membership_attack_summary.csv
- IITD_notebook14_consolidated_summary.json
