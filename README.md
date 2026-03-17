Gemini Embedding 2 is Google's first natively multimodal embedding model that maps text, images, video, audio and documents into a single embedding space, enabling multimodal retrieval and classification across different types of media — and it's available now in public preview.

## Overview
This repository contains a comprehensive Jupyter notebook that demonstrates how to use the Gemini Embedding 2 API for generating multimodal embeddings using the new Google Generative AI SDK.

## Features
- **Multimodal Support**: Embed text, images, videos, audio, and PDFs
- **Unified Embedding Space**: All modalities map to a single 3072-dimensional embedding space by default
- **Cross-Modal Search**: Perform semantic searches across different media types
- **Batch Processing**: Generate embeddings for multiple inputs efficiently
- **Configurable Dimensions**: Truncate embeddings to lower dimensions as needed
- **Semantic Similarity**: Analyze sentence similarity and classification

## Getting Started

### Prerequisites
- Python 3.7+
- Google API Key (get one at [ai.google.dev](https://ai.google.dev))
- Jupyter Notebook environment (for Colab compatibility)

### Installation
```bash
pip install -q -U google-genai
```

### Quick Start
1. Set up your API key in a Colab Secret named `GOOGLE_API_KEY`
2. Open the notebook: `Google's_Gemini_Embedding_2.ipynb`
3. Run the cells to explore different embedding examples

## Supported Formats

### Text
- Up to 8,192 tokens per request

### Images
- Maximum of 6 images per request
- Supported formats: PNG, JPEG

### Audio
- Maximum duration: 80 seconds
- Supported formats: MP3, WAV

### Video
- Maximum duration: 128 seconds
- Supported formats: MP4, MOV

### PDF Documents
- Maximum of 6 pages per request
- Processes both visual and text content

**Note**: Overall maximum input tokens limit is 8,192 tokens

## Key Examples in the Notebook

1. **Text Embeddings**: Generate embeddings for text inputs
2. **Image Embeddings**: Embed images individually
3. **Multimodal Aggregation**: Combine text and images for aggregated embeddings
4. **Audio Embeddings**: Process audio files
5. **Video Embeddings**: Embed video content
6. **PDF Embeddings**: Extract embeddings from PDF documents
7. **Batch Processing**: Generate multiple embeddings in one API call
8. **Dimension Customization**: Truncate embeddings to custom dimensions
9. **Sentence Similarity Analysis**: Analyze semantic similarity between sentences using embeddings

## Model Information
- **Model ID**: `gemini-embedding-2-preview`
- **Output Dimensions**: 3,072 (default, customizable)
- **Language Support**: Over 100 languages

## Use Cases
- Semantic search across multiple modalities
- Content classification and clustering
- Cross-modal recommendation systems
- Similarity analysis
- Information retrieval

## Resources
- [Gemini API Documentation](https://ai.google.dev/gemini-api/docs/models/gemini)
- [Google Generative AI Python SDK](https://github.com/google/generative-ai-python)
- [Embedding API Guide](https://ai.google.dev/gemini-api/docs/embeddings)
- [Medium](https://iamshobhitagarwal.medium.com/googles-gemini-embedding-2-the-silent-release-that-could-change-enterprise-ai-forever-a9314289910b)
