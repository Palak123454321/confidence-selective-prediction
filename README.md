# Evaluating Confidence-Based Selective Prediction Under Controlled Distribution Shifts

## Research Question

How does confidence-based selective prediction behave when a classifier is evaluated under controlled distribution shifts?

## Overview

This project evaluates confidence-based selective prediction using a SmallCNN trained on CIFAR-10.

The experiment studies:

- Gaussian noise
- Gaussian blur
- Brightness shift
- Rotation

under multiple severity levels.

Two selection policies are compared:

1. Fixed confidence threshold
2. Coverage-controlled threshold calibrated on clean data

Confidence calibration is additionally studied using temperature scaling.

## Dataset

CIFAR-10:

- 45,000 training samples
- 5,000 calibration samples
- 10,000 test samples

## Evaluation Metrics

- Accuracy
- Coverage
- Selective Accuracy
- Selective Risk
- Risk-Coverage Curve
- AURC
- ECE

## Project Structure

```text
src/        Source code
tests/      Unit tests
data/       Local datasets
models/     Local model checkpoints
results/    Experimental results
paper/      Research paper
notebooks/  Exploratory notebooks