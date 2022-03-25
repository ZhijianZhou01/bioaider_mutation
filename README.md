### 1. Introduction
This is a command-line interface (non-GUI) of mutation analysis in [BioAider](https://github.com/ZhijianZhou01/BioAider) software.

### 2. Install and run
It's a no-installer, albeit a bit big, but it's the result of packaged software.
How to run it? 
You could switch to the directory of software, and check the help documentation (take linux system as an example):
```
$ ./bioaider_mutation -h
```

Then, the program will output the following information:
```
-------------------------------
  Version: 1.423 (2022/03/24)
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

### 2. Citation
Zhi-Jian Zhou, Ye Qiu, Ying Pu, Xun Huang, Xing-Yi Ge*. BioAider: An efficient tool for viral genome analysis and its application in tracing SARS-CoV-2 transmission. Sustainable Cities and Society. 2020. DIO: 10.1016/j.scs.2020.102466.

https://www.sciencedirect.com/science/article/pii/S2210670720306867
