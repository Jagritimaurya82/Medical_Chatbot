# Medical_Chatbot

# STEPS to run the project

Clone the repository
```bash
git clone https://github.com/Jagritimaurya82/Medical_Chatbot.git
```
 
## STEP 01- Create a conda environment after opening the repository

```bash
conda create -n mchatbot python=3.8 -y
```

```bash
conda activate mchatbot  
```

## STEP 02- install the requirements
```bash
pip install -r requirements.txt
```

## Create a .env file in the root directory and add your Pinecone credentials as follows:
```bash
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```

## Download the quantize model from the link provided in model folder & keep the model in the model directory:
```bash
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

```bash
# run the following command
python store_index.py
```
```bash
# Finally run the following command
python app.py
```
```bash
open up localhost:
```
## Techstack Used:
Python
LangChain
Flask
Meta Llama2
Pinecone