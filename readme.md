# 🧠 Medical_Symptoms – Fine-Tuned GPT2 Model for Symptom Generation

A fine-tuned DistilGPT2 model trained to generate **medical symptoms** when given a disease or condition name. Ideal for building healthcare chatbots, education tools, or assisting in exploratory medical NLP tasks.

---

## ✨ Example Usage

**Input:**  

Bronchitis


**Output:**  
Bronchitis | Persistent cough with yellow or green mucus, chest tightness, wheezing



---

## 📦 Model Details

| Attribute         | Value                    |
|------------------|--------------------------|
| Base Model       | distilgpt2               |
| Architecture     | GPT2LMHeadModel          |
| Model Size       | 81.9M parameters          |
| Language         | English                  |
| Format           | PyTorch (`.bin` format)  |
| Tokenizer        | GPT2Tokenizer            |
| Task             | Text Generation (Symptoms) |
| Fine-tuned by    | [Swapnil Banduke](https://www.linkedin.com/in/swapnilbanduke/) |

---


📦 Medical_Symtoms
├── config.json
├── model_weights.bin
├── tokenizer_config.json
├── special_tokens_map.json
├── merges.txt
├── vocab.json

@model{swapnil_medical_symptoms_2025,
  author       = {Swapnil Banduke},
  title        = {Medical_Symptoms - Fine-tuned GPT2 for Medical Symptom Generation},
  year         = 2025,
  url          = {https://huggingface.co/swapnilbanduke/Medical_Symtoms}
}
