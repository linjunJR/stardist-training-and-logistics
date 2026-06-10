# StarDist Training and Logistics

A collection of Jupyter notebooks for creating labelled data and training StarDist models to track photoelastic disks.

See the original [StarDist](https://stardist.net/) website for more info on the model and its training.

See the [TPE project documentation](https://linjunjr.github.io/TPE_Disk_Image_Processing/) for detailed methods and usage of the notebooks

## Overview

This workflow assumes you have some sub-optimal tracking results at hand, and is seeking to improve the accuracy with stardist. 
The repository contains three sequential notebooks:
- **`manual_refine_GUI.ipynb`** lets you clean and correct existing tracking results via an interactive GUI, so the model doesn't learn from inaccurate data
- **`mask_generator.ipynb`** prepares the data format that stardist requires
- **`TRAINING_stardist_disk_finder.ipynb`** is the actual training pipeline, largely adated from the official [StarDist tutorial](https://github.com/stardist/stardist/tree/main/examples/2D)

## Requirements

- Python 3.x
- StarDist
- TensorFlow/PyTorch
- Jupyter Notebook
- OpenCV, NumPy, and other standard scientific Python packages


