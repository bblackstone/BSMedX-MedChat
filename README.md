# MedChat: Medical Image Analysis with Fine-tuned LLaMa-3.2-11B-Vision-Instruct

This Colab notebook demonstrates fine-tuning the LLaMa-3.2-11B-Vision-Instruct model for medical image analysis using the Radiology_mini dataset and then deploys the fine-tuned model using Streamlit.


## Description

This notebook showcases how to:

1. **Install necessary libraries** like `transformers`, `trl`, `datasets`, `unsloth`, `torch`, `streamlit`, `pyngrok`, and `nvidia-tensorrt`.
2. **Load the pre-trained LLaMa-3.2-11B-Vision-Instruct model** and tokenizer from Hugging Face Model Hub.
3. **Prepare the dataset** by converting it to conversation format suitable for fine-tuning.
4. **Fine-tune the model** with LoRA (Low-Rank Adaptation) to specialize in medical image analysis.
5. **Run inference** with the fine-tuned model to analyze new medical images and generate descriptive insights.
6. **Save the fine-tuned model** and push it to the Hugging Face Hub.
7. **Deploy the model** using Streamlit for interactive use.


## Usage

1. **Set your Hugging Face access token:** Create a `HF_TOKEN` secret in Colab and store your Hugging Face token there.
2. **Set your ngrok authtoken:** Create a `NG_TOKEN` variable and store your ngrok token there.
3. **Run all cells:** Execute all the code cells in the notebook sequentially.
4. **Access the Streamlit app:** Use the ngrok public URL generated in the last cell to access the interactive app.


## Notes

* The notebook utilizes LoRA for efficient fine-tuning, minimizing memory requirements.
* The Radiology_mini dataset is used for demonstration purposes. You can replace it with your own dataset for specific use cases.
* The fine-tuned model is saved locally and can be pushed to the Hugging Face Hub for sharing and reuse.
* The Streamlit app provides a user-friendly interface for image upload and analysis.

## Disclaimer

This is a research-focused notebook and the results should be considered for experimental purposes. Always consult with medical professionals for clinical decision-making
