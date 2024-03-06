# Zindi_Cgiar_crop_damage_classification_challenge

### Competition hosted on <a href="https://zindi.africa/competitions/cgiar-crop-damage-classification-challenge">Zindi</a>

# About

### Create a machine-learning algorithm to classify crops into categories: Good growth (G), Drought (DR), Nutrient Deficient (ND), Weed (WD), and Other (including pest, disease or wind damage). The data for this challenge is a collection of smartphone images of crops.

### The Final Competition score is 0.696384917

### Final Leaderboard Rank is 152.

### The Evaluation Metric is  Log Loss.

### File information
 
 * EDA [![Open in Kaggle](https://img.shields.io/static/v1?label=&message=Open%20in%20Kaggle&labelColor=grey&color=blue&logo=kaggle)](https://www.kaggle.com/code/hari141v/cgiar-crop-damage-classification-challenge-eda)
    #### Basic image information analysis
    #### Images RGB color analysis
    #### Image similarity analysis
    #### Packages Used,
        * seaborn 
        * Pandas
        * Numpy
        * Matplotlib
        * imagehash
        * distance
        * Image
        * cv2

* Model
  ### Trained ViT Base 16 Patch 224 model on five-fold training data with various augmentations. Ten epochs were used to train the five-fold dataset, and early stopping was implemented to control overfitting by monitoring the validation log loss. The test data was predicted using the five-fold model, and test-time augmentation was applied to ensure confident predictions. The model's performance was tracked using WANDB.
  ### [Model Log](https://wandb.ai/hari141v/Cgiar_Crop_Damage_Classification_10)
