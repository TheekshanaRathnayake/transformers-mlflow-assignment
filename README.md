# 🤖 Transformers and MLflow: Downstream Tasks and Experiment Tracking

**Date:** March 2026
**Module:** AI Concepts and Tools
**Coursework Type:** Assignment
**Student Name:** Theekshana Thathsara Rathnayake
**Institution:** Informatics Institute of Technology

---

## 📌 Project Overview

This project demonstrates the practical use of **pretrained transformer models** for solving multiple Natural Language Processing (NLP) tasks. It also integrates **MLflow** to track experiments, log parameters, and compare results across different runs.

The implementation follows a structured approach similar to real-world machine learning workflows.

---

## 🎯 Objectives

* Apply pretrained transformer models to downstream NLP tasks
* Perform inference using Hugging Face pipelines
* Track experiments using MLflow
* Compare multiple runs systematically
* Store outputs and observations as artifacts

---

## 🛠️ What Was Implemented

### ✔ Data Preparation

* Created custom datasets for all tasks
* Ensured required inputs:

  * 20 sentences (Sentiment)
  * 10+ paragraphs (NER)
  * 5 prompts (Text Generation)

### ✔ Model Inference

* Used Hugging Face `pipeline()` API
* Ran inference on all datasets
* Processed predictions and outputs

### ✔ Experiment Tracking (MLflow)

* Created experiment:

  ```
  Transformers_Downstream_Tasks
  ```
* Logged:

  * Parameters
  * Metrics
  * Artifacts
* Created **two runs per task** for comparison

---

## 🧠 Models Used

| Task                     | Model                                             | Purpose                 |
| ------------------------ | ------------------------------------------------- | ----------------------- |
| Sentiment Analysis       | `distilbert-base-uncased-finetuned-sst-2-english` | Classify text sentiment |
| Named Entity Recognition | `dslim/bert-base-NER`                             | Extract entities        |
| Text Generation          | `gpt2`                                            | Generate text           |

---

## 🔧 Tasks and Results

### 1️⃣ Sentiment Classification

* Processed 20 labeled sentences
* Generated predictions and confidence scores
* Calculated accuracy

#### 📊 Results

* Accuracy: **95%**
* Run 1: Default pipeline
* Run 2: Reduced `max_length`

#### 📦 MLflow Logging

* model_name
* num_samples
* accuracy
* predictions (CSV)

---

### 2️⃣ Named Entity Recognition (NER)

* Processed 10+ paragraphs
* Extracted:

  * Person
  * Organization
  * Location

#### 📊 Results

* Run 1: **More entities (fragmented tokens)**
* Run 2: **Cleaner entities (better grouping)**

#### 📦 MLflow Logging

* model_name
* total_entities
* entity distribution
* output files (CSV + JSON)

---

### 3️⃣ Text Generation

* Generated outputs for 5 prompts
* Compared results using different parameters

#### ⚙️ Parameters Compared

* Temperature
* Max length

#### 📊 Observations

* Run 1: More repetitive output
* Run 2: More coherent and structured output

#### 📦 MLflow Logging

* parameters
* generated outputs (CSV)
* observations (TXT)

---

## 📊 MLflow Experiment Tracking

All runs are tracked under:

```
Transformers_Downstream_Tasks
```

For each task:

* ✔ Two runs created
* ✔ Parameters logged
* ✔ Metrics recorded
* ✔ Artifacts saved

This allows clear comparison between different configurations.

---

## 📂 Project Structure

```
transformers-mlflow-assignment/
│
├── transformers_mlflow_downstream_tasks.ipynb
├── README.md
├── requirements.txt
├── .gitignore
│
├── artifacts/
│   ├── task1_sentiment/
│   ├── task2_ner/
│   └── task3_text_generation/
│
├── screenshots/
│   ├── task1_runs.png
│   ├── task2_runs.png
│   ├── task3_runs.png
│
└── notebook_pdf/
    └── transformers_mlflow_downstream_tasks.pdf
```

---

## 🚀 How to Run the Project

### 1. Install dependencies

```
pip install -r requirements.txt
```

### 2. Run the notebook

```
jupyter notebook
```

### 3. Start MLflow

```
mlflow ui
```

### 4. Open MLflow UI

```
http://127.0.0.1:5000
```

---

## 📸 MLflow Screenshots

Includes:

* Task 1 comparison (2 runs)
* Task 2 comparison (2 runs)
* Task 3 comparison (2 runs)

---

## 📄 Deliverables

* ✔ Jupyter Notebook (with outputs)
* ✔ MLflow tracking
* ✔ Comparison screenshots
* ✔ PDF version of notebook
* ✔ GitHub repository

---

## ✅ Conclusion

This project demonstrates how transformer models can be applied to multiple NLP tasks and highlights the importance of **MLflow for experiment tracking and comparison**.

Key takeaways:

* Transformer models are versatile and powerful
* MLflow enables structured experiment management
* Parameter tuning impacts model outputs

---


