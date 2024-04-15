# Stock Embeddings Generation Repository
## Overview
This repository focuses on applying machine learning models to generate and analyze stock embeddings. Our goal is to provide tools for visualizing financial data and capturing market dynamics through advanced NLP techniques and context-aware algorithms.

## Contents

### Python Notebooks
- **pointwise_embeddings.ipynb**
  - Demonstrates the generation of pointwise stock embeddings and includes training and evaluation methods.
- **window_embeddings.ipynb**
  - Focuses on creating embeddings using a sliding window over the stock data, capturing temporal context.
- **CS521.ipynb**
  - Contains advanced financial machine learning techniques, as part of the CS521 course content.

### Python Scripts
- **training_helpers.py**
  - Provides batch processing, training loop management, and evaluation metrics for embedding models.
- **visualisation_functions.py**
  - Tools for visualizing stock market data and interpreting embedding model performance.
- **window_context.py**
  - Manages data within a window context for models requiring time-based historical input.
- **returns_data_class.py**
  - Processes and normalizes financial returns data for model input.
- **sector_classification.py**
  - Implements stock classification into market sectors based on embedding characteristics.
- **embedding_models.py**
  - Contains the implementation of various stock embedding models and associated utilities.
- **base_model.py**
  - Outlines a standard model structure used across the project's machine learning models.
- **pointwise_context.py**
  - Enhances stock data input with additional context for improved model accuracy.

## Main NLP Model
### Architecture
- The primary NLP model uses a **Transformer-based architecture** with attention mechanisms to contextualize data points in stock market sequences.

### Key Functionalities
- **Embedding Generation**
  - Generates semantic-rich embeddings from stock data.
- **Contextual Analysis**
  - Analyzes stock data within given market contexts for trend analysis and anomaly detection.
- **Sector Classification**
  - Classifies stocks into industry sectors to predict market trends.

### Data Processing

1. **Preprocessing**
   - Cleansing and normalizing financial data.
2. **Vectorization**
   - Converting data into numerical form suitable for model input.
3. **Attention Mechanisms**
   - Applying self-attention to prioritize relevant data points dynamically.

## Model Outputs and Evaluation

### Pointwise Embedding Model Output

- **Performance Metrics**
  - Precision Score: **0.68**
  - Recall Score: **0.65**
  - F1 Score: **0.65**
  - Accuracy Score: **0.65**
  - Accuracy Score Top-3: **0.85**

- **Visualization**
  - PCA scatter plot demonstrating sector clustering of stock embeddings.

### Window-wise Embedding Model Output

- **Performance Metrics**
  - Precision Score: **0.52**
  - Recall Score: **0.48**
  - F1 Score: **0.49**
  - Accuracy Score: **0.48**

- **Visualization**
  - PCA scatter plot showing dispersion and sector overlap in stock embeddings.

