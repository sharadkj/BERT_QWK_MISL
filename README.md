# BERT_QWK_MISL
A notebook for training a regression version of BERT to predict the scores of MISL macrostructure elements and then calculate the Quadratic Weighted Kappa.

This code draws mostly from the following repository with code and hyperparameter changes for our specific dataset: https://github.com/ceshine/pytorch-pretrained-BERT/blob/master/notebooks/Sequence%20Regression%20Model.ipynb

It is assumed that PyTorch (pytorch.org) is installed and a large GPU is highly recommended as BERT requires multiple GB of GPU memory. This paper used an NVIDIA GeForce GTX Titan X for all training. There is also an implementation of BERT in PyTorch that must be installed prior to running this notebook. The repository and installation instructions can be found here: https://github.com/huggingface/pytorch-pretrained-BERT.

Comments have been made in the notebook where changes must be made to replicate results on the users machine. To summarize, please store the file "AutomatedNarrativeAnalysisMISLData.csv" in a local directory and add this path in the first cell of the notebook.
The user must also specify a cache directory in that first cell. To replicate the expert score section, the user must also include the path to the file "ExpertScores.csv" in the relevant section. Aside from those few files, the rest of the analysis is handled in memory and self-contained in the notebook.

All data can be found at the following publicly accessible link: https://digitalcommons.usu.edu/all_datasets/79/.
