# Evaluation of the Transformer model for summarization on the CNN/Dailymail dataset

1. Preprocessing ([preprocess.ipynb](preprocess.ipynb))
   * Preprocesses data and stores in GCS-bucket.
2. Exploring dataset ([dataset_metadata.ipynb](dataset_metadata.ipynb))
   * Reads dataset and plots summary of input and output lengths.
3. Model training ([training.ipynb](training.ipynb))
   * Trains the model and stores checkpoints on GCS-bucket.
4. Model evaluation ([generate_targets_and_inputs.ipynb](generate_targets_and_inputs.ipynb), [decode_and_evaluate.ipynb](evaluate.ipynb))
   * Generates data for evaluation or testing.
   * Decodes on generated data and scores using py-rouge-155 (official implementation)
