# paper2summary
This repository contains **LoRA fine-tuning scripts** for the Llama-3.2-1B-Instruct model on scientific paper summarization.  
The fine-tuned model is available on Hugging Face: [gabe-zhang/Llama-PaperSummarization-LoRA](https://huggingface.co/gabe-zhang/Llama-PaperSummarization-LoRA)


## **Performance Comparison**
| Model                     | ROUGE-1 | ROUGE-2 | ROUGE-3 | ROUGE-L |
|---------------------------|----------|----------|----------|----------|
| **Llama-3.2-1B-Instruct** | 36.69    | 7.47     | 1.95     | 19.36    |
| [**Llama-PaperSummarization-LoRA**](https://huggingface.co/gabe-zhang/Llama-PaperSummarization-LoRA) | **41.56** | **11.31** | **2.67** | **21.86** |

The model was evaluated on a **6K-sample test set** using **ROUGE scores** with beam search (beam size = 4)


## **Dataset**
The model was fine-tuned on the [**armanc/scientific_papers**](https://huggingface.co/datasets/armanc/scientific_papers) dataset. Below are the details of the dataset splits:
- **Training Set**: 20K samples
- **Validation Set**: 6K samples
- **Test Set**: 6K samples


## License 
- **Llama 3.2 base model**: The Llama 3.2 model is subject to the [Llama 3.2 Community License](https://www.llama.com/llama-downloads). Please ensure compliance with the Llama 3.2 license when downloading and using the Llama model.
- **LoRA fine-tuning code**: Licensed under the [MIT License](./LICENSE).
