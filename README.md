# [Improving Question Answering Model Robustness with Synthetic Adversarial Data Generation](https://aclanthology.org/2021.emnlp-main.696/)

This repository contains resources derived from "Improving Question Answering Model Robustness with Synthetic Adversarial Data Generation" ([https://aclanthology.org/2021.emnlp-main.696/](https://aclanthology.org/2021.emnlp-main.696/))

<img src="https://github.com/maxbartolo/improving-qa-model-robustness/raw/main/img/pipeline.png" alt="Synthetic Adversarial Data Pipeline" width="480"/>

## Datasets
- SynQA: https://github.com/maxbartolo/improving-qa-model-robustness/raw/main/data/synQA.zip
- Answer Candidates: https://github.com/maxbartolo/improving-qa-model-robustness/raw/main/data/answer_candidates.zip

For further details, refer to the `README.md` files associated with each dataset. For any further technical details, kindly refer to the paper.

## Models
- RoBERTa-Large SynQA: https://huggingface.co/mbartolo/roberta-large-synqa
- RoBERTa-Large SynQAExt: https://huggingface.co/mbartolo/roberta-large-synqa-ext
- ELECTRA-Large SynQA: https://huggingface.co/mbartolo/electra-large-synqa

The ELECTRA-Large SynQA model is the adversarial model-in-the-loop of round 3 of the QA task on [Dynabench](https://dynabench.org/). If you would like to try coming up with questions that the model cannot answer correctly, check out: https://dynabench.org/tasks/qa/create.


## Citation
If you use this work, please consider citing:

```
@inproceedings{bartolo-etal-2021-improving,
    title = "Improving Question Answering Model Robustness with Synthetic Adversarial Data Generation",
    author = "Bartolo, Max  and
      Thrush, Tristan  and
      Jia, Robin  and
      Riedel, Sebastian  and
      Stenetorp, Pontus  and
      Kiela, Douwe",
    booktitle = "Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing",
    month = nov,
    year = "2021",
    address = "Online and Punta Cana, Dominican Republic",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.emnlp-main.696",
    doi = "10.18653/v1/2021.emnlp-main.696",
    pages = "8830--8848",
    abstract = "Despite recent progress, state-of-the-art question answering models remain vulnerable to a variety of adversarial attacks. While dynamic adversarial data collection, in which a human annotator tries to write examples that fool a model-in-the-loop, can improve model robustness, this process is expensive which limits the scale of the collected data. In this work, we are the first to use synthetic adversarial data generation to make question answering models more robust to human adversaries. We develop a data generation pipeline that selects source passages, identifies candidate answers, generates questions, then finally filters or re-labels them to improve quality. Using this approach, we amplify a smaller human-written adversarial dataset to a much larger set of synthetic question-answer pairs. By incorporating our synthetic data, we improve the state-of-the-art on the AdversarialQA dataset by 3.7F1 and improve model generalisation on nine of the twelve MRQA datasets. We further conduct a novel human-in-the-loop evaluation and show that our models are considerably more robust to new human-written adversarial examples: crowdworkers can fool our model only 8.8{\%} of the time on average, compared to 17.6{\%} for a model trained without synthetic data.",
}
```

## License
This datasets are licensed under the MIT License (https://opensource.org/licenses/MIT). For details on model licensing, kindly refer to their respective model cards.
