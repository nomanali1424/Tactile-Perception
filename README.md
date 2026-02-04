# Tactile-Perception

This repository investigates how the brain processes tactile sensations using EEG.
By analyzing neural activity during active touch tasks, the project aims to
understand the relationship between human tactile perception, behavioral judgments,
and EEG responses.

The repository emphasizes **experimental design, signal preprocessing, and
behavioral analysis**, serving as a transparent and research-oriented EEG pipeline
rather than a performance-focused modeling project.

---

## Project Overview

Tactile perception is a complex cognitive process involving sensory encoding,
perceptual judgment, and motor interaction. This project explores:

- EEG signal characteristics during active tactile exploration
- Behavioral similarity judgments of textured objects
- The relationship between perceptual structure and neural responses

The repository documents the full workflow from **experiment design and data
collection** to **EEG preprocessing and behavioral analysis**.

---

## Repository Structure

```
├── single_subject_eeg_preprocessing_validation.ipynb
│ Exploratory notebook demonstrating EEG preprocessing on a single subject
│ (artifact inspection, filtering, baseline correction, and time–frequency analysis)
│
├── Behavioural Data Analysis/
│ ├── Analysis.ipynb
│ ├── MDS_Analysis.ipynb
│ └── README.md
│ Behavioral preprocessing and perceptual analysis of similarity ratings,
│ including Multidimensional Scaling (MDS)
│
├── report/
│ ├── mid_assessment_report.pdf
│ └── README.md
│ Detailed documentation of experimental design, data collection protocol,
│ and hardware/software setup
│
├── Physiological vs Behavioral Data Analysis.pdf
│ Conceptual discussion relating behavioral similarity structure to
│ physiological (EEG) responses
│
└── README.md

```

---

## EEG Preprocessing

The notebook  
**`single_subject_eeg_preprocessing_validation.ipynb`**  
demonstrates the EEG preprocessing workflow applied to a single subject for
validation and clarity.

Key steps include:
- Raw EEG inspection and sanity checks
- Bandpass filtering
- Artifact inspection and ICA-based cleaning
- Baseline correction
- Time–frequency (spectrogram) preparation

This notebook is intended as an **exploratory validation step**. The same
preprocessing logic was later adapted for multi-subject analysis.

---

## Behavioral Data Analysis

The `Behavioural Data Analysis/` directory contains notebooks analyzing behavioral
similarity ratings collected during the tactile perception experiment.

Included analyses:
- Preprocessing and aggregation of Likert-scale similarity ratings
- Construction of perceptual similarity matrices
- Multidimensional Scaling (MDS) to derive perceptual embedding spaces

These analyses provide **perceptual context** for interpreting EEG activity and
enable investigation of how neural responses relate to human tactile judgments.

---

## Experimental Design and Data Collection

Detailed information about the experiment is provided in the `report/` directory.

The report documents:
- Motivation and experimental rationale
- Tactile stimulus selection and trial structure
- Bias control and task design
- EEG acquisition using the Emotiv EPOC X headset
- Synchronization of EEG data with task events

This documentation is included to ensure **research transparency** and to clarify
how experimental design choices influence downstream EEG preprocessing and analysis.

---

## Notes

- Raw EEG data and participant information are not included.
- This repository focuses on preprocessing, analysis, and documentation rather than
  end-to-end classification performance.
- The project is intended as a research artifact demonstrating experimental and
  analytical methodology in EEG-based tactile perception studies.

---