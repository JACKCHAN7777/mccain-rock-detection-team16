# Mccain-Rock-Detection-Team16

## Project Overview
This project aims to develop a machine vision system that can run on edge devices such as a Raspberry Pi. The system is intended to be mounted behind a potato planter to enable real-time field rock detection, rough size estimation, and status tagging.

## Requirements and Priorities
The project currently prioritises visible rock detection as the core task, with lightweight model selection and edge-device feasibility treated as key design constraints. Rough size estimation is considered a secondary extension, while buried or partially buried rock analysis is not part of the first-stage core scope.

For the full MoSCoW requirement breakdown, see [MoSCoW Requirements](./MoSCoW.md).

## Repository Structure
```
├── code/                  # Jupyter notebooks for model training (Kaggle)
│   ├── yolov8s-new.ipynb
│   └── yolo26s-final.ipynb
├── LaTeX Code/            # Dissertation source files
│   └── McCain_Team16.zip
├── Paper/                 # Reference papers
├── model_reference/       # Model reference notes
└── MoSCoW.md
```

## Team Workflow
- **Code development**: All model training and experimentation is conducted on [Kaggle](https://www.kaggle.com/) using GPU notebooks. The `code/` directory contains the exported notebooks.
- **Document collaboration**: Use Overleaf for LaTeX report writing. The `LaTeX Code/` directory contains the dissertation source archive.
- **Version control**: This repository serves as the central hub for project documentation, reference materials, and code snapshots.
