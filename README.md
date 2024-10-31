# A Comparative Analysis of Large Language Models For Text Summarization

## Running the Experiments 
This project includes code for fine-tuning and evaluating various transformer models for text summarization. Below are instructions on how to run these files: 

### Fine-Tuning the Models 
Each model is fine-tuned and trained separately using the provided datasets (BBC News and CNN/DailyMail) meaning there are 2 different files for the 2 different datasets. The notebook files are named accordingly: 
1. BART_tuning_BBCNews.ipynb
2. BART_tuning_CNN_DailyMail.ipynb
3. T5_tuning_BBCNews.ipynb
4. T5_tuning_CNN_DailyMail.ipynb
5. Pegasus_tuning_BBCNews.ipynb
6. Pegasus_tuning_CNN_DailyMail.ipynb

All the notebooks are expected to be run independently and with the datasets associated with the name of the notebook file. The same step can be repeated for all the notebook files and the trained model will be saved as “fine_tuned_’modelname’_’datasetname’”. 

### Evaluating the Models 
After training, the models can be evaluated using the datasets provided in the test data folder found in the ‘Data’ folder of the artefact. There are already functions set in place to carry out evaluation of all the models on each row of data in the dataset using their ROGUE, BLEU and METEOR scores. The results are then aggregated into the mean values and used for evaluation. 

### Reproducing the Results 
The results can be reproduced by following the steps below: 
#### Fine-Tune the Models 
Follow the instructions above to fine-tune each of the models on both datasets.

#### Evaluate the Models 
Run the evaluation scripts to obtain the performance metrics for each model. 

#### Compare the Results 
The evaluation results will be saved in a .csv file called ‘final_results.csv’, which can be analyzed and compared using the provided visualization scripts.
