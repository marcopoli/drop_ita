# Italian version of the DROP Dataset
Dataset based on the Italian translation provided by:

 - **Leonardo Ranaldi, Giulia Pucci, Elena Sofia Ruzzetti, Fabio Massimo Zanzotto, and André Freitas** - [Teasing LLMs adapted to Italian](https://github.com/LeonardRanaldi/italian-instruct-eval/tree/main)
 
 # Citations 
  ```
@inproceedings{Dua2019DROP,
  author={Dheeru Dua and Yizhong Wang and Pradeep Dasigi and Gabriel Stanovsky and Sameer Singh and Matt Gardner},
  title={  {DROP}: A Reading Comprehension Benchmark Requiring Discrete Reasoning Over Paragraphs},
  booktitle={Proc. of NAACL},
  year={2019}
}

@inproceedings{RanaldiPRZF23,
  author       = {Leonardo Ranaldi and
                  Giulia Pucci and
                  Elena Sofia Ruzzetti and
                  Fabio Massimo Zanzotto and
                  Andr{\'{e}} Freitas},
  title        = {Teasing LLMs Adapted to Italian},
  booktitle    = {Proceedings of the 9th Italian Conference on Computational Linguistics,
                  Venice, Italy, November 30 - December 2, 2023},
  series       = {{CEUR} Workshop Proceedings},
  volume       = {3596},
  publisher    = {CEUR-WS.org},
  year         = {2023},
  url          = {https://ceur-ws.org/Vol-3596/short18.pdf},
  timestamp    = {Tue, 02 Jan 2024 17:44:44 +0100},
}

@misc{basile2023llamantino,
      title={LLaMAntino: LLaMA 2 Models for Effective Text Generation in Italian Language}, 
      author={Pierpaolo Basile and Elio Musacchio and Marco Polignano and Lucia Siciliani and Giuseppe Fiameni and Giovanni Semeraro},
      year={2023},
      eprint={2312.09993},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}

  ```

# Dataset Description

- **Homepage:** https://allenai.org/data/drop
- **Repository:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Paper:** https://aclanthology.org/N19-1246/
- **Paper:** https://arxiv.org/abs/1903.00161
- **Point of Contact:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Size of downloaded dataset files:** 8.30 MB
- **Size of the generated dataset:** 110.91 MB
- **Total amount of disk used:** 119.21 MB

### Dataset Summary

DROP: A Reading Comprehension Benchmark Requiring Discrete Reasoning Over Paragraphs.
. DROP is a crowdsourced, adversarially-created, 96k-question benchmark, in which a system must resolve references in a
question, perhaps to multiple input positions, and perform discrete operations over them (such as addition, counting, or
 sorting). These operations require a much more comprehensive understanding of the content of paragraphs than what was
 necessary for prior datasets.


## Dataset Structure

### Data Instances

#### default

- **Size of downloaded dataset files:** 8.30 MB
- **Size of the generated dataset:** 110.91 MB
- **Total amount of disk used:** 119.21 MB

An example of 'validation' looks as follows.
```
This example was too long and was cropped:

{
    "answers_spans": {
        "spans": ["Chaz Schilens"]
    },
    "passage": "\" Hoping to rebound from their loss to the Patriots, the Raiders stayed at home for a Week 16 duel with the Houston Texans.  Oak...",
    "question": "Who scored the first touchdown of the game?"
}
```

### Data Fields

The data fields are the same among all splits.

#### default
- `passage`: a `string` feature.
- `question`: a `string` feature.
- `answers_spans`: a dictionary feature containing:
  - `spans`: a `string` feature.

### Data Splits

| name  |train|validation|
|-------|----:|---------:|
|default|77409|      9536|
