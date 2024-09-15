# kaggle-isic2024 5th Place Winning Solution (Table Part)

This is the repository of part of 5th winning solution of "ISIC 2024 - Skin Cancer Detection with 3D-TBP" in kaggle.
https://www.kaggle.com/competitions/isic-2024-challenge/discussion/533056

![solution](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F3948967%2F38ce6eb11d8320552850efd2a20a1d87%2Fimage1.png?generation=1725877390031631&alt=media)

This repository contains Tabular Model2 in the pipeline above. 


## Contents
```sh
.
├── README.md
└── src
    ├── data
    │   ├── ensemble_oof_df_20240914.csv
    │   ├── preds_conv_nes.parquet
    │   ├── preds_eva_nes.parquet
    │   ├── sub71
    │   ├── sub73
    │   ├── sub75
    │   └── sub77
    ├── past_train_img_scripts
    ├── past_train_table_scripts
    ├── main.ipynb # main train script.
    ├── isic_ensemble_table_only.ipynb 
    ├── isic_ensemble_with_img.ipynb
    └── past_img_train
```

## Running the Notebooks
- To create the model, run main.ipynb in Google Colab using GPU (T4) and High Memory settings (around 50GB).
- For verification of the ensemble code, execute the isic_ensemble_table_only.ipynb notebook.
  - Note: The actual final submission was created using isic_ensemble_with_img.ipynb, but due to the large size of out-of-fold data required, that notebook is too heavy to be hosted on GitHub.
