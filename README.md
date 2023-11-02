# freelance-hotel-OCR

## Hugging Face Repository Download Guide

This guide will show you how to download datasets and models from a [Hugging Face repository](https://huggingface.co/datasets/d4rk3r/invoices).

## Prerequisites

Before you begin, ensure you have installed the `huggingface_hub` library:

```bash
pip install huggingface_hub
```

## Cloning The HF Repo

You can clone an entire repository using `git clone` command:

```bash
git clone https://huggingface.co/datasets/d4rk3r/invoices
```

## Downloading a Specific File

To download a specific file from a repository, use the `hf_hub_download()` function, replace `path/to/file` to actual file path:

```python
from huggingface_hub import hf_hub_download

file_path = hf_hub_download(repo_id="d4rk3r/invoices", filename="path/to/file", repo_type="dataset")
```

## Downloading an Entire Repository

To download an entire repository, use the `snapshot_download()` function:

```python
from huggingface_hub import snapshot_download

file_path = snapshot_download(repo_id="d4rk3r/invoices", repo_type="dataset")
```
