# Solo Summarizer

Solo Summarizer is a text summarization system based on fine-tuning Text-to-Text Transformer (T5) models. This project aims to develop an efficient text summarization system that generates coherent and concise summaries for long documents.

## Overview

This project consists of several phases:
1. Fine-tuning the T5-small model on the BillSum dataset and assessing its performance.
2. Fine-tuning and comparing the performance of T5-base and FLAN-T5-base models on the same dataset.
3. Investigating the factors influencing the text summarization capabilities of each model.
4. Exploring methods to improve the performance of the selected model and applying the system to other domains and datasets.

## Usage

Clone this repository, install the requirements, and then run the provided Jupyter Notebooks to fine-tune the T5 models on the BillSum dataset. The notebooks will guide you through the entire process of data preprocessing, training, and generating summaries.

## Dependencies

This project uses the following libraries:
- Hugging Face Transformers
- Hugging Face Datasets
- PyTorch
- PyTorch Lightning
- Rouge Score

## Results

### Phase 1:
The initial fine-tuning of the T5-small model on the BillSum dataset yielded promising results, with a Rouge1 score of 0.1436, Rouge2 score of 0.0514, RougeL score of 0.1188, and RougeLsum score of 0.119 on the evaluation set.

### Phase 2:
The fine-tuning and comparison of the T5-base and FLAN-T5-base models on the BillSum dataset provided valuable insights into their performance. The T5-base model showed an initial improvement but exhibited odd behavior after the first two epochs. The FLAN-T5-base model faced challenges such as a lack of recorded training loss. Further investigation and optimization are planned for the final phase of the project.

### Phase 3:
In this phase, we focused on optimizing the T5-base and FLAN-T5-base models, addressing the issues encountered during Phase 2. The optimizations led to improved performance on the BillSum dataset, and the final results were achieved. A detailed analysis of the model performance and comparison between the two models can be found in the project report.

## License

This project is licensed under the MIT License.

## Acknowledgements

- Hugging Face Summarization Tutorial
- Transformer models and the BillSum dataset from the Hugging Face Transformers library and Hugging Face Datasets
- Key papers: T5, FLAN-T5, ROUGE, BLEU, Attention is All You Need