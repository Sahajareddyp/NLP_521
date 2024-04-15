Stock Embeddings Generation Repository
This repository is dedicated to the development and application of machine learning models for generating stock embeddings, offering powerful tools for analyzing and visualizing financial data through the lens of Natural Language Processing (NLP) and context-aware algorithms.

Python Notebooks
pointwise_embeddings.ipynb: Showcases methods for generating dense vector representations of stocks on a pointwise basis. The notebook includes detailed procedures for training models on financial data and evaluating the generated embeddings to capture the nuanced performance of individual stocks.
window_embeddings.ipynb: Concentrates on constructing embeddings based on a sliding window approach, which is instrumental in capturing the temporal and contextual nuances of stock data that can influence market behavior.
CS521.ipynb: Contains specialized coursework and demonstrations that pertain to advanced techniques in financial machine learning, as explored in the context of the CS521 course.
Python Scripts
training_helpers.py: Supplies helper functions designed to streamline the machine learning pipeline for stock embeddings, encompassing tasks such as batch processing, training loop orchestration, and evaluation metrics.
visualisation_functions.py: Comprises a toolkit for visualizing financial data and the performance of stock embeddings, aiding in understanding and interpreting complex patterns within the stock market.
window_context.py: This utility is crucial for managing and processing financial data within a given window context, optimizing models that rely on historical data for accurate predictions.
returns_data_class.py: Defines structures and functions for processing returns data, preparing and normalizing financial time-series data for optimal model input.
sector_classification.py: Implements sector-based classification techniques, allowing for nuanced analysis and categorization of stocks into relevant market sectors.
embedding_models.py: Includes the architecture and implementation details of various embedding models tailored for the financial domain, alongside utilities for model persistence and retrieval.
base_model.py: Outlines the foundational model framework that standardizes the approach across different embedding models in this project.
pointwise_context.py: Provides functionality for enhancing stock data inputs with context-sensitive features that improve model performance.
Main NLP Model Architecture
Our primary NLP model employs a sophisticated Transformer-based architecture, adept at managing sequences of stock-related data with an attention mechanism that contextualizes the importance of different time points and attributes in the dataset.

Key Functionalities
Embedding Generation: The model excels at creating high-fidelity embeddings from stock market data, encapsulating both semantic and temporal patterns that are crucial for downstream analysis.
Contextual Analysis: By utilizing both window-based and pointwise methods, the model can dissect and interpret stock data within specific market contexts, sharpening its capabilities in applications like trend analysis and anomaly detection.
Sector Classification: The model is finely tuned for classifying stocks into industry sectors, a feature that leverages embeddings to discern and predict sectoral trends and dynamics.
Data Processing Workflow
Preprocessing: Financial data is cleansed and normalized, including steps such as tokenization of textual data and alignment of time series.
Vectorization: The model transforms preprocessed data into numerical vectors, ensuring that both textual information and numerical indicators are encoded efficiently.
Attention Mechanisms: Utilizing self-attention, the model dynamically weighs the relevance of different parts of the data, reflecting the ever-changing landscape of the financial markets.
Outputs and Performance Evaluation
Pointwise Embedding Model Output
The pointwise embedding model was rigorously evaluated to determine its efficacy, achieving a precision score of 0.68 and an F1 score of 0.65. The model also showed an accuracy of 0.65, with a top-3 accuracy rate of 0.85, indicating its robustness in handling stock data. A PCA visualization of the embeddings reveals distinct clustering by sector, underlining the model's potential in classifying stocks based on their embedded features.

Window-wise Embedding Model Output
The window-wise embedding model presented a precision score of 0.52 and an F1 score of 0.49. While its accuracy score stood at 0.48, the PCA visualization highlighted the dispersion of stocks across sectors, suggesting that while the model captures sector-specific characteristics, there is room for refinement to enhance its predictive precision.
