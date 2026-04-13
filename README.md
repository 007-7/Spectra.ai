# Spectra.ai

An AI-powered video detection platform that analyzes uploaded videos to determine whether they are AI-generated or authentic. The system returns a confidence score for each prediction and supports interactive, LLM-based explanations of its outputs.

trained deep neural networks on a dataset of 50,000+ real and AI-generated frames, utilizing spatio-temporal analysis to achieve a 99.7% detection accuracy. 

## Model

- **Architecture:** EfficientNet-B4 (convolutional neural network)
- **Task:** Binary classification — Real vs. AI-generated video
- **Validation Accuracy:** 99.7%

## Dataset

- **Total frames:** 50,000
- **Real frames:** 25,000
- **AI-generated frames:** 25,000 (sourced from Pika, Sora, and T2VZ)

## Capabilities

- Frame-level inference with confidence scoring
- Difficulty-tiered evaluation (high / mid / low) based on human distinguishability
- Ensemble configuration: EfficientNet-B4 (0.5) + EfficientNet-B3 (0.3) + ResNet50 (0.2)
- Interactive explanations powered by Groq LLM, allowing users to ask questions and receive natural-language reasoning about each prediction

## Tech Stack

- PyTorch, Hugging Face Transformers
- Groq API (interactive LLM explanations)
- Google Colab (training environment)

