## Songs Genre Classification by Lyrics With BERT And LoRA


### Model 

For this project I am using 'bert-base-cased'.
It's pretrained model on English language using a masked language modeling (MLM) objective. It was introduced in <a href='https://arxiv.org/abs/1810.04805'>the paper</a> and first released in this repository. <a href='https://github.com/google-research/bert'>The model</a> is case-sensitive: it makes a difference between english and English.

### Parameter Efficient Finetuning 
I used <a href='https://opendelta.readthedocs.io/en/latest/index.html#'>opendelta library</a> for parameter efficient finetuning

```zsh
> Adapter 
trainable params: 903744 - all params: 109216323 - trainable: 0.827481% 
```

```zsh
> LoRA
trainable params: 294,912 - all params: 108,607,491 - trainable: 0.2715392808402139%
```

### Why use LoRA and not Adapter?

Well LoRA and QLoRA are very good for LLM I thought of using it in BERT to get a good understanding of how LoRA, Adapter work and I used LoRA for two reasons. The first was curiosity to know how the model would perform with a trainable percentage as low as 0.27%. The second reason was the lack of electricity and internet, so I needed faster training. Despite this, the resources did not allow me to see results.  Final training.


### Dataset

In this project I using <a href='https://www.kaggle.com/datasets/neisse/scrapped-lyrics-from-6-genres'>scrapped lyrics from 6 genres </a> and I selected Rap, Rock and Hip Hop 


### Note

I did not have the resources, such as the Internet, electricity, device, etc., to train the model well and choose the appropriate learning rate, so there were no results.


> To contribute to the project, please contribute directly. I am happy to do so, and if you have any comments, advice, job opportunities, or want me to contribute to a project, please contact me <a href='mailto:V3xlrm1nOwo1@gmail.com' target='blank'>V3xlrm1nOwo1@gmail.com</a>
