# 研究学习

## 代码偏好
The **single model file policy** states that all code necessary for the forward pass of a model is in one and only one file - called the model file. If a reader wants to understand how BERT works for inference, she should only have to look into BERT's modeling_bert.py file. We usually reject any attempt to abstract identical sub-components of different models into a new centralized place. We don't want to have a attention_layer.py that includes all possible attention mechanisms. 

we directly put the attention function in the corresponding modeling file.

跟我的偏好非常相符！！！

## TODO
1. 跑通bert预训练代码 
   google search word: pretraining a transformer from scratch with transformers
   参考 https://www.thepythoncode.com/article/pretraining-bert-huggingface-transformers-in-python
        https://huggingface.co/blog/pretraining-bert
        https://towardsdatascience.com/how-to-train-a-bert-model-from-scratch-72cfce554fc6
        https://d2l.ai/chapter_attention-mechanisms-and-transformers/large-pretraining-transformers.html(d2l学习)


## 参考资料
1. https://huggingface.co/blog/transformers-design-philosophy