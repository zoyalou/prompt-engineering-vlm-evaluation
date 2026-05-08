# Chart Visual Question Answering with Open-Source Multimodal Models

## Overview

This project explores how well open-source Large Multimodal Models (LMMs) perform on chart-based visual question answering (VQA) tasks. The focus of the project is evaluating whether models can accurately interpret histogram visualizations and answer statistical questions, such as identifying medians or trends from graphical data.

The project investigates different prompting strategies and compares model outputs across multiple evaluation settings to better understand the strengths and limitations of multimodal reasoning systems.

---

## Objectives

* Evaluate the ability of open-source multimodal models to interpret histogram data
* Compare different prompting strategies for chart reasoning tasks
* Analyze model accuracy and response quality
* Build a lightweight evaluation pipeline for visual question answering experiments
* Explore practical applications of multimodal AI in data interpretation and analytics

---

## Technologies Used

* Python
* Jupyter Notebook
* Hugging Face Transformers
* Pandas
* PIL (Python Imaging Library)
* Qwen2.5-VL-3B-Instruct
* Hugging Face Datasets

---

## Dataset

This project uses histogram-based visual question answering datasets from Hugging Face.

Example dataset source:

* `ReadingTimeMachine/visual_qa_histograms`

The dataset contains histogram images paired with statistical reasoning questions and expected answers.

---

## Methodology

### 1. Data Preparation

* Loaded histogram datasets and image files
* Processed CSV metadata containing questions and expected answers
* Organized image-question-answer pairs for evaluation

### 2. Model Evaluation

Tested the performance of open-source multimodal models using multiple prompting techniques:

* Zero-shot prompting
* Structured prompting
* Chain-of-thought prompting

The model generated answers based on histogram images and accompanying prompts.

### 3. Evaluation Pipeline

An evaluation workflow was built to:

* Run inference across multiple examples
* Compare predicted answers with expected outputs
* Categorize response quality
* Summarize model performance across prompting methods

---

## Example Tasks

The model was evaluated on tasks such as:

* Estimating medians from histograms
* Interpreting distributions
* Identifying trends and patterns
* Answering statistical reasoning questions from chart data

---

## Results

The experiments showed that prompting strategy significantly impacts model performance.

Observed response quality categories included:

* Very Accurate
* Reasonable
* Poor
* Incorrect

Structured and chain-of-thought prompting occasionally improved reasoning quality compared to zero-shot prompting, although performance varied depending on chart complexity.

---

## Key Takeaways

* Multimodal models show promising capabilities for chart understanding tasks
* Prompt engineering plays an important role in reasoning accuracy
* Histogram interpretation remains challenging for smaller open-source models
* Evaluation pipelines are essential for systematically comparing multimodal reasoning performance

---

## Future Improvements

Potential future directions include:

* Expanding evaluation to additional chart types
* Testing larger multimodal models
* Improving automated scoring methods
* Fine-tuning models on chart-specific datasets
* Exploring retrieval-augmented or few-shot approaches

---

## Repository Structure

```text
├── notebooks/
│   ├── project.ipynb
│   └── testing_vqa.ipynb
│   └── hist_error_benchmark.ipynb
├── data/
│   ├── histograms/
│     └──  plot1.png
│     └──  hist_larger_parsed.csv
│     └──  hist_complex_parsed.csv
├── results/
│   ├── quality_summary.csv
│   └── generated_outputs.csv
├── README.md
└── requirements.txt
```

---

## Running the Project

### Clone the Repository

```bash
git clone <repository-url>
cd <repository-name>
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook and run the evaluation pipeline.

---

## Skills Demonstrated

This project demonstrates experience with:

* Multimodal AI systems
* NLP and prompt engineering
* Data preprocessing and evaluation
* Machine learning experimentation
* Model analysis and benchmarking
* Python-based AI workflows

---

## Acknowledgements

* Hugging Face
* Qwen Team
* Open-source multimodal AI research community

