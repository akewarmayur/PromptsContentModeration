# Content Moderation of Generative AI prompts
### Implementation of the paper "Content Moderation of Generative AI Prompts, Springer’s SN Computer Science, 2023"
Here, we provide a framework for analyzing the text prompts based on the content moderation taxonomy. We define the taxonomy for content moderation and explore different language models to classify the prompt as per the moderation taxonomy. The proposed moderation taxonomy can be used to analyze user’s behavior and misuse of any generative AI application. 

### Keyword Identification 
Keyword identification for content moderation is a fundamental process that involves identifying specific words, phrases, or terms that may violate platform guidelines or community standards. These keywords are crucial in flagging or filtering out inappropriate or harmful content. Content moderation systems use keyword lists to detect and address various issues, including hate speech, profanity, explicit content, and more. 

### Zero Shot Text Classification
We defined the labels as mild sexuality, intense sexuality; full nudity, partial nudity; blood and gore violence, physical violence, weapon use, animal violence, state of violence victim; alcohol use, hard drugs use, prescription use; cigarette smoking, marijuana or tobacco use; profanity and hate speech, hate towards humanity. These labels are passed to the zero-shot BART model [27] along with the prompt which results in the moderation category. 

### Text Classification Model
We used the manually annotated data for fine-tuning the BERT model. Following are the results of fine-tuning for different prompt categories.

#### Data
Find the manually annotated data in the `Data` folder

### Code
* Find the keyword process code in `keywordBasedClassification.py` file
* Find the keyword process code in `zeroShotClassification.py` file
### Jupyter Notebooks
* Find the BERT fine-tune process notebook [here](https://platform.openai.com/account/api-keys](https://github.com/akewarmayur/PromptsContentModeration/blob/main/notebooks/BertFineTune.ipynb)https://github.com/akewarmayur/PromptsContentModeration/blob/main/notebooks/BertFineTune.ipynb)

### Citation
If you find this code useful in your research, please consider citing it as:
```
@misc{akewarmayur/PromptsContentModeration,
  author = {Mayur Akewar, Prof. Praful Pardhi},
  title = {PromptsContentModeration },
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub Repository},
  howpublished = {\url{https://github.com/akewarmayur/PromptsContentModeration}},
}
```

