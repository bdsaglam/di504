# Notes

The evaluation metric for the competition is mean F1 score with macro.
https://www.kaggle.com/buinyi/understanding-the-evaluation-metric-cv


## Training

We observed that shallow models such as resnet18 outperforms deep models such as resnet101 
in this task. This is due to the fact that the plant pathologies are usually cover 
small number of pixels in the image, i.e., they're small objects. 
Deep CNNs lose the granularity of features required to identify such small objects; hence,
result in inferior performance.


## Resources

- Kaggle competition
https://www.kaggle.com/c/plant-pathology-2021-fgvc8

- resized dataset
https://www.kaggle.com/ankursingh12/resized-plant2021

- a submission with fastai
https://www.kaggle.com/ankursingh12/fastai-plant2021-starter-training

- resizing with PIL vs Torch vs Open CV
https://tcapelle.github.io/pytorch/fastai/2021/02/26/image_resizing.html

- fastai inference with TTA
https://www.kaggle.com/teykaihong/fgvc8-fastai-inference

- EfficientNet
https://www.kaggle.com/khoongweihao/insect-augmentation-et-al

- duplicate samples with different labels
https://www.kaggle.com/nickuzmenkov/pp2021-duplicates-revealing
https://www.kaggle.com/c/plant-pathology-2021-fgvc8/discussion/229851

- EfficientNet and Focal Loss
https://www.kaggle.com/crissallan/pytorchlightning-efficientnet-focalloss-inference