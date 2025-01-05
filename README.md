## What is ChartDet?
**ChartDet** is simply the implementation of the Swin Transformer block used by the ChartEye model for chart type classification (see paper [here](https://arxiv.org/abs/2408.16123)).

However, despite the model can be trained to classify each different type of chart, it was here trained to discern  charts from other images.

Training images were taken from the [ICPR2022 CHARTINFO UB PMC competition dataset](https://www.kaggle.com/datasets/pranithchowdary/icpr-2022?resource=download-directory), the [PACS](https://paperswithcode.com/dataset/pacs) and [DomainNet](https://paperswithcode.com/dataset/domainnet) datasets.


## How to use
All the notebooks in this repository were used for training, except [this one](./2.1%20chart_multiclassification_training.ipynb), which is still under experimentation.

The main notebook where training was done is: [2. chart_detection_training](./2.%20chart_detection_training.ipynb).
