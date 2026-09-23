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

## Repository Structure
```
├── code/                  # Jupyter notebooks for model training (Kaggle)
│   ├── yolov8s-new.ipynb
│   └── yolo26s-final.ipynb
├── LaTeX Code/            # Dissertation source files
│   └── McCain_Team16.zip
│   └── Team16_McCain_Food_Final.zip
├── Paper/                 # Reference papers
├── model_reference/       # Model reference notes
└── MoSCoW.md
```

## Team Workflow
- **Code development**: All model training and experimentation is conducted on [Kaggle](https://www.kaggle.com/) using GPU notebooks. The `code/` directory contains the exported notebooks.
- **Document collaboration**: Use Overleaf for LaTeX report writing. The `LaTeX Code/` directory contains the dissertation source archive.
- **Version control**: This repository serves as the central hub for project documentation, reference materials, and code snapshots.
