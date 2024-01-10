# [ACL2023] Is GPT-3 a Good Data Annotator?

The repo is the source code for [Is GPT-3 a Good Data Annotator?](https://aclanthology.org/2023.acl-long.626/)

Bosheng Ding, Chengwei Qin, Linlin Liu, Yew Ken Chia, Boyang Li, Shafiq Joty, Lidong Bing

Accepted at 61th Annual Meeting of the Association for Computational Linguistics (ACL'23).

## Setup

### 1. Download the code

```
git clone https://github.com/DAMO-NLP-SG/LLM-Data-Annotator
cd LLM-Data-Annotator
```

### 2. Install dependencies

```
pip install -r requirements.txt
```

### 3. Run code
The files under the '**prompt**' folder are prompts used in our work for different methods and the files under the '**data**' folder are training data for different methods.

#### 3.1. FewRel

```
cd FewRel/code

```
For FewRel, we wrote a simple relation extraction code, main.py to run our experiments. You may follow the instructions in the FewRel folder to write the code.



#### 3.2. SST2

```
cd SST2
```
For SST2 we used the codebase from https://github.com/YJiangcm/SST-2-sentiment-analysis to run our experiments.


#### 3.3. ASTE

```
cd ASTE
```
For ASTE we used the codebase from https://github.com/chiayewken/Span-ASTE to run our experiments.

#### 3.4 CrossNER

```
cd CrossNER
```
For CrossNER we used the codebase from https://github.com/allanj/pytorch_neural_crf to run our experiments.




## Citation

If you find our paper or this project helps your research, please kindly consider citing our paper in your publication.




```
@inproceedings{ding-etal-2023-gpt,
    title = "Is {GPT}-3 a Good Data Annotator?",
    author = "Ding, Bosheng  and
      Qin, Chengwei  and
      Liu, Linlin  and
      Chia, Yew Ken  and
      Li, Boyang  and
      Joty, Shafiq  and
      Bing, Lidong",
    editor = "Rogers, Anna  and
      Boyd-Graber, Jordan  and
      Okazaki, Naoaki",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-long.626",
    doi = "10.18653/v1/2023.acl-long.626",
    pages = "11173--11195",
    abstract = "Data annotation is the process of labeling data that could be used to train machine learning models. Having high quality annotation is crucial, as it allows the model to learn the relationship between the input data and the desired output. GPT-3, a large-scale language model developed by OpenAI, has demonstrated im- impressive zero- and few-shot performance on a wide range of NLP tasks. It is therefore natural to wonder whether it can be used to effectively annotate data for NLP tasks. In this paper, we evaluate the performance of GPT-3 as a data annotator by comparing it with traditional data annotation methods and analyzing its output on a range of tasks. Through this analysis, we aim to provide insight into the potential of GPT-3 as a general-purpose data annotator in NLP.",
}
```

