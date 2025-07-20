# Google-s-transformer-T5
The T5 is a unified deep learning model developed by Google that reframes all natural language processing  tasks into a text-to-text format. It is based on the Transformer architecture  but introduces key modifications for improved generalization and task flexibility
This project implements a variation of the GPT (Generative Pre-trained Transformer) model to generate wine reviews based on a dataset of wine descriptions. The model is trained on a dataset containing wine reviews from various regions, including details about the country, province, variety, and description of the wines. The goal is to generate coherent and realistic wine reviews using a transformer-based architecture.
Features
Data Processing: Cleans and formats wine review data for training.

Transformer Architecture: Implements a custom transformer block with multi-head attention and feed-forward layers.

Text Generation: Generates wine reviews based on a starting prompt with adjustable temperature for creativity control.

Training and Evaluation: Includes training loops with model checkpoints and text generation callbacks.

Dataset
The dataset used is winemag-data-130k-v2.json, which contains over 130,000 wine reviews. Each review includes:

Country

Province

Variety

Description
Model Architecture
The model consists of the following components:

Token and Position Embedding: Combines token embeddings with positional embeddings to capture the order of words.

Transformer Block: Includes multi-head attention, layer normalization, and feed-forward layers.

Output Layer: A dense layer with softmax activation to predict the next token in the sequence.

Key Parameters:
VOCAB_SIZE: 10,000

MAX_LEN: 80 tokens

EMBEDDING_DIM: 256

N_HEADS: 2

FEED_FORWARD_DIM: 256

BATCH_SIZE: 32

EPOCHS: 5

Usage
Training the Model
Load the dataset and preprocess the text.

Tokenize the data and create training sequences.

Train the model using the train_ds dataset.

Save the trained model for future use.
Files
GPT_model.ipynb: Jupyter notebook containing the complete implementation.

winemag-data-130k-v2.json: Dataset file (not included in the repository; must be downloaded separately).

License
This project is open-source and available under the MIT License
