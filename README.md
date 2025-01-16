# Implied NLI

Code & resources for the paper [Entailed Between the Lines: Incorporating Implication into NLI](https://arxiv.org/abs/2501.07719)

### Dataset Overview
**Implied NLI**, or **INLI** is a corpus of 10k premises that mirror real-world communication and 40k hypotheses that are implied, explicit, neutral, and contradictory.

* Number of examples: 40,000
* Number of labels: 4 (implied entailment, explicit entailment, neutral, contradictory)

On top of the raw data, we also include all prompts used to generate INLI, all human annotations described in the paper, and the outputs of the LLM experiments described in the paper.

For more details on the design and content of the dataset, please see [our paper](https://arxiv.org/abs/2501.07719)

### Data Format
Our raw dataset is split into three csv files. 

* Size of training dataset: 32,000
* Size of test dataset: 4,000
* Size of validation dataset: 4,000

In each of these files, one row represents a premise and four corresponding hypotheses. These files include the following columns:

* `dataset`: The original dataset containing the conversation or social norm used to create the premise
* `premise`: A premise
* `implied_entailment`: A hypothesis implicitly entailed in the premise
* `explicit_entailment`: A hypothesis explicitly entailed in the premise
* `neutral`: A hypothesis neither entailed nor contradicted by the premise
* `contradiction`: A hypothesis contradicted by the premise

## Citation
```
@misc{havaldar2025entailedlinesincorporatingimplication,
      title={Entailed Between the Lines: Incorporating Implication into NLI}, 
      author={Shreya Havaldar and Hamidreza Alvari and Alex Fabrikant and John Palowitch and Mohammad Javad Hosseini and Senaka Buthpitiya},
      year={2025},
      eprint={2501.07719},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2501.07719}, 
}
```

## Contact
[Shreya Havaldar](https://shreyahavaldar.com/)

## Disclaimer
INLI may contain premises and hypotheses involving sensitive content, e.g. descriptions of violence, harassment, profanity, etc. All such content originates from the datasets INLI is built off of (Ludwig, Circa, NormBank, SocialChem) and was not introduced by Gemini during the generation of INLI. All such content is purely hypothetical and not based on real people or events. Anyone using this dataset should be aware of these limitations of the dataset.
