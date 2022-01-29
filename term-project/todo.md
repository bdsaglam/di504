
- Literature Search
    + EfficientNet 
    - Class imbalance
        + Focal loss paper
        - Bag of tricks paper?
    - Resnet?
+ Dataset inspection
    + Sample size
    + Class distribution
- Training
    + Loss function
        + BCE
        + FocalLoss
    + Choose a baseline model
    - Choose model architectures
        + ResNet
        + EfficientNet
    - Techniques and tricks
        + Augmentation
        + imagenet pretrained
        + fp16
        + 1-cycle lr policy
        + weighted loss
        - oversampling
    - Hyperparam optimization?
        + Experiment tracking with wandb
- Inference
    + TTA
    + Export & load
    + Submit to Kaggle
- Paper
    - Introduction where you define your problem.
    - Literature review
    - Dataset and its details
    - Methods
        - Image augmentation light, heavy
        - Define F1 macro and samples
        - TTA
    - Results
        - baseline model
        - experiment results table
        - give link to the public wandb experiments
        - ROC curve per class
        - report test performance of the best model
    - Conclusion and Discussion
    - References
- Presentation


## Project Requirements

You are expected to submit a Jupyter notebook file (notebook file is recommended but you may send your entire ready-to-run-project-zip as well), helper files (if needed), and a report. Please don’t submit pre-trained weights and datasets. If they are large files, give the links to the original download locations (if they are not available just upload it to the cloud).
Your Jupyter(*.ipynb) file should contain cell outputs. These outputs should contain parameters like Epoch loss, train, validation and test graphs, network model, data size so on. Don’t forget to comment on the lines so everybody can understand what each cell block is responsible/doing.
Presentation: You should prepare a presentation about your paper and record it as a video (or present it live in Zoom, your choice). It should take a maximum of 8 minutes. You will be informed later to where you are expected to upload the video. After the presentations are uploaded, we may contact you to ask some further questions if needed.
Your project report and codes: should clearly explain what your project is, your efforts and experiments. The paper report should be a maximum of 7 pages long and should follow the IEEE conference format1.

Your report should include;
- Introduction where you define your problem.
- Literature review: A minimum of three papers is expected to be read and referenced properly. It is important to
select papers which are peer-reviewed. Check the reference fields properly. Ensure that there are no missing fields
(some Arxiv papers have already been published. Use these publication names instead of referencing to Arxiv).
- Dataset and its details: You need to give details about your dataset and present a descriptive analysis.
- The method that you are going to use: Ensure to make hyperparameter optimization and report the details of the steps. You can use existing solutions such as Optuna2.
- Results you obtained: You need to make a comparison using well-known metrics with a baseline method. You can make an ablation study if it applies to your study.
- Conclusion and Discussion
- References