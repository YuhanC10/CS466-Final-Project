# Nussinov Algorithm for RNA Secondary Structure Prediction

This Jupyter notebook implements and evaluates the Nussinov algorithm for predicting RNA secondary structures using dynamic programming.

## Overview

The Nussinov algorithm predicts RNA base pairing by maximizing the number of valid base pairs (A-U, G-C) in a sequence. This implementation includes both the standard algorithm and an improved version with minimum loop length constraints.

## Contents

1. **Environment Setup** - Import dependencies (NumPy, Matplotlib, HuggingFace datasets)
2. **Data Loading** - Load and analyze the ArchiveII RNA dataset
3. **Algorithm Implementation**
   - DP matrix filling phase (O(n³) time, O(n²) space)
   - Traceback phase for structure reconstruction
   - Improved version with configurable minimum loop length
4. **Evaluation**
   - Synthetic dataset testing (perfect hairpins, bulged hairpins)
   - ArchiveII dataset evaluation (3,854 sequences)
   - Metrics: Sensitivity, Precision, F1 score
5. **Complexity Verification** - Empirical validation of O(n³) time and O(n²) space complexity

## Dependencies

- numpy
- matplotlib
- datasets (HuggingFace)
- scipy

## Author

Yuhan Cui (yuhanc10) - CS466 Final Project
