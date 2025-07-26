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

## 🧪 How to Use

```python
from transformers import GPT2Tokenizer, GPT2LMHeadModel

# Load model and tokenizer
tokenizer = GPT2Tokenizer.from_pretrained("swapnilbanduke/Medical_Symtoms")
model = GPT2LMHeadModel.from_pretrained("swapnilbanduke/Medical_Symtoms")

# Prompt
input_text = "Diabetes"
input_ids = tokenizer.encode(input_text, return_tensors="pt")

# Generate output
output = model.generate(
    input_ids,
    max_length=50,
    do_sample=True,
    top_k=50,
    top_p=0.95,
    temperature=0.7
)

# Decode and print
print(tokenizer.decode(output[0], skip_special_tokens=True))

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
