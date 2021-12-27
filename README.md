# doi.org/10.1007/s12021-021-09548-1


The implementation of TE-HI-GCN in paper:

Lanting Li et.al "TE-HI-GCN: An Ensemble of Transfer Hierachical Graph Convolutional Networks for Disorder Diagnosis." 
# code by 

General code was developed by Lanting Li

https://doi.org/10.1007/s12021-021-09548-1


this [link](https://drive.google.com/file/d/1UuNYIQ6wDg_C4EtW88pWVbqvZI_vKpF6/view?usp=sharing) of article. 


# Require

| Library      | Version     | Purpose     |
| :------------- | :----------: | -----------: |
|  Pytorch | 1.4.0   | Deep learning library for tensor transformations    |
| Torchvision | 0.2.2 | library required by pytorch |
| Numpy  | 1.18.1 | Datascience library for creating and manipulating arrays in python  |
| sklearn | 0.23 | Machine learning library used to output area under the curve and other stats. |
| matplotlib | 3.1.2 | A visualization library required by sklearn to generate the 2D graphs. |
| Pandas | 0.25.3 | Datascience library for working with tabular data |
| Nibabel  | 3.0.0 | Library for loading in MRI scans into python  |
| Tqdm  | 4.42.1 | library for outputting progress to the console.  |



# Reproducing Results

## For ABIDE Datasets：

mkdir model

cd model

mkdir <fGCN/hiGCN/ehiGCN>  (choose a floder name that you need)

cd <fGCN/hiGCN/ehiGCN>

mkdir <atlas name>

1、f-GCN: python train-fGCN.py

2、HI-GCN: python train-hiGCN.py

3、E-HI-GCN: python train-ehiGCN.py

4、TE-HI-GCN: 

Train the model of Transfer learning part that you need.

Load the Transfer learning part into the E-HI-GCN model.

Then, python train-ehiGCN.

## For ADNI Datasets：

Using the code in the folder: ADNI.

Other operations are consistent with the ABIDE datasets.

Change "name" in these codes when you need to product results of different atlas.

Change "thr" in train-fGCN.py when you need to product results with different thresholds.
