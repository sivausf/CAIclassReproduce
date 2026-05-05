# CAIclassLLMReproduce
Part of our reproducibility paper for LLM generated passcodes

You may use the ipynb notebook file linked in this repository to run all of the code and inference for the experiments. 

Instructions to set up: 

1. **Get access to Hugging Face Models**

Make sure you have access to huggingface models relevant for this project. The models can be found below:

pip install transformers accelerate
huggingface-cli login

Models used:

https://huggingface.co/mistralai/Mistral-7B-v0.1
https://huggingface.co/Qwen/Qwen2.5-14B
https://huggingface.co/google/gemma-7b
https://huggingface.co/meta-llama/Llama-2-7b
https://huggingface.co/meta-llama/Llama-2-13b
https://huggingface.co/meta-llama/Meta-Llama-3-8B

⚠️ Note: Llama and Gemma models may require access approval.

2. **Run the Notebook**

Open the notebook in Google Colab:

finalllm (2).ipynb

Then:

Run cells in order
Follow any instructions in the notebook
Ensure GPU runtime is enabled

Recommended:

A100 or H100 GPU
High RAM runtime

***What the Notebook Does***
Loads LLM models

Generates passphrases under different: temperature, top-p, prompt types (base, topic, entropy)

Stores outputs as JSON

****Computes:****
entropy metrics
filtering criteria
Runs LLM-as-judge evaluation

****Notes****
Generation is computationally expensive
Results may vary slightly due to randomness
Make sure output directories are correctly set
Output

****Results are saved as:****

JSON files (raw generations)
CSV files (aggregated metrics)


## Contributors

Part of CAI class reproducibility project.






## License

This project is open-source under the MIT License.
