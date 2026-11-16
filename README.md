# Russian Text Style Transfer

A student natural language processing project that fine-tunes **mT5-small** to rewrite excerpts from Russian classics in contemporary slang. The notebook prepares paired texts, trains a sequence-to-sequence model with a custom PyTorch training loop, and generates rewrites of new passages.

The original coursework run used **12,000 training examples** and **2,487 validation examples**. It reported a validation loss of 0.793 and mean per-example scores of 0.7566 for the notebook's BLEU variant and 0.8514 for its chrF variant.

## Run the notebook

1. Install the requirements with `python -m pip install -r requirements.txt`. A CUDA GPU is recommended for training.
2. Add a UTF-8 `dataset.csv` with columns `chunk` (original passage) and `translate` (rewritten passage). Use paired texts that you have permission to use.
3. Open `project.ipynb` in Jupyter and run the cells in order. The notebook downloads the base model and saves the fine-tuned checkpoint locally.

The original coursework dataset and model checkpoint are excluded from this repository.
