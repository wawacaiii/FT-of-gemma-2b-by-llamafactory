# 说明
## 项目介绍
该仓库存储的内容是作业复现的一部分，仅作为复现成果的说明，实际价值不大。  
代码中，gemma_lora_sft_otfq.yaml是Gemma-2B的QLoRA微调配置文件，包含了微调参数（模型路径、量化方式、数据集等）。  
./save/lora/sft文件夹中的内容是微调的输出文件，包含微调的模型配置、训练过程的相关信息。  
微调得到的模型超过上传限制，不在这里上传。
## 运行说明
如需复现此次结果：  
1、下载llama-factory源码；  
2、将gemma_lora_sft_otfq.yaml文件复制到目录中；  
3、下载gemma:2b模型，或修改配置文件从云端使用；  
4、在目录执行llamafactory-cli train ./gemma_lora_sft_otfq.yaml；  
llama-factory的使用说明参见对应仓库。  
