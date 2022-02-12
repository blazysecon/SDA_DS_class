# SDA Data Science Class notes

## GIT

### Working with branches

```
git checkout -b your_branch_name
git status  
git add . 
git commit -m 'first day' 
git pull 
git push --set-upstream origin your_branch_name
```

### Working on the main/master branch

```
git status
git add .
git commit -m 'update class notes'
git pull
git push
```

```
git pull  # get the latest changes
git stash # if conflict, your changes will be lost
git checkout main # go back to main branch
```

### Conda

```
conda create -y --name ds39 pip python=3.9
conda activate ds39
conda install black pandas ipython statsmodels scipy \
tqdm seaborn scikit-learn --quiet --yes &&
conda install pandas-profiling glmnet shap jupyterlab \
eli5 -c conda-forge --quiet --yes &&
# also need to install nodejs and graphviz as (Mac/Windows/Linux)
# executables on your specific system
pip install pdpbox graphviz &&
jupyter labextension install @jupyter-widgets/jupyterlab-manager &&
python -m ipykernel install --user --name ds39 \
    --display-name "Python (ds39)"
```

## Visual Studio Code

For working with python scripts

## Jupyter Lab / Jupyter Notebook

For working with notebooks

## Resources

- [Kaggle learn](https://www.kaggle.com/learn)
- [Datacamp](https://app.datacamp.com/learn)

**Books**:
- [Introduction to Machine Learning with Python](https://github.com/thiagordp/machine-learning-books/blob/master/Introduction%20to%20Machine%20Learning%20with%20Python%20-%20A%20Guide%20for%20Data%20Scientists%202016.pdf)
- [Python for Data Analysis](https://www.amazon.de/-/en/Aur%C3%A9lien-G%C3%A9ron/dp/1492032646/ref=pd_bxgy_1/262-2032424-3050336?pd_rd_w=kXgIr&pf_rd_p=a2e044d8-c6c4-472e-be1b-004f9c16cb56&pf_rd_r=1ZZN7H07NDGKJ0FM6B5Y&pd_rd_r=5a081702-89eb-4f8a-960f-99fe7f0eca92&pd_rd_wg=K95M9&pd_rd_i=1492032646&psc=1)
- [Hands-on Machine Learning with Scikit-Learn](https://www.amazon.de/-/en/Wes-McKinney/dp/1491957662/ref=pd_bxgy_2/262-2032424-3050336?pd_rd_w=kXgIr&pf_rd_p=a2e044d8-c6c4-472e-be1b-004f9c16cb56&pf_rd_r=1ZZN7H07NDGKJ0FM6B5Y&pd_rd_r=5a081702-89eb-4f8a-960f-99fe7f0eca92&pd_rd_wg=K95M9&pd_rd_i=1491957662&psc=1)

## HW

- Do homework assignments on knowledge base
- Try to improve prediction accuracy by engineering and adding new features (based on aggregation, like zipcode average, and interaction terms)
- Implement WMAPE in python and test how it is similar to MAPE for predicting house prices in Seattle.
- Form 2-3 person groups
- Identify interesting question and find required data to try to solve it