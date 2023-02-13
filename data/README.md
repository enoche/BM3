Dataset dirs.

# Preprocessing from raw data 从原始数据处理
- datasets: [Amazon](http://jmcauley.ucsd.edu/data/amazon/links.html)  
-- Rating file in `Files/Small subsets for experimentation`  
-- Meta files in `Per-category files`, [metadata], [image features]

## Step by step
All Jupyter notebooks can be found in the [`preprocessing`](https://github.com/enoche/MMRec/tree/master/preprocessing) folder of our [MMRec framework](https://github.com/enoche/MMRec).   
1. Performing 5-core filtering, re-indexing - `run 0rating2inter.ipynb`
2. Train/valid/test data splitting - `run 1spliting.ipynb`
3. Multimodal information preprocessing, TODO