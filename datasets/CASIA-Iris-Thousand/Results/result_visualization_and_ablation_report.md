
# Result Visualization and Ablation Studies

## Recognition results

The baseline model achieved **30.18%** test accuracy. The augmented-data
recognition model achieved **55.825%** test accuracy, a difference of
**25.645 percentage points**.

This is an observed comparison, not a controlled ablation: the preprocessing
pipelines differed, so the accuracy difference cannot be attributed solely
to augmentation.

## Image diversity

The previously recorded diversity score was **0.051823** for the real-image
reference sample and **0.042458** for the GAN sample. These values apply to
the reported sample and should not be generalized without repeated evaluation.

## Privacy evaluation

The exploratory membership-inference ROC-AUC was **0.550688**. This is close
to random ranking. Exact training-image membership remains unverified, so
this is not definitive evidence for or against privacy leakage.

## Ablation study status

The current notebook consolidates available results and records which
controlled comparisons remain unavailable. It does not claim that missing
ablation experiments have been performed.

## Conclusion

Existing results suggest improved recognition performance in the augmented
pipeline, but controlled experiments are needed to isolate the contribution
of each augmentation method and preprocessing choice.
