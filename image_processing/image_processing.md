# Image processing notes

2022-04-24

## Create a conda environment for image processing

```
# conda env remove -n cv2
conda create -y --name cv2 pip python=3.8
conda activate cv2
conda install pandas numpy matplotlib -c conda-forge --quiet --yes
conda install -c conda-forge opencv --quiet --yes
python -m pip install -r requirements.txt
python -m ipykernel install --user --name cv2 \
    --display-name "Python (cv2)"
```

## Create a conda environment for pytorch and fastai

```
conda create -y --name fastai pip python=3.8
conda activate fastai
conda install -c fastchan fastai anaconda --quiet --yes
conda install -c fastai nbdev fastbook --quiet --yes
python -m ipykernel install --user --name fastai \
    --display-name "Python (fastai)"
```

## TED talk about Imagenet

https://www.ted.com/talks/fei_fei_li_how_we_re_teaching_computers_to_understand_pictures?language=en

## Computing resources

You will need a computer with a GPU (like Nvidia GeForce GTX 1080 Ti Graphics Cards or better) to run code in a reasonable amount of time.

Alternatively, Kaggle or Google Colab with GPU runtime enabled is a good choice.

## Using google colab

 - Make a **Copy to Drive**
 - Change **Runtime** to **GPU**
 - Run first cells, when prompted permit access to Google Drive files **Connect to Google Drive**
 
 
 ## Traditional feature extraction ideas
 
 - Convert images to thumbnail size (e.g. 8x8 = 64pixels) and use pixels as features
 - Use binned histogram values as features to determine overall picture callers
 - Use gray_scale to measure image brightness (e.g. binned histogram on gray scale image)
 
 ## Fastai
 
 Video course, a book and other resources for Deep Learning
 
 A user-friendly python package to use with Pytorch
 
 https://www.fast.ai/
 
 ## Homework task (04/24)
 
 1. Create a dataset of images in two distinct classes in separate folders, at least 100 images each. Use specific tools, or python code examples here:  https://course.fast.ai/images
 2. Create image features dataset for these images
 3. Train random forest binary classification algorithm
 4. Report accuracy, describe images, which are incorrectly predicted
 5. Do not forget to have train and validation sample splits
 
 ## Resources:
 - ML book: https://learning.oreilly.com/library/view/hands-on-machine-learning/9781492032632/
 - Github notebook for the book https://github.com/ageron/handson-ml3
 
 ## Kagle
 - Enable GPU in settings on the right
 - You can import notebooks via `File > Import Notebook`
 
  ## Homework task (04/30)
  
  1. Use your dataset (or create a new one)
  2. Resize images to common size (e.g. 224\*224) (crop vs stretch - recommend the last)
  3. Test model performance on validation set using MLP (you can experiment with layer sizes)
  4. Test model performance on validation set using simple CNN with conv and poolling layes (you can experiment with layer sizes)
  5. Test model performance on validation set using simple CNN with conv and poolling layes and added BatchNorm and Dropout (you can experiment with layer sizes)

 