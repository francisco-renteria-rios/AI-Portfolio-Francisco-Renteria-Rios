## GitHub Project Link:
## VQA Assistance 
https://github.com/francisco-renteria-rios/VQA_Assistance.git

## VQA_Grocery_Assistant_App.ipynb from Google Colab
https://colab.research.google.com/drive/1Qet23wIEAw0ce-2Ca1CiFCQO0SqdeMpl?usp=sharing

## VizWiz
https://vizwiz.org/tasks-and-datasets/

## Huggingface
https://huggingface.co/

## Dataset Handling
Dataset: VizWiz
The dataset VizWiz is a public dataset that can be access through Hugging Face or from the VizWiz website.

## Visual Question Answering System project - ITAI 1378 Computer Vision and AI By Francisco Renteria Rios

Problem Statement
The difficulty visually impaired individuals face when attempting to read the grocery labels, make them make mistakes when choosing store items. Their actions can have health consequences. This project demonstrates a Visual Question Answering (VQA) system designed to help visually impaired users understand grocery labels and small print documents. It is important to support people with visual disabilities and make them more independent by inclusion using technology.

Solution Overview
A Visual Question Answering (VQA) system takes an image and a question about that image, then generates an answer. For example, this system can be an app in a smart phone. The user ask a question, “Does this contain nuts?” They system then “sees” the label, understand the text, and gives the specific answer to the question, “Yes, the ingredient list includes almonds and peanuts”. This system empowers visually impaired users to shop, choose, and eat safely.

Technical Approach Model
Pre-trained BLIP-2 model (Bootstrapped Language Image Pretraining). BLIP-2 has an excellent balance of performance, efficiency, and strong reasoning capability.
Framework: PyTorch or TensorFlow for deep learning
Platform: Google Colab
EasyOCR reader

Dataset Plan Source
Public dataset (VizWiz-VQA). It is a free public dataset. It can be access through Hugging Face, Kaggle, or the official VizWiz website. (VizWiz dataset was created specifically for visually impaired people). Size: WizWiz contains over 31,000 image/question pairs.

Labels
Visual Data is already labeled. What we are looking in the future is the check if a specific ingredient is in a product.

Preparation
The dataset already contains labeled data. Although the data contains images with poor quality to represent a real world scenario. We will use only download a subset of the first 100 entries from Hugging Face.

Metrics
Average Normalized Levenshtein Similarity (ANLS): it measures how similar the predicted text is to the correct text. Answerability Prediction (this is a crucial metric drawn from the VizWiz dataset): The system must first decide if the question is even answerable from the image (e.g., the label is blurry, cut off, or doesn't contain the info). Optical Character Recognition (OCR) Metrics: The VQA's performance is capped by its ability to read.

The application will download 10 sample images and make prediction based on predefined questions. It is true that VizWiz are not exclusevely grocery items labels, the images will be tested for their question/answer results. Initially, I plan to have static predictions, but a future plan would be a random lable image taken from a phone.

Week-by-Week Plan
Week Task Milestone 10 (Oct 30) Get dataset, set up environment Dataset ready 11 (Nov 6) Train or fine-tune model Model working 12 (Nov 13) Test and improve Good accuracy 13 (Nov 20) Create demo / video Demo ready 14 (Nov 27) Final testing / documentation Everything done 15 (Dec 4) Present project Presentation day

Resources needed Resource Options / Notes
Compute Google Colab, VizWiz-VQA, Heidi Frameworks Pytorch Estimated Cost $0.00

Risks Probability Mitigation System fails to answer correctly Medium Fine-tuning Poor image quality Medium This condition reflects real world-sitautions
