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
 