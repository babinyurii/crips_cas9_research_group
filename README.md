# crispr_cas9
`crispr_cas9` contains two in-house scripts that are used for NGS data analysis by HBV crispr/cas9 research group. 

## Requirements
- Python 3
- Biopython
- matplotlib
- pandas

## Installation
```
pip install crispr_cas9
```

## Description
This script takes fasta alignment as an input. The input file is the result of deep sequencing reads mapping onto the reference sequence and is imported from the Geneious software.


`crispr_count_indels.py` counts exact number of insertions and deletions. The script creates excel spreadsheets with the raw count.

`crispr_create_plots.py` uses the output of the `crispr_count_indels.py` script and constructs plots and spreadsheets containg the percentage of eash indel and its position according to the reference sequence

The example of output file. Here are all the deletions found irrespective of their length: 
![bars](example_output/dels_bars.png)

And heatmap which shows both percent of indels and their lengths:
![heatmap](example_output/dels_heatmap.png)

The script was used to process sequence data for the work by Kostyushev et al.(2019)

**reference:**
1. Orthologous CRISPR/Cas9 systems for specific and efficient degradation of covalently closed
circular DNA of hepatitis B virus. Dmitry Kostyushev, Sergey Brezgin, Anastasiya Kostyusheva, Dmitry Zarifyan, Irina
Goptar, Vladimir Chulanov. Cellular and Molecular Life Sciences (accepted)
