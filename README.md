# Mccain-Rock-Detection-Team16

## Project Overview
This project aims to develop a lightweight machine vision system for detecting field rocks in potato fields. The system is intended to support on-the-go rock detection from images or video captured near a potato planter. The first-stage focus is visible rock detection, while rough size estimation and rock status tagging are treated as possible extensions.

The project also considers edge-device feasibility, such as deployment on a Raspberry Pi or a similar low-power device.

## Requirements and Priorities
The current project scope prioritises:

- visible rock detection as the core task;
- lightweight model selection for possible edge deployment;
- practical dataset preparation and annotation;
- basic evaluation of detection performance.

Rough size estimation is considered a secondary extension. Buried or partially buried rock analysis is not part of the first-stage core scope, but it may be discussed as a future improvement.

For the full MoSCoW requirement breakdown, see [MoSCoW Requirements](./MoSCoW.md).

## Current Progress
The team has started building a labelled image dataset for rock detection. The initial dataset contains field images collected from mobile phone photos, and rock bounding boxes are being annotated using Roboflow.

At the current stage, the main focus is to prepare a clean labelled dataset and train an initial object detection model.

## Team Workflow
- **Code management**: Follow the GitFlow workflow.
- **Branch convention**:
  - `main`: stable production branch
  - `develop`: main branch for daily development
  - `person name`: personal feature-development branch
- **Document collaboration**: Use Overleaf for report writing.
- **Dataset annotation**: Use Roboflow for image upload, bounding box annotation, quality checking, and dataset export.

## Repository Structure
The planned repository structure is:

.
├── data/                 # Dataset files or dataset configuration
├── notebooks/            # Experiment notebooks
├── src/                  # Source code
├── runs/                 # Training outputs
├── docs/                 # Project documents
├── MoSCoW.md             # Requirement breakdown
└── README.md             # Project overview
