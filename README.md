# freelance-hotel-OCR

```markdown
# Hugging Face Repository Download Guide

This guide will show you how to download datasets and models from a Hugging Face repository.

## Prerequisites

Before you begin, ensure you have installed the `huggingface_hub` library:

```bash
pip install huggingface_hub
```

## Downloading a Specific File

To download a specific file from a repository, use the `hf_hub_download()` function:

```python
from huggingface_hub import hf_hub_download

# Download a file
hf_hub_download(repo_id="d4rk3r/invoices", filename="path/to/file", repo_type="dataset")
```

## Downloading an Entire Repository

To download an entire repository, use the `snapshot_download()` function:

```python
from huggingface_hub import snapshot_download

# Download the entire repository
snapshot_download(repo_id="d4rk3r/invoices", repo_type="dataset")
```

## Versioning

You can download a specific version of a file or repository by using the `revision` parameter:

```python
# Download a specific version of a file
hf_hub_download(repo_id="d4rk3r/invoices", filename="path/to/file", revision="v1.0", repo_type="dataset")

# Download a specific version of a repository
snapshot_download(repo_id="d4rk3r/invoices", revision="v1.0", repo_type="dataset")
```
