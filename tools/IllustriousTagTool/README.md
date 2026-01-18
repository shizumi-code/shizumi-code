# IllustriousTagTool — Free MVP v0.1

IllustriousTagTool is an offline Windows desktop tool designed to generate
**tag classification candidates** from natural language input using a local LLM.

This document is the **canonical specification** for the Free MVP version.

---

## Purpose

The purpose of IllustriousTagTool is to assist humans in organizing text
into structured tag candidates.

* This tool **does not make decisions**
* This tool **does not confirm classifications**
* All final judgments are made by humans

The Free MVP focuses on correctness, transparency, and safe data handling,
rather than automation or optimization.

---

## Key Characteristics (Free MVP v0.1)

* Fully offline execution (no internet connection)
* Windows executable distribution
* Local LLM bundled for internal processing
* Simple single-input UI
* Fixed category structure
* CSV-based data storage
* Explicit error handling (no silent failures)

---

## What This Tool Does

* Accepts natural language input (Japanese / English mixed input supported)
* Processes text using a local LLM
* Outputs **classification candidates only**
* Displays results in a fixed category list
* Allows copying results for external use

---

## What This Tool Does NOT Do

The following are **intentionally excluded** from the Free MVP:

* Automatic classification confirmation
* Translation or language normalization
* Tag recommendation scoring
* Learning, fine-tuning, or model updates
* Online API communication
* UI customization or filtering

These features may be explored in later versions.

---

## Distribution

* Platform: Windows
* Distribution format: Standalone executable (folder-based)
* Internet connection: Not required

Executable files are **not stored in this repository**.

Please download the tool from:
[https://github.com/shizumi-code/shizumi-code/releases](https://github.com/shizumi-code/shizumi-code/releases)

---

## Bundled Local LLM

This tool bundles a third-party local LLM for offline processing.

* Model: Qwen2.5-3B-Instruct
* Format: GGUF
* Quantization: Q4_K_M

The model is used locally only.
Ownership and copyright remain with the original authors.

---

## License Notice (LLM)

The bundled LLM is distributed under the **Apache License 2.0**.

* The license text is included in the distributed package
* Users must comply with the original license terms

This repository does not claim ownership of the model itself.

---

## Data Ownership

* All CSV files and generated outputs belong to the user
* No data is collected, transmitted, or stored externally

---

## Status

* Free MVP v0.1: **Completed and finalized**
* Latest release: v0.1.1 (finalized Free MVP distribution)

Future versions may expand functionality,
but the Free MVP baseline is considered complete.
