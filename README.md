![](https://img.shields.io/github/downloads/ZhijianZhou01/bioaider_mutation/total)
[![](https://img.shields.io/github/downloads/ZhijianZhou01/bioaider_mutation/V1.527/total?color=red&style=flat-square)](https://github.com/ZhijianZhou01/bioaider_mutation/releases/tag/V1.527)
![](https://img.shields.io/github/downloads/ZhijianZhou01/bioaider_mutation/V.1.423/total?)

![](https://img.shields.io/badge/System-Windows/Linux/MacOS-green.svg)
[![](https://img.shields.io/badge/Doi-10.1016/j.scs.2020.102466-yellow.svg)](https://doi.org/Doi:10.1016/j.scs.2020.102466) 


### 1. Introduction
This is a command-line interface (non-GUI) of mutation analysis in [BioAider](https://github.com/ZhijianZhou01/BioAider) software.

### 2. Install and run
It's a no-installer program (although it is a bit large, it is caused by the packaged software).

How to run it? 
You could switch to the directory of software, and check the help documentation (take linux system as an example):
```
$ ./bioaider_mutation -h
```

Then, the program will output the following information:
```
-------------------------------
  Version: 1.527 (2023/02/22)
  Author: Zhou Zhijian
-------------------------------
usage: bioaider_mutation [-h] [-i INPUT] [-m MODES] [-d DATA] [-t TABLE]

optional arguments:
  -h, --help  show this help message and exit
  -i INPUT    input fasta file
  -m MODES    single modes or linked modes
  -d DATA     type of data, nt or aa or codon
  -t TABLE    number of codon table

example: bioaider_mutation -i seq.fas -m single -d codon -t 1
```

The codon table and number, Please refer to [The Genetic Codes](https://www.ncbi.nlm.nih.gov/Taxonomy/Utils/wprintgc.cgi?chapter=tgencodes#SG11).

Of course, if it's not the coding gene sequence, just nucleotides, you could enter as follows:
```
bioaider_mutation -i seq.fas -m single -d nt
```

**Note:** sequences used for mutation analysis need to be aligned in advance, and bioaider_mutation does not provide functions for multiple sequence alignment. 

### 3. Citation
Zhi-Jian Zhou, Ye Qiu, Ying Pu, Xun Huang, Xing-Yi Ge*. BioAider: An efficient tool for viral genome analysis and its application in tracing SARS-CoV-2 transmission. Sustainable Cities and Society. 2020. DIO: 10.1016/j.scs.2020.102466.

https://www.sciencedirect.com/science/article/pii/S2210670720306867
