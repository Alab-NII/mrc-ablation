# Input Ablation for Machine Reading Comprehension using BERT

Our codebase is extended from [huggingface's BERT implementation](https://github.com/huggingface/transformers) (originally `huggingface/pytorch-pretrained-bert` as of Nov. 2018).

### Datasets

#### In the paper

##### Answer extraction

- CoQA
- DuoRC
- HotpotQA
- SQuAD v1.1
- SQuAD v2.0

##### Multiple Choice

- ARC
- MCTest
- MultiRC
- RACE
- SWAG

#### Not in the paper

- OpenBookQA
- TextworldsQA
- QA4MRE

### Scripts

- `run_ans_extr.py`  runs training/evaluation for answer extraction datasets
- `run_mcmrc.py` runs training/evaluation for multiple choice datasets
- `input_ablation_ans_extr.py` provides ablation methods for answer extraction datasets
- `input_ablation_mcmrc.py` provides ablation methods for multiple choice datasets
- `processor.py` provides the preprocessing methods for the datasets above
- `modeling.py` includes the model for multiple choice
