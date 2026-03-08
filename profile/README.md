# Local Inference (LI)

**Local Inference (LI)** is an open initiative focused on building **small, specialized machine learning models** that run locally anywhere.

LI models are designed to be practical, predictable, and deployable without centralized infrastructure. Instead of large general-purpose models, LI focuses on **narrow models trained for a specific task and language**.

These models are intended to run directly on user devices, servers, or browsers.

## Goals

The Local Inference project aims to:

- Build **small task-specific models** rather than large general models
- Enable **local execution** without cloud dependency
- Provide **portable models** that run across platforms
- Keep tooling **simple and developer-friendly**

## Runtime

LI models are distributed in the **ONNX format**, allowing them to run across many environments including:

- Node.js
- Browsers (WebAssembly / WebGPU runtimes)
- Python
- Native runtimes supporting ONNX

This makes the models portable and independent from any single framework.

## Usage

There are two supported ways to use LI models.

### JavaScript package

Each model can be installed through a JavaScript package manager and used through a **simple managed API**.

This option provides the easiest developer experience.

### Direct ONNX usage

Developers can also download the **raw ONNX model** and build their own runtime wrapper.

This allows full control over:

- Runtime choice
- Memory management
- Execution environment
- Integration architecture

## Tokenization

All LI language models use **SentencePiece** tokenization.

This ensures consistent tokenization across environments and languages.

## Licensing

Everything produced by the Local Inference project is released under the **Apache License 2.0**.

This includes:

- Models
- Code
- Tooling
- Specifications

The goal is to keep the ecosystem fully open and usable in both open-source and commercial environments.

## Philosophy

Local Inference promotes a **local-first model architecture**:

- Computation happens where the data lives
- Models are small and specialized
- Infrastructure requirements are minimal

Rather than one large general model, the ecosystem encourages a **collection of focused models**, each optimized for a specific task.
