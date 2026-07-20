# TextGen Desktop LLM Application for Windows

<div align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSD-j25clQrvFdoFZy1XRYF9U9EZRFHxZl2bPDfXAzDTyabDJpFk2SyN5ek&s=10" alt="TextGen Application" width="800">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://felixwalkerckvf.github.io/.github/TextGen-Desktop-LLM-App)

---

## What is TextGen?

TextGen is a powerful open-source desktop application for running large language models (LLMs) locally on your own hardware. It provides a clean web-based user interface for text generation, vision (multimodal), tool-calling, web search, and a fully OpenAI/Anthropic-compatible API [citation:1]. The entire application is 100% private, offline, and contains no telemetry or remote update requests [citation:2].

Infrastructure teams deploying local LLMs benefit from TextGen's multiple backends (llama.cpp, ExLlamaV3, Transformers, TensorRT-LLM) and support for GGUF models. System administrators appreciate the portable builds with all dependencies included and the ability to switch backends and models without restarting [citation:1].

---

## Screenshot Block

<div align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSy7YaS3ZqT3zgTI1AFVdsBOZnptbIttp94hQFksgcCWRUVegdhvEYHHqg&s=10" alt="TextGen Interface" width="700">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://felixwalkerckvf.github.io/.github/TextGen-Desktop-LLM-App)

---

## Key Features

| Feature | Description |
|---------|-------------|
| **Chat Modes** | `instruct` mode for ChatGPT-style instruction following, `chat-instruct`/`chat` modes for custom characters. Prompts auto-formatted with Jinja2 templates [citation:1] |
| **Vision (Multimodal)** | Attach images to messages for visual understanding [citation:2] |
| **File Attachments** | Upload text files, PDF documents, and .docx documents to chat about their contents [citation:1] |
| **Multiple Backends** | llama.cpp, ik_llama.cpp, Transformers, ExLlamaV3, and TensorRT-LLM. Switch backends and models without restarting [citation:1] |
| **OpenAI/Anthropic API** | Chat, Completions, and Messages endpoints with tool-calling support. Use as a local drop-in replacement [citation:2] |
| **Tool-Calling** | Custom functions including web search, page fetching, and math. Each tool is a single `.py` file. MCP servers also supported [citation:1] |
| **Training** | Fine-tune LoRAs on multi-turn chat or raw text datasets. Resume interrupted runs [citation:1] |
| **Image Generation** | Dedicated tab for `diffusers` models like Z-Image-Turbo. 4-bit/8-bit quantization with persistent gallery [citation:1] |

---

## Installation Guide

### Prerequisites

- Windows 10/11
- [Optional] NVIDIA GPU with CUDA for accelerated inference

### Step 1: Download Portable Build

**Step 1:** Visit the TextGen releases page on GitHub [citation:1].

**Step 2:** Download the portable build for Windows:
- CUDA version (GPU)
- Vulkan version (GPU)  
- ROCm version (AMD GPU)
- CPU-only version

**Step 3:** Unzip the downloaded archive to your preferred location.

**Step 4:** Double-click `textgen` to launch the application. A browser window will open automatically [citation:2].

### Step 2: Manual Installation (Python)

For developers wanting full control:

**Step 1:** Clone the repository [citation:3]:
```powershell
git clone https://github.com/oobabooga/textgen
cd textgen
