
## For best viewing experience in this Readme File:

 **Windows/Linux**: press `Ctrl + Shift + V`

 **macOS**: press `Cmd + Shift + V`




## Team Details
* Team Name : Tech Titans
* Team ID   : 3 

## MAIL ID : 
* Emandi Devi Lakshman------22CS10022 ---       8179lakshman@gmail.com
* Sadde Suchith Reddy-------22CS10063 ---       saddasuchithreddy@gmail.com
* GMM Prabhash--------------22CS30027 ---      prabhashgolla2004@gmail.com

# DL2025 Assignment 2 - Image Captioning and Robustness Evaluation
### -> The pip install statements are mentioned at the top of the code whenever neccessary so please don't skip it
* please run the above mentioned part of each code 
* IN CASE OF ANY ERROR IN PART - A  due to the first two cells ( i.e pip install and import statements):
* Please re-run the pip install cell again and then run the import statements
* Also in part - A please note this
* since this was first done in kaggle and we have faced some issues with the meteor , We only made upto the BLEU and Rouge at first and then implemented the meteor part 

* Meanwhile we have saved the trained model from the outputs of code 
```
 For downloading the model file from google drive for testing seperately. not needed if already loaded
 !pip install -q gdown
 file_id = "199sCxfrCK8o9_e_6tlYZU6VUgfkjWTyk"
 !gdown --id {file_id} --output my_model.pth

```

### Part -A  `Part_A.ipynb`.
2. It will:
   - Train a ViT + GPT2 encoder-decoder model.
   - Evaluate BLEU, ROUGE-L, METEOR on test set.
   - Save model weights and generated captions.

### Part -B - Occlusion Robustness

1. Run `Part_B.ipynb`.
2. It will:
   - Apply occlusion at 10%, 50%, 80% levels using 16×16 patches.
   - Evaluate both custom model and SmolVLM on masked images.
   - Save and optionally load caption `.json` files.

### Part C - Caption Source Classification

1. Run `Part_C.ipynb`.
2. It will:
   - Construct dataset of triplets: `<orig_caption> <SEP> <gen_caption> <SEP> <pct>`
   - Train a BERT classifier to distinguish SmolVLM vs. custom model.
   - Report Precision, Recall, F1.

# DL_Assignment3
