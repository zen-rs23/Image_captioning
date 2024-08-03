# Image Captioning with Deep Learning

## Overview

This project, led by Rohit Sharma, focuses on developing an image captioning system that generates descriptive text for images. The system leverages deep learning models, combining Convolutional Neural Networks (CNNs) for feature extraction and Recurrent Neural Networks (RNNs) with Long Short-Term Memory (LSTM) units for caption generation. The Flickr8k dataset, which includes 8,000 images paired with five captions each, served as the primary dataset for this project.

## Dataset

**Flickr8k**: A diverse dataset with 8,000 images and five captions per image, providing a rich variety of scenes and objects. The captions offer multiple perspectives, enabling robust training and evaluation of the image captioning model.

## Methodology

### Feature Extraction

We used pre-trained CNNs to extract visual features from images:
- **ResNet50**
- **VGG16**
- **GoogLeNet**
- **MobileNetV2**

These models were fine-tuned for the specific task of image captioning.

### Caption Generation

The caption generation component used LSTM networks to produce textual descriptions based on the extracted features. Key steps included:
- Tokenization and embedding of captions
- Use of start and end tokens for sentence generation
- Application of dropout for regularization

### Training and Evaluation

The model was trained and evaluated using BLEU scores, a standard metric for assessing the quality of generated text. The evaluation involved BLEU-1 to BLEU-4 scores, which measure the precision of unigrams, bigrams, trigrams, and four-grams, respectively.

## Results

- **ResNet50:** BLEU-1: 0.1379, BLEU-2: 0.0341, BLEU-3: 0.0225, BLEU-4: 0.0192
- **VGG16:** BLEU-1: 0.1617, BLEU-2: 0.0371, BLEU-3: 0.0246, BLEU-4: 0.0208
- **GoogLeNet:** BLEU-1: 0.1438, BLEU-2: 0.0344, BLEU-3: 0.0228, BLEU-4: 0.0191
- **MobileNetV2:** BLEU-1: 0.1469, BLEU-2: 0.0346, BLEU-3: 0.0222, BLEU-4: 0.0183

## Key Findings

The project demonstrated the effectiveness of using deep learning techniques for image captioning, with VGG16 showing the best performance among the models tested. The generated captions were evaluated for accuracy and contextual relevance, highlighting the challenges in generating coherent and contextually accurate longer sentences.

## Future Work

Future enhancements may include:
- Fine-tuning models with more epochs and different optimizers
- Exploring advanced architectures like Transformers for improved caption generation
- Implementing ensemble methods to combine predictions from multiple models

## Conclusion

This project successfully developed an image captioning system that integrates computer vision and natural language processing techniques. As the project lead, I coordinated the team's efforts to ensure a cohesive approach to the technical challenges, resulting in a robust and effective model.

## Contact

For inquiries, please contact [Rohit Sharma](https://www.linkedin.com/in/rohit-sharma-2459096002/).
