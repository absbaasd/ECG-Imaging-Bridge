# Transferring Cardiac Imaging Knowledge to ECGs

**Paired Canonical Targets and Noise-Aware Diffusion**

## Code availability

**Code will be made publicly available upon publication.**

This repository currently contains a brief project overview. The implementation, trained model weights, and training configurations are not public yet.

## Overview

This project studies how paired cardiac imaging can provide training-time supervision for ECG-based prediction. Frozen ECG and imaging encoders provide representations; paired canonical correlation analysis constructs an imaging-side target space; an ECG-conditioned diffusion Bridge predicts these targets. A fixed fusion with a same-space Ridge estimate is evaluated alongside the standalone Bridge.

At inference, the transferred representation is computed from ECG alone. No patient image or imaging encoder is required for that prediction path. Generated targets are latent features, not reconstructed medical images.

## Planned release

- Target construction and preprocessing interfaces.
- Bridge training and inference implementation.
- Evaluation scripts and documented experiment configurations.
- Instructions for obtaining authorized datasets and upstream foundation-model checkpoints.

Release scope will follow the applicable data-use agreements and upstream licenses. Patient data will not be distributed through this repository.

## Status

Research in progress. This page does not announce paper acceptance or a fixed release date. Citation information and reproducibility instructions will be added with the release.
