# Arabic-to-English Translation Using Transformer

This project develops a Transformer model to translate Arabic text to English using TensorFlow. Trained on Arabic-English sentence pairs, it harnesses the power of the Transformer architecture for accurate and efficient translation.

## Models Used

- **Transformer**: Machine translation using the transformer seq2seq featuring multi-head attention, positional embeddings, and feed-forward networks, implement a neural machine translation algorithm using the transformer encoder-decoder modeling..

## Features

- **Text Preprocessing**: Normalizes and tokenizes Arabic and English text, ensuring proper handling of special characters.
- **Advanced Architecture**: Utilizes a 4-layer Transformer with 128-dimensional embeddings and 8 attention heads.
- **Efficient Training**: Employs a custom learning rate schedule and model checkpointing for optimal performance.
- **Real-Time Inference**: Translates Arabic sentences into English seamlessly.
- **Training Visualization**: Integrates `tqdm` for clear progress tracking and loss metrics.

## Requirements

- Python 3.8+
- TensorFlow 2.10+
- NumPy
- tqdm
- unicodedata
- re

## Dataset

The model requires a dataset of Arabic-English sentence pairs. Download it from [[Dataset Link](https://github.com/SamirMoustafa/nmt-with-attention-for-ar-to-en/blob/master/ara_.txt)] and place the `ara_.txt` file in the project root. The dataset should contain tab-separated sentence pairs.

## Getting Started

- **Prepare the Dataset**:
  - Download `ara_.txt` and place it in the project root.
  - Ensure the file is formatted with tab-separated Arabic-English pairs.

- **Try it on Colab**:
  - Explore the project in Google Colab: [[Colab Link](https://colab.research.google.com/drive/1ZUzgs0FqWVNJ8-zCbwswUpBluMBS0v-u?usp=sharing)]

## Project Structure

- `main.py`: Handles data preprocessing, model definition, training, and inference.
- `ara_.txt`: Dataset file (to be downloaded and placed in the root).
- `transformer_model.keras`: Model checkpoint.
- `transformer_model_full.keras`: Final trained model.

## Example Output

```
Epoch 1/20: 100%|██████████| 168/168 [00:01<00:00, 146.74batch/s, Batch Loss=X.XXXX]
Epoch 1 | Train Loss: X.XXXX | Val Loss: X.XXXX | Time: X.XX sec
...
🟢 Arabic Input     : كيف حالك؟
🔵 English Translation : How are you?
```

## Acknowledgments

- Inspired by the "Attention is All You Need" paper by Vaswani et al.
- Developed with TensorFlow and Python for educational purposes.

## Contact

For questions or issues, open a GitHub issue or contact your-email@example.com.
