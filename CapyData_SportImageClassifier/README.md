# CapyData_Sport Action Image Classifier

## Project Overview
This project focuses on developing an image classification model specifically for sports-related images. The objective is to accurately identify the type of sport depicted in each image using deep learning techniques. The model aims to recognize a variety of sports based on visual cues such as players' attire, equipment, and environment. 

## Objectives
1. Collect and curate a dataset of sports images.
2. Preprocess and annotate the dataset with gold output sport name.
3. Develop an image classifier model using deep learning.
4. Evaluate model performance and improve caption quality.
5. Update to the main project: Sport Action Image Captioning.


## Project Organization
```
📂 CapyData_ImageCaptioning
│   ├── 📂 app/
│   ├── 📂 data/
│   │   ├── 📂 metadata/
│   │   ├── 📂 raw_images/
│   │   ├── 📂 raw_photos/
│   │   ├── 📄 captions.txt
│   ├── 📂 models/
│   ├── 📂 notebooks/
│   │   ├── 📂 dataset/
│   │   │   ├── 📄 1_data_collection.ipynb
│   │   │   ├── 📄 2_pinterest_crawler.ipynb
│   │   │   ├── 📄 3_data-annotation_openai.ipynb
│   │   ├── 📄 descriptions.txt
│   ├── 📂 scripts/
│   ├── 📂 src/
│   │   ├── 📄 descriptions.txt
│   │   ├── 📄 preprocessing.py
│   ├── 📄 LICENSE
│   ├── 📄 README.md
│   ├── 📄 requirements.txt
```

## Getting Started
To set up and run this project locally, follow these steps:

1. Clone the repository:
```bash
git clone https://github.com/your-repo/sports-captioning.git
cd sports-captioning
```

2. Set up the environment:
```bash
conda create -n captioning-env python=3.9 -y
conda activate captioning-env
```

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

4. Run the notebooks:
Open the Jupyter notebooks in the `notebooks/` folder to view and run model training and evaluation steps.

## Evaluation Metrics
- Data Quality Metrics:
    - Caption length distribution
    - Vocabulary diversity
    - Word frequency analysis
    - Image quality checks
- Model Performance Metrics:
    - BLEU, ROUGE (n-gram-based)
    - BERTScore (semantic similarity)
    - Distinct-n (caption diversity)
    - Human Evaluation

## Modeling Approaches

Four different approaches were considered for training the model:

1. Traditional Pipeline:
- CNN + LSTM (Show and Tell model)

2. Attention-Based Pipeline:
- CNN + LSTM + Attention (Show, Attend and Tell)

3. Transformer-Based Pipeline:
- CNN/ViT + Transformer (e.g., BART, T5)

4. Modern Pretrained Models:
- Encoder: CLIP, Oscar, ViT
- Decoder: GPT/Vision-Language Transformers
- Fine-tuning models like BLIP-2 or multimodal architectures

## How to Contribute

If you want to contribute to this project, follow these steps:
1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Create a pull request with a detailed explanation of your changes.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute it with proper attribution.

## Group's Resources (Timeline, Meeting notes, Docs)
- [Project Drive](https://drive.google.com/drive/u/0/folders/1bOzHSAkUOj7Zp-7Flf7NnK-F441BHmwe).

## Contributors
This project is done by the Capydata group, University of Science, VNU-HCM.

| Student ID | Name                   |
|------------|------------------------|
| 22127234   | Cao Hoàng Lộc          |
| 22127360   | Võ Nguyễn Phương Quỳnh |
| 22127440   | Phan Võ Minh Tuệ       |
| 22127450   | Phạm Anh Văn           |