# Renal CT Data Management and Sharing Plan

This repository demonstrates the NIH Data Management and Sharing Plan for the project on **Structured Radiology Report Generation from 3D Renal CT Scans**.

Due to HIPAA compliance and IRB restrictions, this repository does not contain:
- Raw patient CT imaging data
- Protected health information (PHI)
- Executable code processing sensitive data
Instead, it provides an example **Conda environment configuration** and documentation that illustrate how the computational environment for this project would be shared to support reproducibility and cross-platform use.

---

## Project Overview
This project focuses on:
- Managing de-identified 3D renal CT imaging data in compliance with HIPAA and institutional policies.
- Extracting structured clinical features from expert-annotated radiology reports using large language models (LLMs).
- Generating structured radiology reports from CT volumes and/or extracted clinical features using fine-tuned multimodal AI models.
- Following community standards (e.g., DICOM, RadLex, RSNA guidelines) for data formatting, terminology, and metadata.

While the raw data and processing scripts are not publicly available, the reproducibility principles demonstrated here apply directly to the actual project.

---

## Environment Configuration

The included `environment.yml` file specifies the core computational environment used in this project. It includes essential packages for medical image processing, deep learning, and natural language processing.

```bash
# Clone the repository
git clone https://github.com/renjie-liang/renal-ct-data-plan.git
cd renal-ct-data-plan

# Create and activate the Conda environment
conda env create -f environment.yml
conda activate renal-ct
