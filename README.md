# Handwritten Letter and Word Recognition Using Vision Transformers
### Description
This project explores the use of Vision Transformers (ViT) for handwritten character recognition, comparing their performance to a Convolutional Neural Network (CNN) baseline. The task involves classifying 62 classes — uppercase letters (A–Z), lowercase letters (a–z), and digits (0–9) — using transfer learning on a small dataset.

If time allows, the project will be extended to full word recognition using sequence-based methods.

#### Features
Fine-tunes a pretrained ViT (vit-base-patch16-224) from HuggingFace.

Trains a CNN baseline for comparison.

Supports data augmentation (rotation, scaling, noise).

Evaluates models using accuracy, precision, recall, F1-score, and confusion matrices.

Optionally extends to word-level recognition.

#### Visuals
(Optional – You can add screenshots or sample output images here later)

#### Installation
Requirements
Python 3.10+

NVIDIA GPU (RTX 4060 or similar recommended)

Kaggle API access to download the dataset or dataset zipped file.

Steps
bash
Copy
Edit
## Clone the repository
git clone https://gitlab.ecs.vuw.ac.nz/jiaziru/aiml-339-project.git
cd aiml-339-project

## Install dependencies
pip install -r requirements.txt

## Download dataset from Kaggle
kaggle datasets download -d dhruvildave/english-handwritten-characters-dataset
unzip english-handwritten-characters-dataset.zip -d data/
#### Usage
Train ViT Model
bash
Copy
Edit
python src/train_vit.py
Train CNN Model
bash
Copy
Edit
python src/train_cnn.py
Evaluate Models
bash
Copy
Edit
python src/evaluate.py
#### Roadmap
Implement ViT fine-tuning

Implement CNN baseline

Add word-level recognition with CTC decoding

Experiment with additional datasets

#### Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss the proposed update.
Make sure to test your changes and follow the existing coding style.

#### Authors
Zirui Jia – Victoria University of Wellington
Email: steven5115115@gmail.com

#### License
This project is for academic purposes under AIML 339.
Dataset and pretrained model usage are subject to their respective licenses:

Dataset: Kaggle License

Model: HuggingFace ViT License
