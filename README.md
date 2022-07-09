# BM3
Pytorch implementation for "Bootstrap Latent Representations for Multi-modal Recommendation"

## Overview of BM3
<p>
<img src="./images/bm3.png" width="800">
</p>

## Data  
Download from Google Drive: [Baby/Sport/Elec](https://drive.google.com/drive/folders/1Fk21441EO1l7wgOOARh2thu4FjgtKWQp?usp=sharing)  
The data already contains text and image features extracted from Sentence-Transformers and CNN.  

## How to run
`python main.py -d baby`

You may specify other parameters in CMD or config with `configs/model/*.yaml` and `configs/dataset/*.yaml`.

## Best hyper-parameters for reproducibility
We report the best hyper-parameters of BM3 to reproduce the results in Table I. of our paper as:  

| Datasets | layers | dropout | reg_weight |
|----------|--------|---------|------------|
| Baby     | 1      | 0.5     | 0.1        |
| Sports   | 1      | 0.5     | 0.01       |
| Elec     | 2      | 0.3     | 0.1        |

 