# C-TIRADS Ultrasound Classification of Thyroid Nodules via Contrastive Learning Integrated with Clinical Data

This repository implements the deep learning model **ThyroVision** from the paper:  
*"C-TIRADS Ultrasound Classification of Thyroid Nodules via Contrastive Learning Integrated with Clinical Data"*.

ThyroVision combines thyroid ultrasound images with clinical features (age, gender, nodule count, three‑dimensional size) and leverages Supervised Contrastive Learning (SCL) for fine‑grained C‑TI‑RADS classification (five‑category and seven‑category).

## Main Dependencies

- Python 3.8+
- PyTorch 1.13+
- CUDA 11.7 (if using GPU)

Full dependencies are listed in `requirements.txt`.

# Dataset Preparation

1. The raw data should include:
   - Thyroid nodule ultrasound images (`.png` or `.jpg`)
   - A clinical information table (`.xlsx` or `.csv`) containing the following fields:  
     `image_path`, `Age`, `Gender`, `Nodules_num`, `Nodule_size_length`, `Nodule_size_wide`, `Nodule_size_depth`, `labels`
2. Place all images into `data/images/` and the clinical table into `data/clinical.csv`.

