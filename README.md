# UniversalCEFR

# 🇪🇺 EuroBERT Fine-Tuning for English and Welsh CEFR Classification

This repository contains multiple fine-tuning experiments using the **EuroBERT** language model for CEFR (Common European Framework of Reference) proficiency classification in **English** and **Welsh**.

---

## Repository Structure

### 🔹 `eurobert_en/`
Fine-tunes the **pre-trained EuroBERT** model on **English** data. The resulting model is saved for future use.

### 🔹 `eurobert_en_cy/`
Uses the previously fine-tuned **`eurobert_en`** model as a starting point and further fine-tunes it on **Welsh** data.

### 🔹 `eurobert_en_cy_B2/`
Also starts from the **`eurobert_en`** model but focuses specifically on fine-tuning it for **Welsh B2-level classification**.

### 🔹 `eurobert_cy_B2/`
Directly fine-tunes the **original EuroBERT** (not `eurobert_en`) on **Welsh B2-level** classification tasks.

---

## Key Notes

- All models build upon **EuroBERT**, a multilingual model trained on European languages.
- Welsh (`cy`) and English (`en`) datasets are used in varying combinations to test transfer learning effectiveness.
- The **B2 classifier** task targets the CEFR B2 proficiency level, a common benchmark for language assessments.

---

## Outputs

- Trained model checkpoints
- Evaluation metrics (accuracy, F1, etc.)
- Fine-tuned tokenizers and config files (if applicable)

---

## 🛠 Requirements

Install dependencies via:

```bash
pip install -r requirements.txt
