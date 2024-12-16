@author: jessicaguan

Studies have linked birth control access to a higher quality of life. Research findings suggest that communities with higher rates of contraceptive usage experience lower crime rates. The authors further hypothesise that the correlation could be due to increased educational opportunities, financial opportunities, and a reduced number of unplanned pregnancies (N. Hill et al). However, communities in lower socioeconomic classes tend to have less access to contraceptive methods due to lack of healthcare and fewer contraceptive options. Exploring which socioeconomic factors most affect women’s access to birth control and family planning is important in knowing what resources are needed in these communities. This research paper uses neural computing methods to classify women’s contraceptive methods based on socioeconomic factors.
This project creates 2 models (multilayer perceptron and support vector machine) based on the [UCI dataset](https://archive.ics.uci.edu/dataset/30/contraceptive+method+choice) which contains information about women's characteristcs and contraceptive method choices.

requirements:
`pandas` == 1.5.3,
`sklearn.svm` == 0.0.post11,
`numpy` == 1.24.3,
`torch` == 2.0.1

instructions:
There are a total of 2 models, `final_svm_model.pkl` and `final_mlp_model.pth`. `final_svm_model.pkl` is the SVM model, and `final_mlp_model.pth` is the MLP model. Both models were trained on a dataset to classify women's contraceptive methods based on socioeconomic factors.

The hyperparameter tuning, training, and testing for the SVM model was done in `FinalContraceptiveSVM.ipynb`, and the hyperparameter tuning, training, and testing for the MLP model was done in `FinalContraceptiveMLP.ipynb`.

The test data for `final_svm_model.pkl` is saved as `svm_x_test.csv` and `svm_y_test.csv`. The test data for the `final_mlp_model.pth` is saved as `mlp_x_test.csv` and `mlp_y_test.csv`.

To reproduce the testing results, a separate file is provided called testing_reproducibility.ipynb. In this file, the code to define and load the pretrained models and load the test data is already there. Run the libraries and packages needed at the top, then run each cell to test the results.

1. Open `testing_reproductibilty,ipynb`
2. Run the cell to import needed packages
3. Run the rest of the cells in the "Test MLP model" section to load the MLP model, load the data for MLP, get the test results, reproduce the confusion matrix graph and the roc curve graph.
4. Run the rest of the cells in the "Test SVM model" section to load the SVM model, load the data for SVM, get the test results, reproduce the confusion matrix graph and the roc curve graph.
