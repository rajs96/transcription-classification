# transcription-classification
Using Longformer to classify transcriptions into their category of medicine

# How to Run

To run this in Colab, you need to have your `HOME_PATH` set properly in this cell:
```
# Replace with your path
HOME_PATH = '/gdrive/MyDrive/DictateMD_takehome'
DATA_PATH = join(HOME_PATH, 'data')
CSV_FILE_PATH = join(DATA_PATH, 'mtsamples.csv')
```

Then you need to have the following directory structure:
```
data
- mtsamples.csv
checkpoints
- medical-model-epoch=3-train_loss=0.07-valid_loss=0.46.ckpt
- train_losses.p
- valid_losses.p
- model_evaluation.p
```

If these are set properly, you should be able to run `solution.ipynb` in Colab with the current args set.

If you want to run the training yourself, or modify filepaths, you will need to download the notebook
and modify some of the variables (CKPT_PATH, TRAIN, etc.). You will also need a high-RAM GPU.
