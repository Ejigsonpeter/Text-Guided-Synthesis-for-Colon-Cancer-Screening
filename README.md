# Text-Guided-Synthesis-for-Colon-Cancer-Screening

## Overview
This project addresses the critical challenge of data scarcity in AI-assisted colonoscopy by developing an efficient strategy for generating synthetic colonoscopy image data. While existing works have utilized various generative models (GANs, DALL-E 2, Midjourney, Imagen, LDM, and VQ-GAN), our approach uniquely applies fine-tuned Visual Language Models (VLMs) specifically for colonoscopy data generation, enabling intelligent data augmentation for improved cancer screening.

## Key Findings
- **Image Generation Performance**: Stable Diffusion (SD) and DreamBooth LoRa achieved a consistent average Inception score of 2.36 across three datasets, indicating high authenticity of generated images
- **Classification Results**:
  - ViT and DeiT: 93% accuracy
  - BiT: 92% accuracy
  - FixResNeXt: 91% accuracy
  - EfficientNet: 86% validation accuracy
- **Segmentation Performance** (using SAM-generated masks):
  - FPN achieved best results:
    - IoU: 0.64
    - F1-score: 0.72
    - Recall: 0.87
    - Dice Coefficient: 0.72

## Features
- Text-to-image synthesis using fine-tuned Visual LLMs
- Integration with Stable Diffusion and DreamBooth LoRa
- Multiple classification model implementations (ViT, DeiT, BiT, FixResNeXt, EfficientNet)
- Segmentation model implementations (U-Net, PSNet, FPN, LinkNet, MANet)
- SAM integration for mask generation
- Comprehensive evaluation framework

## Prerequisites
- Python 3.8+
- PyTorch
- Stable Diffusion dependencies
- DreamBooth requirements
- SAM (Segment Anything Model) dependencies
- Additional dependencies (listed in requirements.txt)


## Model Architecture

### Image Generation
- Fine-tuned Visual LLMs
- Stable Diffusion implementation
- DreamBooth LoRa adaptation

### Classification Models
- Vision Transformer (ViT)
- Data-efficient Image Transformer (DeiT)
- Big Transfer (BiT)
- FixResNeXt
- EfficientNet

### Segmentation Models
- U-Net
- PSNet
- Feature Pyramid Network (FPN)
- LinkNet
- MANet

## Evaluation Metrics
- Inception Score for generated images
- Classification accuracy
- Segmentation metrics:
  - Intersection over Union (IoU)
  - F1-score
  - Recall
  - Dice Coefficient

## Dataset
The project utilizes three datasets for comprehensive evaluation:
1. Development Dataset: [Google Drive](https://drive.google.com/file/d/1bZ27-A3RLTYot65swbtu0A3p4O9Asp0-/view)
2. Testing Dataset: [Google Drive](https://drive.google.com/file/d/1WGmSUHog2-vTlu0hKx97jVL8VZwQI06J)
3. Generated synthetic dataset using our approach

## Contributing
We welcome contributions! Please follow these steps:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## Credits
- Image Evaluation Code: [ImageCLEFmed-MEDVQA-GI-2024](https://github.com/simula/ImageCLEFmed-MEDVQA-GI-2024)
- CLEF Dataset: Provided through the ImageCLEF initiative
- SAM (Segment Anything Model): Meta AI Research

## License
[Insert your chosen license here]

## Citation
```bibtex
@inproceedings{Peter2024AdvancingAM,
  title={Advancing AI-Powered Medical Image Synthesis: Insights from MedVQA-GI Challenge Using CLIP, Fine-Tuned Stable Diffusion, and Dream-Booth + LoRA},
  author={Ojonugwa Oluwafemi Ejiga Peter and Md Mahmudur Rahman and Fahmi Khalifa},
  booktitle={Conference and Labs of the Evaluation Forum},
  year={2024},
  url={https://api.semanticscholar.org/CorpusID:271772323}
}
```

## Contact
Email:ejigsonpeter@gmail.com
