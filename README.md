# MLOps Assignment 1
# MLOps Assignment 1 – House Price Prediction (Boston Housing Dataset)

##  Overview
This repository implements a comprehensive ML workflow for predicting house prices using the Boston Housing Dataset.  
We trained and evaluated two models:  
- **Decision Tree Regressor** (`dtree` branch)  
- **Kernel Ridge Regressor** (`kernelridge` branch)  

The project also includes a **GitHub Actions CI pipeline** to test the models on every push to `kernelridge automatically`.

---

##  Setup Instructions

# 1. Clone Repository

git clone (https://github.com/KishanBouri/mlops_assignment1)

cd mlops_assignment1

# 2. Create Environment

conda create -n mlops_a1 python=3.9 -y
conda activate mlops_a1

# 3. Install Dependencies

pip install -r requirements.txt

# 4. Running Models Locally
-Run Decision Tree (from dtree branch or main after merge)
python train.py

-Run Kernel Ridge (from kernelridge branch)
python train2.py

# 5.  GitHub Actions CI

The CI/CD pipeline is configured to run on push to the kernelridge branch.

It will:
1. Checkout code
2. Set up Python environment
3. Install dependencies
4. Run both train.py and train2.py
5. Print their MSE scores in the GitHub Actions logs

# 6. Performance Comparison

Model	Test MSE

Decision Tree Regressor	10.416078431372549

Kernel Ridge Regressor	28.838639363498928



# 7. Branches

-main → contains README and merged code

-dtree → DecisionTreeRegressor implementation

-kernelridge → KernelRidge implementation + GitHub Actions CI



