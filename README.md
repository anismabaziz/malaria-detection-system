# Malaria Cell Classification using Deep Learning

A deep learning project for automated classification of malaria-infected and uninfected red blood cell images using Convolutional Neural Networks (CNN) and Transfer Learning with ResNet50V2.

## 🔬 Overview

Malaria is a life-threatening disease caused by parasites that are transmitted through the bites of infected mosquitoes. Early and accurate diagnosis is crucial for effective treatment. This project implements deep learning models to automatically classify microscopic images of red blood cells as either infected (Parasitized) or uninfected (Uninfected) with malaria parasites.

### Models Implemented

- **Custom CNN**: A convolutional neural network built from scratch
- **ResNet50V2 Transfer Learning**: Pre-trained ResNet50V2 with frozen base layers
- **ResNet50V2 Fine-tuned**: ResNet50V2 with fine-tuned top layers for domain adaptation

## 📈 Results

### Model Performance

| Model                          | Accuracy | Notes                                |
| ------------------------------ | -------- | ------------------------------------ |
| Custom CNN                     | 93.60%   | Built from scratch architecture      |
| ResNet50V2 (Transfer Learning) | 93.41%   | Pre-trained on ImageNet, frozen base |
| ResNet50V2 (Fine-tuned)        | 96.23%   | Fine-tuned top layers                |

## 🎯 Conclusion

The results demonstrate several important findings:

- The custom CNN performed surprisingly well, achieving 93.60% accuracy and slightly outperforming the initial transfer learning approach
- Basic transfer learning with ResNet50V2 achieved 93.41% accuracy, showing that pre-trained features alone weren't sufficient for this specialized medical imaging task
- **Fine-tuning was the key to success**, boosting ResNet50V2 performance to 96.23% - a significant improvement of 2.8%
- The importance of domain adaptation is clearly evident, as fine-tuning allowed the model to adapt from natural images (ImageNet) to microscopic cell images
- All models achieved over 93% accuracy, demonstrating the viability of automated malaria detection using deep learning

The fine-tuned ResNet50V2 model represents the best approach for this malaria classification task, achieving clinically relevant accuracy that could assist healthcare professionals in diagnosis. The final model size reached +200MB, making it suitable for deployment in most clinical environments.

---

**Note**: This project is for research and educational purposes. Medical diagnosis should always involve qualified healthcare professionals.
