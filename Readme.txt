Read-me

The provided zip-file contains the following files and folders:

* RUN_WINE and RUN_MNIST are the most important notebooks, containing all work to reproduce the results in the report. You need to change "filepath" in order to run the notebooks. All code chunks including training and validation are commented out. Pre-trained models are used which are stored in another folder.

RUN_WINE and RUN_MNIST are both structured as follows:
- Data Exploration
- Functions definition for plotting PCA/TSNE results and computing loss
- General model specification for baseline but also for epistemic and aleatoric modeling
- Fitting, evaluating baseline
- Fitting, evaluating epistemic model, calculate epistemic uncertainties, visualize results
- Fitting, evaluating aleatoric model, calculate aleatoric uncertainties, visualize results
- Fitting, evaluating epistemic and aleatoric model, calculate epistemic and aleatoric uncertainties, visualize results
- Further visualizations, including effect of modeling uncertainties on accuracy
- Quality check with ECE

Some other results such as loss attenuation, overlap between result and LOF computations are found at different positions in the two notebooks. The headlines are however indicative of which result to find where. 

The corresponding pdf files show the code, but sometimes the outputs are not visible.



* trained_models contains several trained models, including models trained for hyper parameter tuning

* data contains the dataset used in the analysis

* TEST_saved_uncertainties contains the computed values for epistemic and aleatoric uncertainties (including increase of training set) and predicted classes so that all results can be reproduced in RUN_WINE and RUN_MNIST

* MNIST and WINE are the original files used to train the models. For any further output details, you can refer to these notebooks, however they may not contain all calculations conducted in RUN_WINE and RUN_MNIST

* FINAL_accuracy_loss comprises files storing accuracies and losses from trained models

* FINAL_plots includes plots which are in the report


The notebooks were created using Colab using Python 3.7.10 