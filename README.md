# An Exhaustive Five-by-Five Classification for an Induced Ordered Binary Pattern

Ryutaro Yonezu — Independent Researcher  
No.51 · Version 1.0 · 3 November 2026 · Preprint

For the induced ordered binary pattern H=001/010/111, this limited computer-assisted study compares the minimum number tau_H of cells meeting every existing occurrence with the minimum number D_H of cell flips needed to make a matrix H-free. The exhaustive enumeration of all 33,554,432 binary 5-by-5 matrices records exactly 153 matrices with D_H>tau_H, all with (tau_H,D_H)=(1,2). Exhaustive verification through square order four shows that five is the smallest separating square order. The accompanying archive contains the enumerator, the full 153-code list, recorded counts, Python checkers, proofs, bibliographic notes, and SHA256 hashes.

The principal contribution is this exact finite classification for one fixed 3-by-3 pattern. The direct-sum consequence is elementary and is not claimed as new or as a nonpolynomial removal lower bound. Wang, arXiv:2610.15370, gives a stronger prior separation for another pattern. The complete proof of OpenAI Math #190 was not independently audited here. No minimality claim is made for all rectangular matrices.

Status: Preprint; not human peer-reviewed. Novelty: INCONCLUSIVE. Rights: All rights reserved. Prior independent AI audit: MODEL / PROOF / COMPUTATION PASS; MINIMALITY PASS for square order only. AI auditing is not a substitute for human peer review.

## Publication

- [Zenodo Preprint — DOI 10.5281/zenodo.23919060](https://doi.org/10.5281/zenodo.23919060)
- [Zenodo record](https://zenodo.org/records/23919060)
- [GitHub Release v1.0](https://github.com/yonezaemon1-hub/no51-five-by-five-ordered-binary-pattern/releases/tag/v1.0)

## Files and reproduction

- [Paper PDF](https://github.com/yonezaemon1-hub/no51-five-by-five-ordered-binary-pattern/releases/download/v1.0/No51_v1.0_PREPRINT_20261103.pdf)
- [Reproducibility ZIP](https://github.com/yonezaemon1-hub/no51-five-by-five-ordered-binary-pattern/releases/download/v1.0/No51_v1.0_REPRODUCIBILITY_20261103.zip)

The archive's frozen_v0.3/ directory preserves the audited historical snapshot, including its historical HOLD wording. The current release is v1.0. Do not alter the frozen files.

From frozen_v0.3/, run Python 3.10+ with the standard library:

```text
python -I check_hashes.py
python -I verify_no51.py
python -I verify_153_independently.py
```

The 153-witness Python check does not establish completeness by itself. For completeness, use exhaustive_5x5.c. Run the C enumerator only in a separate working copy: it overwrites separating_5x5.txt. Compare its output against the frozen list and recorded counts.

## Checksums

```text
e7ecb7ed79737d2b9499d54e31f26daff4bac10bd959d8492899b8ae9c981ae7  No51_v1.0_PREPRINT_20261103.pdf
9a5d227b36fc6a9e099f8fe5b874acfbc75afe957e377175145161add1070cfe  No51_v1.0_REPRODUCIBILITY_20261103.zip
```
