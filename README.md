# Exploring and Evaluating Attributes, Values, and Structures for Entity Alignment

The code of our EMNLP2020 paper *Exploring and Evaluating Attributes, Values, and Structures for Entity Alignment*.

## Dependencies

* python 3
* [PyTorch >= 1.0](https://pytorch.org/get-started/locally/)
* [sklearn](https://scikit-learn.org/stable/)
* [huggingface/transformers 1.1.0](https://github.com/huggingface/transformers)

## Code

1. Run the following scripts to train all the subgraphs.

```bash
>> python train_subgraph.py --gpu_id [GPU_id] --channel [choose from {Digital, Literal, Structure, Name}] --dataset [choose from {DBP15k/zh_en, DBP15k/fr_en, DBP15k/ja_en}] --load_hard_split [or not]
```

2. Run the following scripts for ensemble.

```bash
>> python ensemble_subgraphs.py --gpu_id [GPU_id] --dataset [choose from {DBP15k/zh_en, DBP15k/fr_en, DBP15k/ja_en}] --svm [or not] --load_hard_split [or not]
```

## Datasets

Download the datasets from [OneDrive](https://1drv.ms/u/s!AuQRz5abAH5T2jDOmiMlkqFP8s0Z?e=V6wNWS) and unzip it under the current folder.

## Reference

If you use the code, please cite our paper:

```bib
@inproceedings{liu2020exploring,
  title={Exploring and Evaluating Attributes, Values, and Structures for Entity Alignment},
  author={Liu, Zhiyuan and Cao, Yixin and Pan, Liangming and Li, Juanzi and Liu, Zhiyuan and Chua, Tat-Seng},
  booktitle={EMNLP},
  year={2020}
}
```

## Acknowledgement
This research is supported by the National Research Foundation, Singapore under its International Research Centres in Singapore Funding Initiative. Any opinions, findings and conclusions or recommendations expressed in this material are those of the author(s) and do not reflect the views of National Research Foundation, Singapore.