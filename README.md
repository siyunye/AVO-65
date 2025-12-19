# AVO-65: A Large-Scale Hierarchical Audio-Visual Object Dataset

[![License: CC BY 4.0](https://img.shields.io/badge/Data%20License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![License: MIT](https://img.shields.io/badge/Code%20License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Official repository for the paper: **"AVO-65: A LARGE-SCALE HIERARCHICAL AUDIO-VISUAL OBJECT DATASET"** (Submitted to ICASSP 2026).

---

## 🚀 Overview

**AVO-65** is a novel, object-centric audio-visual dataset designed to advance research in robust multimodal learning. Unlike previous datasets that focus on flat labels or single modalities, AVO-65 treats auditory and visual modalities with equal importance and provides a rigorous hierarchical structure.

### Key Features:
* **Scale:** \~30,000 high-quality video segments (\~83 hours).
* **Taxonomy:** The first dataset to systematically apply the **Hornbostel-Sachs (H-S) taxonomy** for hierarchical audio-visual labeling.
* **Consistency:** Guaranteed **semantic, temporal, and spatial consistencies** between audio and visual tracks.
* **Real-world Complexity:** 100% real-world samples, retaining challenging cases like occlusion and modality absence.
* **Granularity:** 4-level hierarchical labels covering 65 distinct object categories.

---

## 📂 Dataset Structure

The dataset is organized into 4 hierarchical levels. Below is an example of our annotation format in the released CSV:

| YouTube ID | Start Time | End Time | Level 1 | Level 2 | Level 3 | Level 4 (Label) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `video_id_001` | 10.5 | 20.5 | Idiophones | Struck Idiophones | Cymbals | **Crash Cymbal** |
| `video_id_002` | 45.0 | 55.0 | Chordophones | Lutes | Bowed Lutes | **Cello** |

### Taxonomy Visualization
AVO-65 follows the **Hornbostel-Sachs** classification system, providing a unique foundation for **Hierarchical Learning**:
1.  **Idiophones** (e.g., Triangle, Xylophone)
2.  **Membranophones** (e.g., Snare Drum, Bass Drum)
3.  **Chordophones** (e.g., Piano, Violin, Guitar)
4.  **Aerophones** (e.g., Flute, Trumpet)
5.  **Electrophones** (e.g., Electric Guitar, Synthesizer)

---

## 🛠 Usage & Download

### 1. Download Annotations
The complete metadata and labels are provided in `avo65_metadata.csv`.

### 2. Data Access
As per ICASSP infrastructure guidelines, we provide YouTube IDs and timestamps. You can use tools like `yt-dlp` to download the original segments.

---

## 📊 Baselines

We provide comprehensive baseline evaluations on AVO-65, including both CNN-based and Transformer-based architectures:

* **CNN Backbones:** ResNet, VGG.
* **SOTA Models:** **MBT** (Multimodal Bottleneck Transformer), **UAVM** (Unified Audio-Visual Model).
* **Fusion Strategies:** Concatenation, Cross-Attention, Bottleneck Fusion.

> **Note:** Detailed SOTA comparison results can be found in **Table 6** of our paper.

---

## 📜 License

* **Data:** The AVO-65 dataset annotations are licensed under a [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
* **Code:** All scripts and baseline implementations are licensed under the [MIT License](LICENSE).

---

## ✍️ Citation

If you find AVO-65 useful in your research, please cite our work.

---

### 🎬 Dataset Samples

<div align="center">
  <video src="https://github.com/user-attachments/assets/1504c894-3080-4d21-b635-139a411ba9c6" 
         width="200" 
         controls="controls">
  </video>
  <br />
  <p>
    <b>Category: Guitar (Chordophones)</b><br />
    <i>(Native GitHub Player: Click play to watch directly)</i>
  </p>
</div>
  <p>
    <b>Category: Guitar (Chordophones)</b><br />
    <i>(Native GitHub Player: Click play to watch directly)</i>
  </p>
</div>


