# BM3
Pytorch implementation for "Bootstrap Latent Representations for Multi-modal Recommendation"

## Overview of BM3
<p>
<img src="./images/bm3.png" width="800">
</p>

## Data  
Download from Google Drive: [Baby/Sports/Elec](https://drive.google.com/drive/folders/13cBy1EA_saTUuXxVllKgtfci2A09jyaG?usp=sharing)  
The data already contains text and image features extracted from Sentence-Transformers and CNN.  

## How to run
1. Put data folder under `data` dir.
2. Enter `src` folder and run with  
`python main.py -m bm3 -d baby`  
You may specify other parameters in CMD or config with `configs/model/*.yaml` and `configs/dataset/*.yaml`.

## Best hyper-parameters for reproducibility
We report the best hyper-parameters of BM3 to reproduce the results in Table III of our paper as:  

| Datasets | layers | dropout | reg_weight |
|----------|--------|---------|------------|
| Baby     | 1      | 0.5     | 0.1        |
| Sports   | 1      | 0.5     | 0.01       |
| Elec     | 2      | 0.3     | 0.1        |

 
