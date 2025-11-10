# Modern AI with Unsloth.ai

## Course Information
- **Course**: CMPE-255 Data Mining (Section 47)
- **Semester**: Fall 2025
- **Due Date**: November 9, 2024, 11:59 PM

---

## Assignment Overview
This repository contains 5 colab notebooks demonstrating different LLM fine-tuning techniques using unsloth.ai:

1. **Full Fine-tuning** - Complete model parameter updates
2. **LoRA Fine-tuning** - Parameter efficient training
3. **RLHF (DPO)** - Reinforcement learning with human feedback
4. **GRPO** - Reasoning model training
5. **Continued Pre-training** - Teaching new languages/domains

---

## 📓 Colab Notebooks

### Colab 1: Full Fine-tuning
- **File**: `unsloath_full_finetuning.ipynb`
- **Model**: SmolLM2-135M
- **Method**: Full fine-tuning (all parameters updated)
- **Dataset**: Synthetic QA pairs from research paper
- **YouTube**: [Video Link]

### Colab 2: LoRA Fine-tuning
- **File**: `colab2_lora_finetuning.ipynb`
- **Model**: SmolLM2-135M
- **Method**: LoRA (Parameter Efficient Fine-tuning)
- **Dataset**: Same as Colab 1
- **YouTube**: [Video Link]

### Colab 3: RLHF with DPO
- **File**: `colab3_rlhf.ipynb`
- **Model**: SmolLM2 or Llama-3.2-3B
- **Method**: Direct Preference Optimization
- **Dataset**: Preferred and rejected responses
- **YouTube**: [Video Link]

### Colab 4: GRPO Reasoning
- **File**: `colab4_grpo_reasoning.ipynb`
- **Model**: SmolLM2 or reasoning model
- **Method**: Group Relative Policy Optimization
- **Dataset**: Math/coding problems
- **YouTube**: [Video Link]

### Colab 5: Continued Pre-training
- **File**: `colab5_continued_pretraining.ipynb`
- **Model**: Base LLM
- **Method**: Continued pre-training
- **Dataset**: New language/domain corpus
- **YouTube**: [Video Link]



---

## 🚀 Quick Setup

### Installation
```bash
pip install --upgrade uv
pip install unsloth vllm synthetic-data-kit==0.0.3
uv pip install transformers==4.56.2
uv pip install --no-deps trl==0.22.2
```

### GPU Requirements
- Full Fine-tuning: 8GB+ VRAM
- LoRA: 4GB+ VRAM
- RLHF/GRPO: 8GB+ VRAM

---

## 📁 Project Files
```
unsloath/
├── README.md
├── unsloath_full_finetuning.ipynb
├── colab2_lora_finetuning.ipynb
├── colab3_rlhf.ipynb
├── colab4_grpo_reasoning.ipynb
└── colab5_continued_pretraining.ipynb
```

---

## 🔑 Key Concepts

**Full Fine-tuning vs LoRA**
- Full: Updates all parameters, more accurate, slower
- LoRA: Only trains adapters, 90% less memory, faster

**RLHF vs GRPO**
- RLHF (DPO): Uses labeled preferred/rejected pairs
- GRPO: Model generates and evaluates its own outputs

---

## 📚 References

**Official Documentation**
- [Unsloth Documentation](https://docs.unsloth.ai/)
- [Fine-tuning Guide](https://docs.unsloth.ai/get-started/fine-tuning-llms-guide)
- [RL Guide](https://docs.unsloth.ai/get-started/reinforcement-learning-rl-guide)
- [Continued Pre-training](https://docs.unsloth.ai/basics/continued-pretraining)

**GitHub & Tutorials**
- [Unsloth Notebooks](https://github.com/unslothai/notebooks/)
- [Kaggle Tutorial](https://www.kaggle.com/code/kingabzpro/fine-tuning-llms-using-unsloth)
- [Ollama Export Guide](https://docs.unsloth.ai/tutorials/how-to-finetune-llama-3-and-export-to-ollama)

