# Predicting peritumoral glioblastoma infiltration and subsequent recurrence using deep learning-based analysis of multi-parametric magnetic resonance imaging

This github repository contains the Python implementatino of the following paper submission: Kwak, S. et al., "Predicting peritumoral glioblastoma infiltration and subsequent recurrence using deep learning-based analysis of multi-parametric magnetic resonance imaging" Journal of Medical Imaging. 

## How to use

For this version of code, Python 3.9.7 or above is required. Required python packages can be installed by using `requirements.txt`. Once can be installed by running 

`pip install -r requirements.txt`

#### Requirements

Code is assumed user has access to MRI scans (FLAIR, T1, T1CE, T2, and ADC), ROIs (Far, and Near), and brain tumor segmentatino.

#### Usage

Please run code in following order:
1) `Infiltrative_ROI/`: `Near_far_selection.ipynb` -> `Near_far_patchMaking.ipynb` -> `Training_NearFar.ipynb` -> `Testing_nearFar_byInst.ipynb` -> `Post_processing.ipynb`
2) `Noninfiltrative_ROI/`: `Create_Non_infiltrative_ROI.ipynb`
3) `Evaluation map/`: `Create_eval_map.ipynb`
4) `Main/`: `Training.ipynb` -> `Testing_InfiltrativeNoninfiltrative.ipynb` -> `Post_processing.ipynb`

Make sure put appropriate input and output directory as suggested.



