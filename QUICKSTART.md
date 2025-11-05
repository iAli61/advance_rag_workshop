# 🚀 Quick Start Guide - RAG Workshop

## TL;DR - Get Started in 3 Commands

```bash
uv sync                       # Install all dependencies
source .venv/bin/activate     # Activate environment
jupyter notebook              # Start Jupyter
```

Then edit `.env` with your Azure OpenAI credentials.
---

## What Was Created?

### ✅ Core Files
- **`pyproject.toml`** - All dependencies 
- **`.env.example`** - Environment variable template



---

## Installation Methods

```bash
# Install UV
curl -LsSf https://astral.sh/uv/install.sh | sh

# Create environment and install
uv venv
source .venv/bin/activate
uv pip install -e .

# Setup environment
cp .env.example .env
```

---

## Configure Azure OpenAI

Edit `.env` with your credentials:

```bash
nano .env
```

Required values:
```env
AZURE_OPENAI_API_KEY=your_key_here
AZURE_OPENAI_ENDPOINT=https://your-resource.openai.azure.com/
AZURE_OPENAI_DEPLOYMENT_NAME=gpt-4
AZURE_OPENAI_EMBEDDING_DEPLOYMENT=text-embedding-ada-002
```

---

## Test Your Setup

```bash
python -c "
import llama_index
import sentence_transformers
import torch
import ragas
print('✅ All packages imported successfully!')
print(f'PyTorch: {torch.__version__}')
print(f'CUDA: {torch.cuda.is_available()}')
"
```

---

## Start Working

```bash
# Activate environment
source .venv/bin/activate

# Start Jupyter
jupyter notebook

# Navigate to RAG_demo/ folder
# Open any demo notebook (01-12)
```