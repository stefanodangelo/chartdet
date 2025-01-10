## What is ChartDet?
**ChartDet** is simply the implementation of the Swin Transformer block used by the ChartEye model for chart type classification (see paper [here](https://arxiv.org/abs/2408.16123)).

However, despite the model can be trained to classify each different type of chart, it was here trained to discern charts from other images.

The training dataset contains:
- 22,923 chart images from the [ICPR2022 CHARTINFO UB PMC competition dataset](https://www.kaggle.com/datasets/pranithchowdary/icpr-2022?resource=download-directory)
- 20009 general images sampled from the [DomainNet dataset](https://paperswithcode.com/dataset/domainnet)
- 9991 general images from the [PACS dataset](https://paperswithcode.com/dataset/pacs)

All the notebooks in this repository were used for training, except [this one](./2.1%20chart_multiclassification_training.ipynb), which is still under experimentation.

The main notebook where training was done is: [2. chart_detection_training](./2.%20chart_detection_training.ipynb).

## How to use
The trained model is available on HuggingFace at [this link](https://huggingface.co/stefanodangelo/chartdet). 

## What can be improved?
Future improvements include:
- adding more images to the training set from the existing datasets (DomainNet and ICPR2022)
- classifying each type of chart (e.g. bar, pie, etc.)
- using other datasets to add new types of general images to help the model generalize even more (e.g. diagrams, outdoor pictures, etc.)
