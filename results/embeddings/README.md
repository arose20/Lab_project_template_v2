# Embeddings

This directory contains exported low-dimensional or latent representations derived from processed data.

## Examples

- PCA coordinates
- UMAP embeddings
- t-SNE embeddings
- Harmony embeddings
- scVI latent space
- NicheCompass latent space

## Rules

- Embeddings should be reproducible from processed data.
- Prefer storing embeddings within canonical datasets (e.g. AnnData, Seurat) when possible.
- Export embeddings here only when they are intended for sharing or downstream use.
