# Automated Clinical Documentation from Patient Encounters

## Overview

**Automated Clinical Documentation from Patient Encounters** is a project aimed at streamlining healthcare documentation by leveraging AI to generate structured medical notes from patient-doctor interactions. The project uses state-of-the-art NLP and machine learning techniques to understand conversations, organize details, and output clinical documentation ready for EHR (Electronic Health Record) systems.

## Features

- **Ambient AI transcription**: Converts clinician-patient conversations into structured notes.
- **Contextual summarization**: Extracts medical history, physician assessments, symptoms, and treatment plans.
- **Data extraction & EHR integration**: Organizes information for easy integration into EHRs.
- **Clinical coding support**: Assists with medical billing and compliance documentation.
- **Extensible model pipeline**: Built to support further customization for different clinical settings.

## Project Structure

- `/data` -- Example datasets and medical transcripts
- `/models` -- NLP/ML models for transcription, summarization, and coding
- `/scripts` -- Automation and preprocessing scripts
- `/notebooks` -- Jupyter/Colab notebooks for analysis and development

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/adikal25/Automated-Clinical-Documentation-from-Patient-Encounters.git
    cd Automated-Clinical-Documentation-from-Patient-Encounters
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Configure environment variables (see `.env.example`).

## Usage

- For **transcribing encounters**, place audio/text files in `/data` and run:
    ```bash
    python scripts/transcribe.py --input data/sample_encounter.wav
    ```
- For **generating clinical notes**, use:
    ```bash
    python scripts/generate_notes.py --input data/transcripts/
    ```
- Output structured clinical documentation will be saved to `/output`.


## citation
@inproceedings{dsw_2025,
 author = {Aline Gassenn and Luís Andrade and Douglas Teodoro and José Rodrigues-Jr},
 title = { Medical Dialogue Audio Transcription: Dataset and Benchmarking of ASR Models},
 booktitle = {Anais do VII Dataset Showcase Workshop},
 location = {Fortaleza/CE},
 year = {2025},
 pages = {71--82},
 publisher = {SBC},
 address = {Porto Alegre, RS, Brasil},
 doi = {10.5753/dsw.2025.248010},
 url = {https://sol.sbc.org.br/index.php/dsw/article/view/37199}
}

