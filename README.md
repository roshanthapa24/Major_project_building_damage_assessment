# Building Damage Assessment Using Satellite Imagery

A deep learning-based system for automated building damage assessment using satellite imagery. This project uses pre and post-disaster satellite images to classify and localize building damage caused by natural disasters.

---

## Project Overview

Natural disasters like earthquakes, floods, and volcanic eruptions cause massive building damage. Manual assessment is slow and dangerous. This project automates damage detection using Satellite imagery and state-of-the-art deep learning models to speed up disaster response and recovery efforts.

---

## Features

- Pre and post-disaster image comparison
- Automated building damage detection and segmentation
- Multiple model implementations (Detectron2, DETR, SAM, ChangeFormer)
- Semantic segmentation of damaged regions
- Evaluation metrics for model performance

---

## Models Used

| Model | Purpose |
|-------|---------|
| Detectron2 | Instance segmentation of buildings |
| DETR (Detection Transformer) | Object detection on custom dataset |
| SAM (Segment Anything Model) | Building segmentation |
| ChangeFormer | Change detection between pre/post disaster |

---

## Dataset

- **xBD Dataset** — large-scale dataset for building damage assessment
- **xView Dataset** — overhead imagery dataset
- Images include pre-disaster and post-disaster satellite scenes
- Annotations in COCO format

---

## Tech Stack

- Python
- PyTorch
- Detectron2
- Hugging Face Transformers
- Google Colab
- OpenCV
- NumPy / Pandas
- Tensorboard

---

## Project Structure

```
├── notebooks/
│   ├── detectron2_postDisaster.ipynb
│   ├── detectron2_preDisaster.ipynb
│   ├── finetune_detectron2_post.ipynb
│   ├── finetune_detectron2_pre.ipynb
│   ├── Detr_implementation.ipynb
│   ├── Detr_custom_dataset.ipynb
│   ├── Fine_tuning_DetrForObjectDetection.ipynb
│   ├── semantic_segmentation_xBD_dataset.ipynb
│   ├── NB_create_xview_data.ipynb
│   ├── xView_baseline_model.ipynb
│   └── annotation_formatter.py
├── configs/
│   ├── config.yaml
│   └── 1_pre_config.yaml
├── main.py
├── aimodel_pre.py
└── req.txt
```

---

## Installation

```bash
git clone https://github.com/roshanthapa24/Major_project_building_damage_assessment.git
cd Major_project_building_damage_assessment
pip install -r req.txt
```

---

## Usage

1. Open any notebook in the `notebooks/` folder using Google Colab
2. Mount your Google Drive
3. Follow the steps inside each notebook

---

## Team

- Roshan Thapa
- Gaurav Shah
- Roshan Ojha
- Yogesh Pant 

---

## Acknowledgements

- [xView2 Dataset](https://xview2.org/)
- [Detectron2 by Facebook AI](https://github.com/facebookresearch/detectron2)
- [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything)
- [ChangeFormer](https://github.com/wgcban/ChangeFormer)
