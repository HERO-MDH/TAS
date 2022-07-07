# TAS: Ternarized Neural Architecture Search for Resource-Constrained Edge Devices
An Pytorch Implementation of the paper [https://www.es.mdh.se/pdf_publications/6351.pdf] (DATE 2022)

If you find any part of our code useful for your research, consider citing our paper.

```
@inproceedings{loni2022tas,
  title={TAS: Ternarized Neural Architecture Search for Resource-Constrained Edge Devices},
  author={Loni, Mohammad and Mousavi, Hamid and Riazati, Mohammad and Daneshtalab, Masoud and Sj{\"o}din, Mikael},
  booktitle={2022 Design, Automation \& Test in Europe Conference \& Exhibition (DATE)},
  pages={1115--1118},
  year={2022},
  organization={IEEE}
} 
```
# Intoduction 
we propose (i) a new cell template for ternary networks with maximum gradient
propagation; and (ii) a novel learnable quantizer that adaptively
relaxes the ternarization mechanism from the distribution of the
weights and activation function

# Searching Architectures
To search architectures, use the following command.
```
python src/search.py --save [ARCH_NAME]
```
*  [ARCH_NAME]: the name of the searched architecture

# Training Searched Architectures from scratch
 train our best searched cell on CIFAR10, use the following command.
```
python src/train.py --learning_rate 0.05 --save [SAVE_NAME] --arch TER_ARCH_In_GENOTYPE --parallel 
```
train our best searched cell on ImageNet, use the following command.
```
python src/train_imagenet.py --data [PATH_TO_IMAGENET] --arch TER_ARCH_In_GENOTYPE --model_config [MODEL_CONFIG] --save [SAVE_NAME]
```
# Contributors

Some of the code in this repository is based on the following amazing works.
* [https://github.com/gistvision/bnas]
