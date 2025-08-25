# Gen AI Local Recipes

A comprehensive collection of Jupyter notebooks and basic utilities for running large language models (LLMs) and diffusion models efficiently on local hardware. This project provides practical recipes and best practices for developers and researchers who want to harness the power of generative AI without relying on cloud services.

## Table of Contents

- [Features](#-features)
- [Quick Start](#-quick-start)
- [Notebooks](#-notebooks)
- [Project Structure](#-project-structure)
- [Hardware Requirements](#-hardware-requirements)
- [License](#-license)

## Features

- **GPU Evaluation**: Tools to assess your hardware capabilities
- **Text Generation**: Comprehensive examples using Hugging Face models
- **Chat Interfaces**: Build conversational AI systems locally
- **Model Quantization**: Optimize models for resource-constrained environments
- **Image Generation**: Stable Diffusion and Flux model implementations
- **LoRA Fine-tuning**: Advanced model customization techniques
- **Text-to-Video**: Cutting-edge video generation capabilities
- **Utilities**: Helper functions for model management and evaluation

## Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/gen-ai-local-recipes.git
   cd gen-ai-local-recipes
   ```

2. **Set up the environment**
   ```bash
   # Create virtual environment
   uv venv --seed
   
   # Activate environment (Windows)
   .venv\Scripts\activate
   
   # Activate environment (Linux/macOS)
   source .venv/bin/activate
   
   # Install dependencies
   uv sync
   ```

3. **Launch Jupyter Lab** (optional: Jupyter is also supported by some IDEs)
   ```bash
   jupyter lab
   ```

4. **Start with the setup notebook**
   Open `notebooks/01 - Environment Setup.ipynb` to install initial dependencies and authenticate with Hugging Face.

## Notebooks

The project includes hands-on tutorials covering various aspects of local AI deployment:

| Notebook | Description | Difficulty |
|----------|-------------|------------|
| `01 - Environment Setup.ipynb` | Initial setup and Hugging Face authentication | Beginner |
| `02 - GPU Evaluation.ipynb` | Hardware assessment and memory profiling | Beginner |
| `03 - Text Generation - HF.ipynb` | Text generation with Hugging Face models | Intermediate |
| `04 - Chat - HF.ipynb` | Building chat interfaces with local models | Intermediate |
| `05 - Quantization - HF.ipynb` | Model optimization and quantization techniques | Advanced |
| `08.1 - Diffusion Models - sd.ipynb` | Stable Diffusion image generation | Intermediate |
| `08.2 - Diffusion Models - flux.ipynb` | Flux model implementations | Advanced |
| `09 - Diffusion with LoRA.ipynb` | Custom model training with LoRA | Advanced |
| `10 - Text2Video Diffusion.ipynb` | Video generation from text prompts | Advanced |

## Project Structure

```
gen-ai-local-recipes/
├── notebooks/              # Jupyter notebooks with tutorials
├── src/                    # Source code and utilities
│   ├── __init__.py
│   └── utils.py           # Helper functions for model management
├── pyproject.toml         # Project configuration and dependencies
├── uv.lock               # Dependency lock file
├── LICENSE               # Apache License 2.0
└── README.md             # This file
```

## Hardware Requirements

### Recommended Configuration
- **GPU**: NVIDIA RTX 3080/4080 or better (12GB+ VRAM)

### Model Size Guidelines
Use the [Hugging Face Model Size Estimator](https://huggingface.co/docs/accelerate/main/en/usage_guides/model_size_estimator) to determine VRAM requirements for different models and quantization levels.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Hugging Face](https://huggingface.co/) for their excellent model hub and libraries

---

**Made with ❤️ for the local AI community**
