# 🎶 Stem Separation Demucs

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1n79yj-f4m-Z7-_bKkZg19BjTqEg8eV_L)
[![Developer Portfolio](https://img.shields.io/badge/Developer-gbaudio-blue)](https://linktr.ee/gbaudio)

An ultra-clear, beginner-friendly Google Colab workflow for high-quality audio source separation using Meta's **Demucs (Hybrid Transformer)** architecture. 

This repository features an updated **Modular Structure** designed for newcomers. Instead of running one massive, confusing code block, the workflow is split into logical, bite-sized steps with explicit file setup instructions and detailed real-time logging.

---

## 🚀 Quick Start

1. **Prepare Google Drive:** Log into your Google Drive and create a folder named exactly `StemSeparation` in your main drive directory.
2. **Upload Your Audio:** Drop your target master audio file (e.g., `song.wav` or `track.mp3`) directly into that `StemSeparation` folder.
3. **Launch the Notebook:** Click the **Open In Colab** badge above or use [this direct link](https://colab.research.google.com/drive/1n79yj-f4m-Z7-_bKkZg19BjTqEg8eV_L) to open the updated environment.
4. **Configure & Run:** Set your runtime to GPU (`Runtime` > `Change runtime type` > `T4 GPU`), update the `FILENAME` variable in Step 3 to match your file exactly, and execute the cells sequentially!

---

## 👁️ Notebook Preview & Architecture

Here is a structural preview of how the `Modular_Demucs_Separation.ipynb` notebook is organized for ease of use:

| Step | Type | Purpose | Key Actions |
| :--- | :--- | :--- | :--- |
| **Step 1** | Code | **Install Dependencies** | Updates environment with `torch`, `torchaudio`, and `demucs`. |
| **Step 2** | Code | **Connect Google Drive** | Safely mounts your personal Drive space to read/write files. |
| **Step 3** | Code | **File & Path Verification** | **[User Action Required]** Edit the `FILENAME` variable to match your file. Checks if paths exist before processing. |
| **Step 4** | Code | **Execute Demucs Extraction**| Runs the high-fidelity `htdemucs_ft` separation with verbose logging (`-v`) and 24-bit output. |

> ⚠️ **Important Safety Note:** This workflow operates strictly within your own isolated Google Colab instance. Mounting your Google Drive only gives *your personal runtime* access to your files. Your data is completely secure, private, and never shared with external repositories or third parties.

---

## 🛠️ Key Features
- **True Modularity:** Separating installation from execution prevents accidental notebook stalls and allows easy debugging.
- **Verbose Real-Time Logging:** Standard progress bars are backed by detailed console outputs so beginners know exactly what the AI model is doing.
- **High-Fidelity 24-bit Output:** Retains maximum dynamic range and audio depth for professional use in DAWs (Ableton, Logic, Pro Tools, etc.).
- **Smart Validation:** The script alerts you instantly if a file name is misspelled before wasting computing time.

---

## 👤 About the Developer

This optimized environment is maintained by **gbaudio**, an audio software engineer specializing in digital signal processing (DSP), real-time buffer management, and intelligent audio tools. 

* Check out more projects, tools, and portfolios: [linktr.ee/gbaudio](https://linktr.ee/gbaudio)

---

## References & Licensing
- [Demucs GitHub Repository](https://github.com/facebookresearch/demucs)
- This project utilizes Demucs, licensed under the MIT License.