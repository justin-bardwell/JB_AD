# Predicting Conversion from Normal Cognition to Cognitive Impairment with Patch-based CNNs

## Justin Bardwell

### Supervisors: 
- **Ghulam Mubashar Hassan**
- **Farzaneh Salami**
- **Naveed Akhtar**

Overview of repository:

| Directory        | Contents of directory                                                                                                                      |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| Data             | Data selection process and scripts to download data                                                                                        |
| Final_Models     | Data split into train, test and validation. </br> Training/fine-tuning process for all models. </br> Inference and results for all models. |
| Scans_CN         | All FreeSurfer MRI files for subjects remaining congitively normal throughout the study                                                    |
| Scans_Converters | All FreeSurfer MRI files for subjects converting to cognitive impairment in the study                                                      |


Experiment 1 Results:

|     Model                   |     Accuracy    |     AUC     |     Sensitivity    |     Specificity    |
|-----------------------------|-----------------|-------------|--------------------|--------------------|
|     Voxel-based ResNet50    |     0.50        |     0.50    |     0.00           |     1.00           |
|     Patch-based ResNet50    |     0.90        |     0.99    |     0.80           |     1.00           |


Experiment 2 Results:

|     Model             |     Accuracy    |     AUC     |     Sensitivity    |     Specificity    |
|-----------------------|-----------------|-------------|--------------------|--------------------|
|     ResNet50          |     0.90        |     0.99    |     0.80           |     1.00           |
|     SEResNet50        |     0.90        |     0.99    |     0.80           |     1.00           |
|     SEResNeXt50       |     0.75        |     0.85    |     0.90           |     0.60           |
|     ResNet18          |     0.65        |     0.8     |     0.70           |     0.60           |
|     DenseNet121       |     0.85        |     0.97    |     1.00           |     0.70           |
|     Ensemble Model    |     0.85        |     0.97    |     1.00           |     0.70           |
