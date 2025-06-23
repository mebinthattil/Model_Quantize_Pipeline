# Model_Quantize_Pipeline
An automated script for taking a llama family of models from HF and then quantizing it and running it in chat mode. This automatically selects the best way to go about it based on the hardware that you use to run it.

## Steps to run
1. First clone this repo: `git clone git@github.com:mebinthattil/Model_Quantize_Pipeline.git`
2. cd into the repo: `cd Model_Quantize_Pipeline`
3. setup and activate a python venv called `llama-venv` strictly using python version 3.10.
  This would look something like this: `/your/python/path/to/python3.10 -m venv llama-venv ; source llama-venv/bin/activate`
4. Finally set permissions and run this script: `chmod +x setup_script.sh; ./setup_script.sh`

## Some pre-requisites:
1. HF CLI must be authenticated
2. Git must be setup right
3. I think thats it XD

## Why was this made
Well surely a script for this was not needed, but I like scripts. Also laying out a pipeline like this makes it easier for me to quickly quantize models and test out their performance. Since its hooked up to HF models, this makes my job a whole lot easier. I can also monitor the size of models quickly after quantization. 
