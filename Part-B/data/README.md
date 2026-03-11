# Toy Sparse Dataset for AdaGrad Reproduction

## Source
The dataset was **synthetically generated** using the `make_classification` function from the **scikit-learn** library.

---

## How the Dataset Was Created
The dataset was generated using a **Python script** in `task_2_1.ipynb`.

Key details:
**Number of samples:** 1,000  
**Number of features:** 20  

To simulate situations similar to **text classification problems** (where AdaGrad performs well), an **artificial sparsity mask** was applied. This mask sets approximately **85% of the feature values to 0.0**, making the dataset **sparse**.

---

## How the Dataset Is Used
This dataset is used in the notebooks:

- `task_2_2.ipynb`
- `task_2_3.ipynb`

In these notebooks, the dataset is used to train a **Logistic Regression model**.

### Purpose of the Experiment
The goal is to test whether the **AdaGrad optimization algorithm** can adapt its **learning rates** to better learn from the **rare non-zero informative features**, compared to a **standard Gradient Descent baseline**.