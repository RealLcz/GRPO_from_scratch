# GRPO from scratch
This repo contains codes and training results of a pure pytorch implementation of GRPO. 

To run my code, you may first set up the environment as required :

```pip install -r requirements.txt```

After that, you could directly use script :

```python3 standard.py```

## Summary

Small Language Model (SLMs) like o.5B or 1.5B models' ability to follow instructions is very weak. For example, we may use SYSTEM_PROMPT like
```
按照如下格式回答问题：
<think>
你的思考过程
</think>
<answer>
你的回答
</answer>
```
However, SLMs may not follow your required template at first. After training for roughly 200 steps, SLMs will gradually learn to follow your demand but not accurately.


## Training settings

### Foundation Models
Qwen/Qwen2.5-1.5B-Instruct  [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Hugging%20Face-FFD21E?logo=huggingface&logoColor=000)](https://huggingface.co/Qwen/Qwen2.5-0.5B-Instruct)


### Training Benchmark
swulling/gsm8k_chinese  [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Hugging%20Face-FFD21E?logo=huggingface&logoColor=000)](https://huggingface.co/datasets/swulling/gsm8k_chinese)


## Training Results
Digit Reward Mean
<img width="2528" height="1328" alt="W B Chart 2026_2_13 02_36_10" src="https://github.com/user-attachments/assets/c5f93422-e61c-419f-bb5c-c3f4b603c4da" />

Mark Reward Mean
<img width="2528" height="1328" alt="W B Chart 2026_2_13 02_35_53" src="https://github.com/user-attachments/assets/d0ff2a79-0253-4ad6-a220-33c527f33784" />


<img width="2528" height="1328" alt="W B Chart 2026_2_13 02_38_14" src="https://github.com/user-attachments/assets/040121de-5e89-4fd6-8187-68c799e14c69" />
<img width="2528" height="1328" alt="W B Chart 2026_2_13 02_38_26" src="https://github.com/user-attachments/assets/c0981ad7-d580-4ef9-9241-5eddd36bccc2" />
<img width="2528" height="1328" alt="W B Chart 2026_2_13 02_38_37" src="https://github.com/user-attachments/assets/29d4f060-59d7-4df5-b74e-22521e4bc967" />


More specific results are available at https://wandb.ai/changzhiliu1-uestc/grpo/workspace?nw=nwuserchangzhiliu1

