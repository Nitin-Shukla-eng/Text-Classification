# Text-Classification

Project Overview
This project focuses on Natural Language Processing (NLP) and Binary Text Classification. Using a dataset of over 100,000 wine reviews, I built a deep learning model that analyzes the text description of a wine and predicts whether it is "high quality" (90 points or above) or "standard quality."

Tech Stack & Tools
Language: Python

Environment: Google Colab

Deep Learning Framework: TensorFlow & Keras (using tf_keras legacy bridge)

Embeddings: TensorFlow Hub (nnlm-en-dim50)

Data Handling: Pandas, NumPy

Visualization: Matplotlib

Model Architecture
The model leverages Transfer Learning by using a pre-trained embedding layer from TensorFlow Hub. This allows the model to understand the semantic meaning of English words before training on specific wine vocabulary.

Input Layer: Raw text (wine descriptions).

Embedding Layer: nnlm-en-dim50 (converts text into 50-dimensional vectors).

Hidden Layers: Two Dense layers (16 units each) with ReLU activation.

Regularization: Dropout layers (0.4) to prevent overfitting.

Output Layer: Single Dense unit with Sigmoid activation (outputs a probability between 0 and 1).
