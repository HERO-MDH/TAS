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
