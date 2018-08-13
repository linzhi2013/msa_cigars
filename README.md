# msa_cigars

## 1 Introduction

`msa_cigars` is a tool to get the CIGARs of a multiple sequence alignment. ONE alignment in the input file is assumed! CIGARs are in respect of the reference sequence. By Guanliang MENG, see https://github.com/linzhi2013/msa_cigars. 

## 2 Installation

    pip install msa_cigars

There will be a command `msa_cigars` created under the same directory as your `pip` command.

## 3 Usage
    
    $ msa_cigars
    usage: msa_cigars [-h] -i <FILE> -refseq_id <STR> [-n <STR>] [-g <STR>]
                     [-f <FORMAT>] [-o <FILE>]

        To get the CIGARs of a multiple sequence alignment.
        ONE alignment in the input file is assumed!

        CIGARs are in respect of the reference sequence.

        'O' normal bases, e.g. A, T, G, C
        '-' deletion
        'N' unknown base

            seq - - - N N N O O O
         refseq - N O N - O O N -
          cigar P n D B u U M N I

        By Guanliang MENG,
        see https://github.com/linzhi2013/msa_cigars.

        optional arguments:
          -h, --help        show this help message and exit
          -i <FILE>         input msa file
          -refseq_id <STR>  MsaCigars class uses regular expression to find out the
                            sequence id of refseq. Thus, make sure the value of
                            'refseq_id' option is unique among the input msa file.
          -n <STR>          character of unknown base [N]
          -g <STR>          character of gap base [-]
          -f <FORMAT>       the msa format [fasta]
          -o <FILE>         outfile name [stdout]


## 4 Author
Guanliang MENG

## 5 Citation
Currently I have no plan to publish `msa_cigars`.

However, since `msa_cigars` makes use of `Biopython`, you should also cite it if you use `breakSeqInNs_then_translate` in your work:

    Peter J. A. Cock, Tiago Antao, Jeffrey T. Chang, Brad A. Chapman, Cymon J. Cox, Andrew Dalke, Iddo Friedberg, Thomas Hamelryck, Frank Kauff, Bartek Wilczynski, Michiel J. L. de Hoon: “Biopython: freely available Python tools for computational molecular biology and bioinformatics”. Bioinformatics 25 (11), 1422–1423 (2009). https://doi.org/10.1093/bioinformatics/btp163

Please go to `http://www.biopython.org/` for more details.







