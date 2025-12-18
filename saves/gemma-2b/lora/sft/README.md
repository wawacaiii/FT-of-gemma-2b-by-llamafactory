---
library_name: peft
license: other
base_model: ./models/gemma-2b
tags:
- base_model:adapter:./models/gemma-2b
- llama-factory
- lora
- transformers
pipeline_tag: text-generation
model-index:
- name: sft
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft

This model is a fine-tuned version of [./models/gemma-2b](https://huggingface.co/./models/gemma-2b) on the alpaca_en_demo dataset.
It achieves the following results on the evaluation set:
- Loss: 1.5093

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 1
- eval_batch_size: 4
- seed: 42
- gradient_accumulation_steps: 8
- total_train_batch_size: 8
- optimizer: Use paged_adamw_8bit with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: cosine
- lr_scheduler_warmup_ratio: 0.1
- num_epochs: 3.0
- mixed_precision_training: Native AMP

### Training results



### Framework versions

- PEFT 0.17.0
- Transformers 4.57.3
- Pytorch 2.5.1+cu121
- Datasets 3.0.0
- Tokenizers 0.22.1