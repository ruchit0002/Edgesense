# EdgeSense: On-Device Artificial Intelligence

## Overview

EdgeSense is an **on-device AI system** that performs sentiment analysis locally without relying on cloud-based inference.
The system uses a lightweight transformer model to analyze text and predict sentiment in real time while ensuring **low latency and user privacy**.

This project demonstrates how modern AI models can be optimized to run efficiently on local devices such as laptops and mobile phones.

---

## Problem Statement

Most AI applications today rely on cloud-based processing:

* User data is sent to remote servers
* High latency due to network dependency
* Privacy concerns with sensitive data
* Requires continuous internet connectivity

There is a need for AI systems that can operate **offline, fast, and securely on-device**.

---

## Solution

EdgeSense addresses this by:

* Running a pretrained NLP model locally
* Eliminating the need for internet connectivity
* Reducing response time
* Preserving user privacy

---

## Key Features

* On-device sentiment analysis (no cloud required)
* Fast inference with low latency
* Automatic dataset handling
* Accuracy and performance evaluation
* Interactive user input for real-time predictions

---

## How It Works

### 1. Dataset Loading

The system loads a sentiment dataset (`sst_train.csv`).

### 2. Data Processing

* Automatically detects text and label columns
* Cleans and converts labels into numerical format

### 3. Model Loading

A pretrained transformer model is loaded:

```text
distilbert-base-uncased-finetuned-sst-2-english
```

### 4. Inference

* Text is tokenized into numerical format
* Model predicts sentiment (Positive / Negative)

### 5. Evaluation

The system measures:

* Accuracy
* Inference time (latency)

---

## Workflow

```text
Dataset → Preprocessing → Model Inference → Prediction → Evaluation
```

---

## Example

Input:

```text
This movie is amazing
```

Output:

```text
Prediction: Positive
```

---

## Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* Pandas

---

## Installation

```bash
pip install torch transformers pandas
```

---

## Usage

Run the script:

```bash
python Edgesense.py
```

---

## Results

The system provides:

* Sentiment prediction
* Accuracy score
* Average inference time

Example:

```text
Accuracy: 91.0%
Average Inference Time: 110 ms
```

---

## Why This Project Matters

This project demonstrates:

* On-device AI deployment
* Privacy-preserving machine learning
* Efficient model usage on edge devices

It aligns with industry trends toward **Edge AI and local inference systems**.

---

## Future Improvements

* Model quantization for faster performance
* Multimodal input (text + voice)
* Deployment as a mobile or desktop application
* Hardware optimization using Apple ML frameworks

---

## Author

Ruchit Bhalekar
