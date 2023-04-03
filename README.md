** Converted model for GPTQ from https://huggingface.co/lmsys/vicuna-13b-delta-v0 **

* IMPORTANT NOTE: Use the .safetensors model unless it does not work. In which case, try .pt.

GPTQ conversion command (on CUDA branch):
CUDA_VISIBLE_DEVICES=0 python llama.py ../lmsys/vicuna-13b-v0 c4 --wbits 4 --true-sequential --groupsize 128 --save vicuna-13b-4bit-128g.pt

Added 1 token to the tokenizer model:
python llama-tools/add_tokens.py lmsys/vicuna-13b-v0/tokenizer.model /content/tokenizer.model llama-tools/test_list.txt

Use of Oobabooga with these tags:
--wbits 4
--groupsize 128

Enjoy