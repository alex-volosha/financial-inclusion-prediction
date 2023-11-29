# Financial inclusion in Africa 
 Find a notebook where I demonstrate the way I created different machine learning models to predict which individuals are most likely to have or use a bank account. The models and solutions developed can provide insights into some of the key factors driving individuals’ financial security.


---

Click on "Use this Template" (Green button)
![alt text](./images/financial_inclusion.png)


Add description of: 

A) What needs to be completed to be done with the milestone

B) The definition of done: what will your result look like when you have completed the milestone? (check the provided format)
![alt text](./images/create_milestone.png)

Now navigate to "issues".

Assign issues to milestones, give it assignees (people who will work on the task). 
![alt text](./images/tasks_to_mileston.png)



## Requirements and Environment

Requirements:
- pyenv with Python: 3.11.3

Environment: 

For installing the virtual environment you can either use the Makefile and run `make setup` or install it manually with the following commands: 

```Bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Usage

In order to train the model and store test data in the data folder and the model in models run:

```bash
#activate env
source .venv/bin/activate

python example_files/train.py  
```

In order to test that predict works on a test set you created run:

```bash
python example_files/predict.py models/linear_regression_model.sav data/X_test.csv data/y_test.csv
```


