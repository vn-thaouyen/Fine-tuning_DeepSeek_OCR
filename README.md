# Fine-Tuning DeepSeek-OCR for Vietnamese Handwritten Text

This project fine-tunes the DeepSeek-OCR model to improve recognition performance on Vietnamese handwritten text.

## Course
This project is completed as part of: Introduction to Natural Language Processing

## Project Structure
- 23127542.ipynb: Notebook containing source code 
- ocr_results_per_images.csv: Detailed OCR outputs including CER and WER metrics for each test image (Baseline)
- ocr_metrics_summary.csv: Statistical summary (Mean, Median, Std, Max, Min) of CER and WER across the full test set (Baseline)
- ocr_results_per_images_fine-tuned.csv: Detailed OCR outputs including CER and WER metrics for each test image (Fine-tuned)
- ocr_metrics_summary_fine-tuned.csv: Statistical summary (Mean, Median, Std, Max, Min) of CER and WER across the full test set (Fine-tuned)

## Objective
- Adapt a pre-trained Vision-Language OCR model to Vietnamese handwritten data
- Improve recognition accuracy through parameter-efficient fine-tuning
- Compare the original and fine-tuned models using quantitative and qualitative evaluation

## Methodology
- Collected and preprocessed Vietnamese handwritten OCR dataset   
- Applied LoRA-based fine-tuning using Unsloth  
- Tuned hyperparameters (learning rate, batch size, training steps)  
- Evaluated models on an independent test set  

## Evaluation
- Metric: Character Error Rate (CER)
- Compared:
  - Original DeepSeek-OCR model
  - Fine-tuned model
- Conducted error analysis on common Vietnamese recognition issues

## Tools & Frameworks
- Python
- PyTorch
- HuggingFace Transformers
- Unsloth
- Google Colab

## Results
Fine-tuning improved OCR performance on Vietnamese handwritten text, reducing character-level recognition errors compared to the baseline model and completely eliminated halluciation observerd in the baseline model
