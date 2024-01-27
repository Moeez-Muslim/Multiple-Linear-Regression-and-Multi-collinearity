# Multiple Linear Regression and Multi-collinearity

## Overview
This repository contains code for implementing a Multiple Linear Regression model using the Iris Dataset. The dependent feature in focus is the **Petal Width**, while the independent features include **Sepal Length** and **Petal Length**. The code demonstrates the identification of confounding variables and addresses multi-collinearity to streamline the model.

## Files
- **iris.csv**: The dataset used for the analysis.
- **multiple_linear_regression.py**: Python script containing the code for the Multiple Linear Regression model.
- **README.md**: This file, providing an overview of the project.

## Requirements
Ensure you have the following libraries installed to run the code:
- NumPy
- Pandas
- PyMC
- ArviZ
- Matplotlib

Install them using the following:
```bash
pip install numpy pandas pymc3 arviz matplotlib
```

## Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/Moeez-Muslim/Multiple-Linear-Regression-and-Multi-collinearity.git](https://github.com/Moeez-Muslim/Multiple-Linear-Regression-and-Multi-collinearity.git)
   cd Multiple-Linear-Regression-and-Multi-collinearity
   ```

2. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook multiple_linear_regression.ipynb
   ```

3. The script will output the summary statistics and forest plot, providing insights into the model's coefficients and the identification of confounding variables.

## Model Details
### Initial Model (using X1 and X2)
- **Dependent Variable:** Petal Width
- **Independent Variables:** Sepal Length (X1), Petal Length (X2)
- **Model:** Multiple Linear Regression
- **Results:**
  - Intercept(α): -0.01
  - Slope1(β1): -0.082
  - Slope2(β2): 0.449

### Identifying Confounding Variables
- A forest plot is used to identify that X1 is a confounding variable as its coefficient (β1) is almost 0.

### Addressing Confounding (dropping X1)
- The model is redefined, removing the confounding variable X1.
- The new model only uses X2, simplifying the model without compromising accuracy.

## Conclusion
The refined model demonstrates reduced complexity with comparable accuracy, highlighting the importance of identifying and addressing confounding variables in multiple linear regression.

Feel free to explore and adapt the code for your specific use case. If you have any questions or suggestions, please open an issue or reach out.

Happy coding!
