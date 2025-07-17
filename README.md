# Fine-Tune-for-Classification-and-NER
Finetuning Transformer based for Indonesian news classification and NER
## Classification
In here, I use IndoBERT, mBERT, and RoBERTa. This work is related with [Comparing-Embedding-Methods](https://github.com/ThomasArtemius/Comparing-Embedding-Methods) repository.
| Model    | Accuracy | F1 Score |
|----------|----------|----------|
| IndoBERT | **0.9378** | **0.9375** |
| mBERT    | 0.9279   | 0.9278   |
| RoBERTa  | 0.9297   | 0.9299   |

## NER
In here, I use IndoBERT, sBERT, and mBERT. Each model perform 2 finetuning methods (except IndoBERT, which has partial finetuning): Full finetuning and LoRA. This task is actually related with [Named-Entity-Recognition](https://github.com/ThomasArtemius/Named-Entity-Recognition) repository. Here is the result of token level accuracy:
| Model       | Full Fine-Tune | Partial Fine-Tune | PEFT Fine-Tune |
|-------------|----------------|--------------------|----------------|
| **IndoBERT**   | **0.94**         | **0.94**             | 0.92           |
| sBERT       | **0.91**         | —                  | 0.87           |
| mBERT       | **0.94**         | —                  | 0.90           |
