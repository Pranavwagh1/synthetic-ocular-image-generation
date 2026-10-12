## Privacy Leakage Analysis — Results

The exploratory loss-based membership inference experiment achieved a
ROC-AUC of **0.5507**, indicating **weak discrimination** between the sampled
member and held-out groups.

The mean noise-prediction MSE was **0.005886** for sampled members
and **0.007689** for held-out samples. The lower member loss
suggests a difference in model behavior, but the ROC-AUC indicates that
this signal has limited discriminative power.

### Limitations

The available image-level CSV contains all 2,000 identities in each of
the train, validation, and test splits. It does not independently verify
the exact images used to train the identity-conditioned diffusion model.
Therefore, this experiment must be described as exploratory, not as
definitive evidence of privacy leakage.

The best threshold accuracy was selected and evaluated on the same samples,
so it is not an independent estimate of attack performance. A stronger
evaluation would require verified training membership, a controlled
member/nonmember protocol, and an independent test set for attack evaluation.

### Conclusion

These results provide an initial assessment of loss-based privacy signals
in the ocular diffusion model. They do not establish either the presence
or absence of significant privacy leakage. Further controlled evaluation
is needed before drawing stronger privacy conclusions.