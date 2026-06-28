# 🎶 Stem Separation Demucs

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1n79yj-f4m-Z7-_bKkZg19BjTqEg8eV_L)
[![Developer Portfolio](https://img.shields.io/badge/Developer-gbaudio-blue)](https://linktr.ee/gbaudio)

An ultra-clear, beginner-friendly Google Colab workflow for high-quality audio source separation using Meta's **Demucs (Hybrid Transformer)** architecture[cite: 5].

This repository features an updated **Modular Structure** designed for newcomers[cite: 5]. The workflow is split into logical, bite-sized steps with explicit file setup instructions and detailed real-time logging[cite: 5].

---

## 🚀 Quick Start

1. **Prepare Google Drive:** Log into your Google Drive and create a folder named exactly `StemSeparation` in your main drive directory[cite: 5].
2. **Upload Your Audio:** Drop your target master audio file (e.g., `song.wav` or `track.mp3`) directly into that `StemSeparation` folder[cite: 5].
3. **Launch the Notebook:** Click the **Open In Colab** badge above or use [this direct link](https://colab.research.google.com/drive/1n79yj-f4m-Z7-_bKkZg19BjTqEg8eV_L) to open the updated environment[cite: 5].
4. **Configure & Run:** Set your runtime to GPU (`Runtime` > `Change runtime type` > `T4 GPU`)[cite: 5]. In Step 3 of the `Google Colab`, the code will pause and ask you to type the exact filename of your audio file; enter it and press **Enter** to proceed[cite: 4, 5].

---

## 👁️ Notebook Preview & Architecture

| Step | Purpose | Key Actions |
| :--- | :--- | :--- |
| **Step 1** | **Connect Google Drive** | Safely mounts your personal Drive space to read/write files[cite: 4, 5]. |
| **Step 2** | **Install Dependencies** | Updates environment with `torch`, `torchaudio`, and `demucs`[cite: 4, 5]. |
| **Step 3** | **File Verification** | **[Interactive Input]** Type your filename when prompted; the script verifies the file before processing[cite: 4, 5]. |
| **Step 4** | **Execute Extraction** | Runs the high-fidelity `htdemucs_ft` separation with verbose logging (`-v`) and 24-bit output[cite: 4, 5]. |

> ⚠️ **Important Safety Note:** This workflow operates strictly within your own isolated Google Colab instance[cite: 5]. Mounting your Google Drive only gives *your personal runtime* access to your files[cite: 5]. Your data is completely secure, private, and never shared with external repositories or third parties[cite: 5].

---

## 🛠️ Key Features
- **Interactive Workflow:** Step 3 uses a direct user prompt, making it easy to swap files without editing code[cite: 4].
- **Verbose Real-Time Logging:** Detailed console outputs let you track exact progress[cite: 5].
- **High-Fidelity 24-bit Output:** Retains maximum audio depth for professional use in DAWs[cite: 5].
- **Smart Validation:** The script alerts you instantly if a file name is misspelled before wasting computing time[cite: 4, 5].

---

## 👤 About the Developer

Workflow by **Geoff Bremner (gbaudio)**, an audio software engineer specializing in digital signal processing (DSP), real-time buffer management, and intelligent audio tools[cite: 4, 5]. 

* Check out more projects, tools, and portfolios: [linktr.ee/gbaudio](https://linktr.ee/gbaudio)

---

## References & Licensing
- [Demucs GitHub Repository](https://github.com/facebookresearch/demucs)[cite: 5]
- This project utilizes Demucs, licensed under the MIT License[cite: 5].