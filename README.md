# Cats vs Dogs — Convolutional Neural Network

**Computer Vision · Deep Learning · TensorFlow/Keras · Experimental Evaluation**

## Overview | Descripción

An educational image-classification case study exploring how a custom convolutional neural network (CNN) learns to distinguish cats from dogs, and how changes to training settings influence its results.

Estudio académico de clasificación de imágenes que implementa una red neuronal convolucional (CNN) desde cero y compara el efecto de varios hiperparámetros sobre su entrenamiento y evaluación.

## Methodology | Metodología

- Dataset used in the recorded local experiments: **697 labeled images**, organized into `cats/` and `dogs/` folders.
- Baseline architecture: three convolutional layers (32, 64 and 128 filters), max-pooling, global average pooling, dropout (0.25) and a two-class softmax output.
- Training: Adam optimizer, sparse categorical cross-entropy and five baseline epochs.
- Experiments: batch size, image resolution, number of epochs, data augmentation, convolutional filters, activation function, dropout, optimizer, loss function and validation proportion.

## Recorded results | Resultados registrados

| Experiment | Recorded metric |
|---|---|
| Baseline (five epochs) | 59.71% validation accuracy |
| Dropout 0.50 experiment | 62.50% validation accuracy |
| Baseline model | 93,506 parameters reported in the notebook |

These are **saved outputs from an educational experiment**, not independently reproduced benchmarks. They should not be interpreted as production-level accuracy.

Estas cifras corresponden a **salidas guardadas del ejercicio académico**; no constituyen una validación externa ni acreditan un modelo listo para producción.

## Limitations | Limitaciones

- The dataset is small; comparisons between runs can be unstable.
- The notebook builds validation and test subsets using batches from a larger held-out dataset. The partitioning procedure needs review before making strong claims about an independent test set.
- The notebook uses Google Colab and project-specific Google Drive paths; the original image dataset is **not included** in this repository.
- Some cells depend on variables or helper functions defined earlier in the notebook. Run the notebook in order with the dataset configured.

## Files | Archivos

- [`case_study_cats_vs_dogs_convolutional_neural_network.ipynb`](case_study_cats_vs_dogs_convolutional_neural_network.ipynb) — original case-study notebook, including saved outputs.
- [`requirements.txt`](requirements.txt) — main Python dependencies.

## Running the notebook | Ejecución

1. Prepare a dataset directory with `cats/` and `dogs/` subfolders.
2. Open the notebook in Google Colab or a compatible Jupyter environment.
3. Update its Google Drive / `DATA_DIR` paths to your own data location.
4. Install the dependencies and run the cells in their intended order.

The training results were **not rerun** as part of preparing this repository.

## Use and attribution | Uso y atribución

This repository documents an educational case study. Unless separately stated, no permission to reuse or redistribute the author's original materials is granted. Third-party datasets and libraries remain subject to their respective terms.
