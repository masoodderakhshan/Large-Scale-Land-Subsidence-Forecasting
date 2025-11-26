# Large-Scale Land Subsidence Forecasting with InSAR and Environmental Variables

[![Status](https://img.shields.io/badge/Status-Submitted-blue)](https://www.springer.com/journal/11069)
[![Journal](https://img.shields.io/badge/Journal-Natural%20Hazards-orange)](https://www.springer.com/journal/11069)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## 📌 Abstract
Land subsidence, primarily caused by unsustainable groundwater extraction, is a growing geohazard in many regions worldwide. Effective mitigation requires accurate, large-scale predictive models.

This repository contains the source code and implementation details for the paper **"Large-Scale Land Subsidence Forecasting with InSAR and Environmental Variables via Machine Learning Approaches"**, submitted to the *Natural Hazards* journal.

The study focuses on 8 key regions in Iran, utilizing Multi-source geospatial data (Sentinel-1 InSAR, GLDAS, ISRIC) to train **ElasticNet**, **LightGBM**, and **BiLSTM** models. The framework demonstrated high accuracy, with **ElasticNet** achieving an $R^2$ of 0.95 and RMSE of 5.21 mm on unseen test regions.

## 👥 Authors

* **Amirreza Shahmiri**
    * *Department of Civil and Architectural Engineering, Sultan Qaboos University, Muscat, Oman*
    * [![ORCID](https://img.shields.io/badge/ORCID-0009--0002--0746--3887-green)](https://orcid.org/0009-0002-0746-3887)
* **Masoud Ebrahimi Derakhshan**
    * *School of Civil Engineering, Iran University of Science and Technology (IUST), Tehran, Iran*
    * [![ORCID](https://img.shields.io/badge/ORCID-0009--0009--3453--8304-green)](https://orcid.org/0009-0009-3453-8304)
* **Seyed Mostafa Siadatmousavi** (Corresponding Author)
    * *School of Civil Engineering, Iran University of Science and Technology (IUST), Tehran, Iran*
    * [![ORCID](https://img.shields.io/badge/ORCID-0000--0002--0068--7506-green)](https://orcid.org/0000-0002-0068-7506)

## 📂 Repository Contents

The source codes are provided as text files for accessibility, reflecting the current repository structure:

### 1. Model Implementations
Code for the ML/DL models, categorized by forecasting steps:

* **ElasticNet:** `ElasticNet_Step1.txt`, `ElasticNet_Step1&2...txt`, `ElasticNet_3Step_S...txt`
* **LightGBM:** `LightGBM_Step1.txt`, `LightGBM_Step1&2&...txt`
* **BiLSTM:** `BiLSTM_1Step.txt`, `Bi_LSTM_3Step.txt`
* **Core Configs:** `Core_Model_1STP.txt`, `Core_model_DS.txt`

### 2. Visualization & Analysis
* `Plot-8-Location.txt`: Study area mapping.
* `Plot-Disp.txt`: InSAR displacement plotting.
* `BARDSIR.txt`: Region-specific data/script for Bardsir case study.

## 🚀 Usage

1.  Open the desired model file (e.g., `ElasticNet_Step1.txt`).
2.  Copy the content into your Python environment (or save as `.py`).
3.  Ensure required libraries (Scikit-learn, TensorFlow/PyTorch, LightGBM) are installed.
4.  Run the script to reproduce the forecasting results.

## 📊 Performance Summary

The **ElasticNet** model outperformed other architectures on the test dataset:

| Model | $R^2$ Score | RMSE (mm) | MAE (mm) |
| :--- | :---: | :---: | :---: |
| **ElasticNet** | **0.95** | **5.21** | **3.81** |
| LightGBM | *[See Paper]* | *[See Paper]* | *[See Paper]* |
| BiLSTM | *[See Paper]* | *[See Paper]* | *[See Paper]* |

## 📜 Citation

If you use this code or dataset in your research, please cite our paper:

```bibtex
@article{Shahmiri2025Subsidence,
  title={Large-Scale Land Subsidence Forecasting with InSAR and Environmental Variables via Machine Learning Approaches},
  author={Shahmiri, Amirreza and Ebrahimi Derakhshan, Masoud and Siadatmousavi, Seyed Mostafa},
  journal={Natural Hazards},
  year={2025},
  note={Submitted}
}
